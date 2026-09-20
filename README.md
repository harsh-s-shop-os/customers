# ShopOS PLG Customers — Master Context

**Read this file first.** Every live customer has its own file under `active/`; churned accounts move to `churned/`. This file explains how to read them, what patterns cut across customers, and how to maintain the set.

Last full revision: 2026-09-13. Data as of 2026-09-13 unless a customer file says otherwise.

---

## 1. Purpose & scope

ShopOS has a small set of paying self-serve ("DIY" / PLG) customers alongside a few retainer and custom-plan accounts. Ajay asked (Slack, Sep 2026) that someone track these customers' usage in PostHog, talk to them, and learn what works and what doesn't **before marketing scales acquisition**. Lobster/Harsh (product design) owns this and presents a weekly update in the WBR (Weekly Business Review) PLG section.

**In scope:** every account that pays ShopOS in any form — self-serve monthly/yearly plans, custom plans, retainers — plus recently churned paying accounts.
**Out of scope:** revenue optimisation per account; the general population of trial users (they matter for funnel work, which lives elsewhere).

**The core question this entire workspace optimizes for, for every customer without exception:**

> Where is this user getting real value from the product, where is it failing them, and what does each of those imply should get fixed.

Value and friction are two separate questions, not one — a customer file needs an answer to both, not a single verdict. Every section below (roster tags, the review loop in §8, the customer-file scaffold in §2) exists only in service of answering this for each customer; a file can be data-complete and still fail if it doesn't answer this. This is the successor to an earlier, looser framing of the same goal ("is the product working for this brand? Not how much they pay") — kept for continuity, superseded by the statement above.

---

## 2. How to read a customer file

### Tags

Each customer carries exactly one status tag. Tags describe the relationship *right now* and change over time.

| Tag | Meaning |
|---|---|
| `deriving-real-value` | Uses the product regularly and gets output or decisions from it that matter to their business. |
| `tried-not-getting-value` | Still shows up, but is not producing output or acting on results. Looking, not doing. |
| `stopped-forgotten` | No meaningful activity for weeks; may still be paying. |

The second and third tags may merge later; kept separate for now to see if the distinction earns its place.

### Scaffold — live account

Every live customer file follows this order:

1. **Tag** and one-line status
2. **Identity** — every email / workspace tied to this customer, and *why* each one is connected
3. **Who they are** — business, role, geography, how they arrived
4. **Lifecycle** — signup → activation → purchase → now, with dates
5. **Usage** — what they actually do, with numbers
6. **Health signal** — the one or two indicators that say whether this account is getting healthier or sicker
7. **Touchpoints** — every human contact ShopOS has had with them
8. **Read** — our interpretation, each claim tagged `[Certain]` / `[Likely]` / `[Guessing]`
9. **Open questions** — things to check in data, and things to ask them on a call
10. **Next action** — one concrete thing
11. **Changelog** — dated edits to this file

### Scaffold — churned account

Same skeleton, past tense, with three renamed sections: **Usage before leaving**, **Decay signal**, **Likely reason**, and **Fix** replaces Next action. This mirrors the PLG triage automation's churn posts, so a live file becomes a churn file by editing, not rewriting.

---

## 3. Roster

| Customer | File | Plan (Sep 11 list) | Tag | One-line status |
|---|---|---|---|---|
| PointTaken (Sharath) | [active/pointtaken.md](active/pointtaken.md) | Custom, 50k credits/mo | `deriving-real-value` | Agency + design partner; 3 seats; heaviest self-serve-adjacent user. Sep 17: conditional buy-in on the feed, and a new trust problem — Gavin returned contradictory numbers in one chat |
| patchandbagel | [active/patchandbagel.md](active/patchandbagel.md) | Growth $99/mo | `deriving-real-value` | Healthiest true PLG account; lives in Cowork/agents/publishing, not image generation; renewed Sep 13 and still publishing a week later |
| Dawn (Arcadia Home) | [active/dawn-arcadia-home.md](active/dawn-arcadia-home.md) | Pro yearly $180 | `deriving-real-value` | Low-frequency solo operator, returning monthly for 8 months; upgrade-curious |
| R for Rabbit | [active/r-for-rabbit.md](active/r-for-rabbit.md) | Retainer, 3 mo, $3,825 | `deriving-real-value` | 5 seats, canvas-heavy — but **zero canvas runs Sep 13–20 and the heaviest seat silent since Sep 12**; no Stripe subscription so churn alerts won't fire |
| Agilitas | [active/agilitas.md](active/agilitas.md) | Retainer $199/mo (new Sep 10) | `deriving-real-value` | 20+ seats since Nov 2025, heaviest usage in the base; the $199 line does not describe this account |
| Sidharth Suresh | [active/sidharth-suresh.md](active/sidharth-suresh.md) | Pro $19/mo | `tried-not-getting-value` | Founder of Fashnstack, building an adjacent Creative Director product. First call Sep 16; sent an unsolicited Monica audit to Ajay Sep 17 — no reply. 91 searches / 3 completed generations in 6 months. Renewal Sep 29 |
| Imran Khan (Crafeed) | [active/imran-khan.md](active/imran-khan.md) | Growth $99/mo | `tried-not-getting-value` | Two identities, zero output on either across 11 weeks — still logging in (last seen Sep 16); relationship owner unknown |
| Patricia Noble | [active/patricia-noble.md](active/patricia-noble.md) | Business $199/mo | `stopped-forgotten` | Bought 48 min after signup, silent since Jul 23, reportedly renewed again Sep 20. Paying $199/mo for 0 completed generations |
| Zeppelin | [active/zeppelin.md](active/zeppelin.md) | Plus $49/mo | `stopped-forgotten` | Only match is a Free account dormant since Apr 11; paying identity unconfirmed |
| Eustress *(churned Sep 9)* | [churned/eustress.md](churned/eustress.md) | was Pro | — | Sold on a call, 109 searches / 0 executions, cancelled after payment failure |

---

## 4. Cross-customer patterns

Each pattern lists confidence and the number of accounts it rests on. **Do not present a pattern with n ≤ 2 as settled.** Update the evidence count when a new account confirms or contradicts it.

### 4.1 Searching Spaces without running them precedes churn — `[Likely]`, n = 4
Eustress (109 searches / 0 executions → cancelled), hiaradigitals (22 / 0 → past_due), Patricia (13 / 0 → silent), and live: Sidharth (91 / 3, still paying). Sharath and Dawn — healthy — search a lot but *also* execute (412/62 re-verified 2026-09-20, and 115/72). The ratio, not the search count, is the signal.

**Counter-example found 2026-09-20:** Sunny (PointTaken) runs 1,005 searches against 96 executions created — a worse ratio than Sidharth's — while completing 1,931 Space generations, the highest output in the base. Searching heavily is evidently compatible with heavy production when the person knows what they're doing. The ratio discriminates only among accounts that are *also* producing little; it is not a standalone churn predictor. Treat §4.1 as narrower than first written.

### 4.2 Fast or assisted conversion followed by zero self-produced output ends in churn — `[Likely]`, n = 4
Eustress (Hemanth ran sample generations on a call → purchase → never generated alone), Patricia (purchase 48 min after signup → 0 generations), Imran/Crafeed (2 days then gone), hiaradigitals (bought day 4 → past_due). The purchase happened on promised or demonstrated value; the product did not carry it once the person was alone.

### 4.3 The agent/routine layer is what retains; image generation is the credit sink — `[Likely]`, n = 2
Sharath (stated on call: Gavin routines are the value, Monica ~5% of his time, images burn credits) and patchandbagel (behavioural: 145 Cowork messages, 41 published, 3 image generations). Two data points from opposite ends of the base saying the same thing. Needs a third before it goes in a WBR as a claim.

### 4.4 Heavy usage sits on human-negotiated terms, not self-serve checkout — `[Certain]` on the pattern, n = 3
PointTaken (custom plan), Agilitas (custom + Business seats), R for Rabbit (retainer with manually granted credits) account for the overwhelming majority of generations. Self-serve payers paid *before* producing anything. Pricing in the base tracks sales touch, not usage.

### 4.5 Credit cost shapes power-user behaviour — `[Likely]`, n = 2
Sharath (stated: plans every decision around credit cost; stopped "Jobs" when they leaked ~2k credits/run; 4 out_of_credits events) and Agilitas' Amit (28 out_of_credits events). Orchestrator routing is a credit cost in Sharath's model, not only image generation.

### 4.6 Multi-seat accounts retain; solo accounts churn — `[Likely]`, n = 4 vs 3
Retained: R for Rabbit (5 seats), Agilitas (20+), PointTaken (3), patchandbagel (2). Churned/at-risk: Eustress, Patricia, hiaradigitals — all single seat. Confounded with sales touch (4.4); treat as correlated, not causal.

### 4.7 Payment failure is not disengagement — `[Certain]` that the two differ, n = 2
Sidharth hit `past_due` and re-subscribed unprompted 3 months later; Eustress hit `past_due` and used it as the exit. Keep billing state and usage state as separate columns.

### 4.8 Customers judge the feed on output quality, not on the mechanic — `[Likely]`, n = 2 — **not settled**
Both accounts shown the feed prototype (Sidharth 2026-09-16, PointTaken 2026-09-17) accepted the premise — a feed of ready drafts beats a blank prompt box — and then immediately made their real judgment somewhere else. Sidharth: "it lastly depends upon how creative the feed is… the buck stops" at the output; he read the sample cards as generic within seconds and said he'd go back to prompting in chat. Pratik and Sharath: "in the right direction", followed by two rounds of *what signal actually generates this card*, and a refusal to judge it until they've sent five jobs-to-be-done and seen how they land.

Neither raised a single objection to the interaction model. The feed relocates the trust question from "can I trust this agent's output" to "can I trust this card" — it does not remove it. At n = 2 this is a hypothesis, not a finding; a third feed conversation either confirms it or breaks it.

### 4.9 Nobody reaches out until the customer is already gone — `[Certain]`, n = 4
Sidharth: six months, a card failure, and a `past_due` lapse with zero contact until 2026-09-16 — and he was *deliberately holding his credits* waiting for someone to tell him how to use the product. Patricia: bought the $199 plan, went silent in 11 days, has now renewed at least once with no human ever contacting her. Eustress: contacted on the way in (Hemanth ran the samples), never after. Imran/Crafeed: relationship owner unknown. The self-serve base is unowned by default; the accounts that get a human are the ones that already had one at purchase (§4.4).

---

## 5. Guidelines — maintaining this workspace

**Add a customer file** the day an account starts paying (self-serve checkout, custom plan, or retainer signed). Not on trial start.

**Edit in place** when something material changes: tag change, churn, reactivation, a call or Slack exchange, a new identity discovered. Add a dated line to that file's Changelog. Don't append a second copy of a section.

**Identities:** when a second email or workspace for the same customer turns up, add it to that file's Identity section with why it's connected. Never create a second file for the same customer.

**Churn:** move the file to `churned/`, switch the scaffold to past tense, fill Likely reason and Fix. Keep the history. Update the roster row.

**This file** changes only for: roster changes, a new or revised cross-customer pattern (with evidence count), a new guideline, or a change to the agents-only sections. Single-customer detail never lives here.

**Open questions** live in the customer's file, not here, so they get asked on the next call with that customer.

**Tags** are the only categorisation. Don't introduce buckets, tiers, or segments in customer files; if a new tag is needed, add it to the table in §2 first.

---

## 6. Data sources & how to read them — *agents only*

Humans can skip this section.

- **PostHog:** project **ShopOS Pro Prod** (id 231368), org ShopOS, US cloud, timezone UTC. Group type `workspace` (key = `org_…`).
- **Paying-user filter:** a person is a payer when `subscriptionStatus IN ('active','past_due')` AND `active_plan != 'Free'`. Every new signup receives a 14-day Business trial, so `hasSubscription = true` / `active_plan = 'Business'` / `subscriptionStatus = 'trialing'` is the default state of a fresh signup, not a payer. Exclude `@shopos.ai` emails.
- **Aggregate by email, not `person_id`.** The same human often has 2–3 person rows (one created at anonymous visit, one at `$identify` with `workspace_id`). Customer files list every email; queries should `GROUP BY coalesce(person.properties.email, properties.email)`.
- **Person properties are snapshots**, written at ingestion. `totalCredits`, `remainingMonthlyCredits`, `renewalDate`, `last_seen_at` on the `persons` table can be stale. Compute recency from `events.timestamp`.
- **Purchase events** (`subscription_purchase_completed`, `topup_purchase_completed`) exist from ~2026-04-12. Earlier purchases (Dawn's yearly, PointTaken's custom) have no event. R for Rabbit is granted credits manually — no Stripe subscription, so `#plg-churn-prod` will never fire for it; churn there is visible only as usage decay. Agilitas, despite the retainer, shows as Business seats with `subscriptionStatus` in PostHog.
- **Output events by surface:** Spaces → `space_execution_created`, `space_generation_completed`, `space_published`, `space_result_downloaded`; Canvas → `canvas_workflow_run_started`; Creative Director → `creative_director_studio_generation_completed`; Cowork/agents → `cowork_message_completed`, `content_published`; Routines → `routine_created`, `gavin_routine_enabled`. "Health" means output on *any* surface — a Spaces-only gate misreads Cowork-heavy users (patchandbagel).
- **Search vs. execution:** `space-search` (hyphen) is the search event; `space_execution_created` is the run. Ratio per §4.1.
- **Other projects in the org** (ShopOS Pro Dev 230727, Stg 230731, Amazon Copilot ×3) hold internal test data. The existing "ShopOS Growth Dashboard" lives in Dev.
- **Shobhit's "PLG triage automation"** (Claude + PostHog) posts churn breakdowns in Slack after a Stripe cancel alert. It missed Eustress's March–July history (identity split). Coordinate before duplicating.
- **Slack channels:** `#plg-sign-ups-prod` (signups), `#plg-plan-updates-prod` (purchases, upgrades, payment failures), `#plg-churn-prod` (cancellations). Stripe Alerts app posts to these.

---

## 7. People & sources — *agents only*

| Who / what | Role in this work |
|---|---|
| Ajay (Co-founder) | Kicked this off (Slack, Sep 2026); wants a WBR PLG update; hypothesis: "we're not in touch with our paid users" |
| Lobster / Harsh (product design) | Owner of this workspace; spoke to Sharath (PointTaken) on 2026-09-07 |
| Hemanth | Customer-facing on PLG accounts — calls, sample generations, follow-up on payment failures (Eustress) |
| Shobhit | Runs the PLG triage automation; author of the Eustress breakdown format this workspace adopts |
| Manish Mishra, Vedant Vaibhav | Tagged by Ajay on the Eustress thread; Manish is PointTaken's engineering contact for bugs |
| Nambi, Madhu Madhur, Prashant | Named by Sharath as ShopOS people he has worked with on Spaces / Richard |
| "PLG — Paying Customers (as of Sep 11)" | Slack list of paying accounts and plans; the roster's plan column comes from it |
| PointTaken call, 2026-09-07 | Amie transcript (PDF) + Fathom summary; both in Lobster's possession |
| PointTaken call, 2026-09-17 | Feed prototype + Gavin walkthrough; Gemini notes & transcript at `interviews/point-taken/pointtaken-2026-09-17-transcript.md` |
| Sidharth call, 2026-09-16 | Pulse check + feed walkthrough; Gemini notes & transcript at `interviews/sidharth/2026-09-16-shopos-sidharth-pulse-check.md` |
| Sidharth Monica deep dive, 2026-09-17 | Unsolicited written product audit emailed to Ajay; saved at `interviews/sidharth/2026-09-17-sidharth-monica-deep-dive.md` |
| Eustress thread, Sep 9–13 | Stripe alert → Ajay → Hemanth → Shobhit's breakdown → Ajay's hypothesis |

---

## 8. How this workspace gets built — the review loop

Lobster is the reviewer here, not the PostHog operator — that division is deliberate. Ajay's ask was a product-fit read on each customer, not a data-analyst skill set, and the operating model reflects that:

1. **Agent gives a read** on the customer: tag, one-line status, and the 1–2 things that actually matter — each with a confidence tag ([Certain]/[Likely]/[Guessing]).
2. **Lobster asks "back it up"** on whatever seems off or important — not on every claim, just the ones worth doubting.
3. **Agent gives the PostHog steps in plain UI terms** — nav path, filter, the number to expect — never SQL or raw event-schema jargon as the primary explanation.
4. **Lobster verifies it in the PostHog UI.** Match → move on. Mismatch → that's a real finding (about the read or the data), fix whichever is wrong before it goes in the file.
5. **The output per customer stays short:** tag, status line, and conclusions each classified as **design issue** (route to design/eng), **glitch/technical** (route to eng), or **discovery question** (goes in `questions.md` or the customer's Open Questions). A customer write-up with verified stats and no product conclusion is a miss — the data work is only ever in service of a design read, never the deliverable itself.

Underneath step 1, the agent still does the legwork properly before handing over a read — resolving identity (domain → workspace → plan), separating chat/interactive usage from monitoring/routine usage per seat (an agent run mostly through routines can look unused if you only count chat), and checking friction (`out_of_credits`, failures, rageclicks, abandoned surfaces) rather than raw volume alone. That discipline is internal to producing a correct read; it is not a checklist Lobster runs.

One thing worth remembering when a customer goes quiet: an account with no Stripe subscription (manually-granted credits) will never trip `#plg-churn-prod` no matter how quiet it goes — check billing shape before calling silence "stopped-forgotten" instead of "unmonitored."

## 9. Changelog — *agents only*

- **2026-09-20 (later)** — Full PostHog re-verification pass across all 10 files. Material corrections: **PointTaken** usage table re-measured now that the pointtaken.in filter works — Creative Director was recorded as 37/85/2 generations, the truth is 8 prompts and **zero completions on any seat**; Canvas 33/127 → 19/61 workflow runs; active days, searches, executions and out_of_credits all corrected. **R for Rabbit** — zero canvas runs Sep 13–20 and productteam silent since Sep 12; the decay signal that file was built to watch is firing. **patchandbagel** — renewal question closed behaviourally (active 7 of 8 days post-renewal, still publishing). **Agilitas** — amit ran 173 generations in a week with zero `out_of_credits`, first clean week on record. **Dawn** — returned Sep 16–17, cadence intact. **Imran** — last seen Sep 16, still zero output. **Sidharth** — Fashnstack founder status and his unsolicited Monica audit added. §4.1 narrowed with a counter-example (Sunny: 1,005/96 searches-to-executions *and* 1,931 completions). No changes needed for Patricia (updated earlier same day), Zeppelin or Eustress.
- **2026-09-20** — Folded in two feed-prototype calls. `pointtaken.md`: new Feed concept feedback section (Sep 17), Gavin data-discrepancy and credit-pooling blockers, design pickups 6–8, rewritten Next action. `sidharth-suresh.md`: first-contact call (Sep 16) written up incl. his feed feedback; usage re-verified in PostHog and corrected (searches 73 → 91, completed generations 1 → 3 — Creative Director output had been missed; active days 43 → 48); post-call Sep 17 session added. `patricia-noble.md`: re-verified silent, flagged that her credit/subscription person properties are frozen at her last event and are not a live billing read. New patterns §4.8 (feed judged on output quality, n = 2, not settled) and §4.9 (nobody reaches out until the customer is gone, n = 4). Roster status lines updated for all three.
- **2026-09-13** — Workspace created. Master README, 9 live customer files, 1 churned file (Eustress). Identities resolved in PostHog Pro Prod. Seven cross-customer patterns drafted with evidence counts. Sources: Sep 11 paying list, Ajay's Slack ask, Eustress thread, PointTaken call transcript.
- **2026-09-14** — §8 rewritten: replaced the four-step operator checklist with the actual working loop (agent reads → Lobster spot-checks in the PostHog UI). Lobster reviews and verifies; does not run PostHog analysis directly. Identity/surface-split/friction discipline kept, but as internal method, not a step-by-step Lobster follows.
- **2026-09-14** — §1 sharpened: the workspace's core question restated as the two-part value/friction statement, replacing the older single-verdict framing.

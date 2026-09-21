# Patricia Noble

**Tag:** `stopped-forgotten`
**Status:** Highest-priced self-serve plan in the base ($199/mo Business). **Session recordings reviewed 2026-09-21 overturn the previous read of this account.** She was not a fast buyer who produced nothing: she exhausted her free-plan credits while working, upgraded to Business to continue, and produced real finished work — 5 deck/catalogue versions for her brand Habana Resortwear, confirmed in the event data. Further output shown on the recordings (campaign images, Diwali shots) is **not verifiable in events** — see Usage. She also tried to book a demo four days *before* signing up and the form returned a 502. Last seen 2026-07-23; reported to have renewed again 2026-09-20.

## Identity
| Email | Workspace | Why connected |
|---|---|---|
| patricia.noble.torres@gmail.com | `org_3GPvQoxzTtAdw8zfk6R5rNTFiDl` | Only identity; person row created 2026-07-07 (anonymous visit), identified 2026-07-12 |

## Who they are
Individual operator behind **Habana Resortwear** (referred to in-product as "Habana PC"), a resortwear brand. Dominican Republic, direct traffic, Business monthly (35,000 credits).

She onboarded by **connecting an Instagram URL, not a website** — corrected 2026-09-21; the earlier "brand URL scan, so she has a live site" note was wrong, and the Instagram-only source later caused the agent to pick up the Instagram logo as her brand logo. **She works in Spanish** — she explicitly specified Spanish when generating her client catalogue.

## Lifecycle (all times UTC)
- **2026-07-08 — requested a demo on `/contact-sales` and the form failed.** She filled in email, name and company, clicked "Request a Demo", and got "Webhook responded with status 404"; the network call actually returned a **502 Bad Gateway**. Session ended on the error. Her first-ever action on ShopOS was asking to speak to a human, and it never reached anyone.
- 2026-07-12 19:53 signup → 19:54 onboarding completed with brand URL scan → 19:57 upgrade button → 20:14 brand memory page → 20:37 checkout started → 20:41 pricing ×4, plan selected ×2 → **20:41 Business purchased** (48 min after signup)
- 2026-07-12 20:47 Creative Director landing → 3 prompts submitted → 21:30 chat "retry" clicked ×2
- 2026-07-12 → 07-13 (one long overnight session, on recording): onboarded Habana via Instagram URL → worked with the Creative Director agent ("Tere") on a social ad campaign → **exhausted her free-plan credits, which is what sent her to upgrade** (corrected 2026-09-21: the limit she hit was the free-tier allowance *before* purchase, not a mid-session wall on a paid plan — `out_of_credits` has never fired for her at any point, before or after the upgrade) → chat thread churn: 3 `chat_created` events in 8 minutes (20:48, 20:51, 20:56), consistent with the recording's account of losing a thread → she told the agent she was frustrated → re-uploaded assets and generated multiple campaign directions
- 2026-07-13 00:49 share created + link copied · 01:27 35 Cowork messages started, 30 completed
- **`[Unverified — zero events]` 2026-07-13 (later sessions):** the whole block below comes from recording summaries and has **no event footprint of any kind** — after 01:31:55 UTC on Jul 13 there are exactly 3 events on her account (onboarding ×2 and one space-search, all at 19:35), and **zero events on Jul 14 and Jul 15**. Do not treat as fact until the recordings' own timestamps are checked. Claimed: generated Diwali campaign lifestyle shots, reviewed batches in the Image Editor, saved assets to Brand Memory, then built a **13-slide client catalogue in Spanish** — generated successfully, but the in-app preview failed to load so she had to download it to check. Then refined it in Creative Studio: fixed slide 6, worked around a **PPTX-instead-of-PDF download**, caught the agent **using her Instagram logo as the brand logo** and uploaded the real one, and finished with a **fully branded PDF catalogue**
- **`[Unverified — zero events]` 2026-07-14** — claimed return visit to re-read the finished work. **No events at all were recorded on 2026-07-14.** Either the recording is mis-dated, the session never identified to her person record, or it did not reach PostHog.
- 2026-07-17 onboarding re-entered (6 starts) · 2026-07-23 last seen
- Renewal on record 2026-08-12 · 31,653 of 35,000 credits remaining on record
- 2026-09-20 renewal reported by Lobster (billing side; not visible in PostHog — see Health signal)

## Usage (lifetime)

**As recorded by events** — active days 4 · sessions 7 · pageviews 59 · Creative Director prompts 3, retry clicks 2 · Cowork 35 messages started / 30 completed, 15 tool executions, 3 agents invoked · Space generations 0, Canvas 0, Space searches 13, executions 0 · 1 share created · 26 dead clicks · 6 onboarding starts · `out_of_credits` **0, lifetime**.

**Her 15 Cowork tool executions, broken out (checked 2026-09-21):** 10 × `storeMemory` (skill) and **5 × `generateDeck` (generation, all `status: completed`)** — at 23:19:09, 01:00:03, 01:05:45, 01:14:51 and 01:31:37. That is 5 deck/catalogue versions, and it matches the recording's "five design revisions". `cowork_tool_executed` is the **only** event that maps Cowork work; `space_generation_completed` and `creative_director_studio_generation_completed` are both genuinely 0 for her, which is why this output was previously read as zero.

**Confirmed in events — what she produced**
- **5 deck/catalogue versions** (`generateDeck`, completed) — the 13-slide Spanish catalogue and its revisions
- 1 share created + link copied (00:49)
- 2 brand-memory writes via `storeMemory`

**Claimed on recordings, NOT verifiable in events**
- Multiple social ad campaign directions plus final image assets — no image-generation tool event exists in her data; no `generateImage`-type `tool_name` appears anywhere
- Diwali campaign lifestyle shots / Image Editor batch review — no events
- The in-app preview failure, the PPTX-instead-of-PDF download, the Instagram-logo-as-brand-logo bug — no events
- The Jul 14 review session — no events

**The honest split.** Her deck output was always in the data; the earlier "0 generations" read was a wrong-event-name error on our side, not an instrumentation gap. The image-side output is a genuine gap — nothing in the schema records it. And the Jul 13-evening / Jul 14 block is neither: it has no footprint at all, not even a pageview, which is a different and more worrying condition than missing completion events.

## Health signal
Nine weeks of silence after a four-day burst in which she did more finished work than most accounts in this base. Re-checked in PostHog on 2026-09-20: last event is still 2026-07-23 18:51 UTC, zero events since, no cancellation or downgrade event either.

**Her person properties are frozen, not current.** `hasSubscription: true`, `subscriptionStatus: active`, `planType: Business`, `totalCredits` 31,653, `remainingMonthlyCredits` 31,653, `renewalDate` 2026-08-12 — all written at her last event on Jul 23 and unchanged since, because person properties only update when an event fires. Do not read these as live.

This is the limit of what product analytics can say about her: an auto-renewal that involves no login leaves no trace here. The reported 2026-09-20 renewal is invisible in PostHog and has to be confirmed in Stripe. Treat PostHog silence as "no product activity", never as "no billing activity".

## Touchpoints
- **2026-07-08 — she initiated contact and ShopOS lost it.** Completed demo request on `/contact-sales`; endpoint returned 502 (surfaced to her as a 404 webhook error). No lead was created, so nobody knew she had asked.
- After that: nothing. No outreach after purchase, none after she went quiet, none after either renewal. The only human contact she ever attempted was the one the product dropped.

## Read
*Rewritten 2026-09-21 after reviewing the session recordings, then corrected again the same day after cross-checking every claim against the event log. Claims are tagged for whether the events back them.*

- `[Likely]` **She did not buy on a promise — she bought after exhausting the free plan.** She submitted a Creative Director prompt at 20:15:17 on the free tier, then selected a plan at 20:37 and purchased at 20:41. Corrected 2026-09-21: the earlier "hit a credit wall mid-session while producing" wording was wrong on two counts — the limit was the free-tier allowance *before* she paid, and `out_of_credits` has never fired on this account at any point. Still the healthier conversion shape than README §4.2, but the evidence is the free-plan sequence, not a paid-plan wall.
- `[Likely]` **She got what she came for, and left anyway.** 5 completed deck generations ending 01:31:37 on Jul 13, then effectively nothing. Downgraded from `[Certain]`: the "came back on Jul 14 to re-read it" part has zero event backing, so the shape holds but that detail does not. Still reads as a retention failure rather than an activation failure.
- `[Certain]` **Her first contact with ShopOS was a demo request that 502'd**, four days before signup. She wanted a human at the start and the form ate it; she then paid $199/mo self-serve and still never heard from anyone.
- `[Guessing]` The bugs she hit — chat deleted mid-session, in-app preview failing to load, PPTX served when PDF was requested, Instagram logo taken as brand logo — come from recording summaries only. Downgraded from `[Certain]` on 2026-09-21: **no event in this project records any of them**, and three of the four sit inside the Jul 13-evening window that has no events at all. Worth routing to eng as leads, not as confirmed defects.
- `[Guessing]` The chat deletion is the most damaging of those. **Structurally untestable**: no event type anywhere in this project records a chat being deleted (`brand_memory_deleted`, `draft_workflow_deleted` and `overlay_template_deleted` exist; no chat equivalent). What events do show: 3 `chat_created` events inside 8 minutes (20:48:03, 20:51:10, 20:56:04) — thread churn consistent with the story, but at the *start* of the night, not at the 01:25:52 timestamp cited in the recording. One generic `api_call` is logged at exactly 01:25:52.121 with no payload detail.
- `[Likely]` Re-entering onboarding six times on Jul 17 was her looking for a way to start the *next* project and not finding one — not failing to start the first.
- `[Certain]` She works in Spanish. Upgraded from `[Guessing]`: she specified Spanish for the catalogue output.

## Open questions
**To check in data**
- ~~Session replays~~ — done 2026-09-21; five recordings summarised in `interviews/patricia/2026-07-session-recordings.md`.
- ~~Reconcile the credit-wall timing.~~ — resolved 2026-09-21: she exhausted the **free-plan** allowance and upgraded off the back of it. `out_of_credits` has never fired on this account, so free-tier exhaustion evidently does not emit that event. **Follow-up: does `out_of_credits` fire for free-plan users at all?** If not, every free-tier credit wall in this workspace is invisible.
- **Is the `/contact-sales` demo endpoint still returning 502?** Test it. If it is, every enterprise lead since July has been silently dropped — this is far bigger than one customer.
- **Re-run every "0 generations" read in this workspace against `cowork_tool_executed`, not just the `*_generation_completed` events.** Hers was wrong for exactly this reason: 5 completed `generateDeck` calls sat in the data the whole time. This is a workspace-wide re-check, not a Patricia item.
- **Why does the Jul 13-evening / Jul 14 window have zero events of any kind** — not even `$pageview` — when the recordings show activity? Three candidates: recordings mis-dated, session never identified to her person record, or events not reaching PostHog. If it is the third, it affects every file here.
- Is image generation instrumented anywhere? No `generateImage`-type `tool_name` appears in her data or in the sampled property values for `cowork_tool_executed`.
- **Confirm the 2026-09-20 renewal in Stripe** and how many cycles she has now paid for with zero output (Jul 12 purchase, then Aug and Sep renewals = up to ~$600 for 3 completed generations of nothing).
- Does any renewal or invoice event reach PostHog for *any* customer, or is billing entirely invisible here? This affects every file in this workspace, not just hers.

**To ask (email; a call is unlikely)**
- What were you trying to create on your first day?
- What would have needed to happen for you to come back?

## Next action
She is still the strongest case in the base for a customer who converted for the right reason and got dropped — but the email needs to reference only what we can stand behind.

1. **Test `/contact-sales` today.** If the demo endpoint is still 502ing, that is a revenue leak affecting everyone, not a note in one customer file. Route to eng with the Jul 8 recording attached.
2. **Resolve the Jul 13-evening / Jul 14 blackout before anything else in this file is trusted.** Pull the recordings' own timestamps and session IDs and check them against the event log. If sessions are genuinely not reaching PostHog, that outranks every other item here.
3. **Email her in Spanish, from a person, referencing the Habana catalogue by name** — she built it, we can prove it (5 versions), and ask what she needed next that she didn't get. Do **not** apologise for the deleted chat in writing until item 2 confirms it happened.
4. Confirm the Sep 20 renewal in Stripe and decide deliberately whether to keep billing her while that email is outstanding.
5. Route the four bugs to eng as **leads, not confirmed defects** — none of them has event backing.

## Changelog
- 2026-09-21 (3) — **Cross-checked every recording-derived claim against the event log; corrected three and downgraded four.** (a) The "hit a credit wall mid-session" story was wrong: she exhausted the **free plan** and upgraded off that; `out_of_credits` has never fired on this account. (b) The "0 generations" read was **our error, not an instrumentation gap** — `cowork_tool_executed` shows 5 completed `generateDeck` calls (23:19:09, 01:00:03, 01:05:45, 01:14:51, 01:31:37), matching the recording's five revisions; we had only checked `space_generation_completed` and `creative_director_studio_generation_completed`. (c) The entire Jul 13-evening and Jul 14 narrative has **zero events of any kind** — 3 events total after 01:31:55 on Jul 13, none at all on Jul 14 or 15 — so it is now tagged `[Unverified]` throughout rather than stated as fact. (d) The chat-deletion claim is structurally untestable: no chat-deletion event type exists in this project; 3 `chat_created` events cluster at 20:48–20:56, not at the cited 01:25:52, where only a bare `api_call` is logged. Read claims downgraded accordingly.
- 2026-09-21 (2) — Confirmed via `execute-sql`: zero events for her in the last 30 days and in the last 60 days (only the Jul 23 pageview). Checked `subscription_purchase_completed` specifically: fired once, at her original Jul 12 purchase, never on the Aug or reported Sep renewal — so renewal charges don't appear to emit any PostHog event at all, for her specifically. Documented in Health signal and Open questions.
- 2026-09-21 — **Major correction from session recordings** (five July recordings, summarised in `interviews/patricia/2026-07-session-recordings.md`). She produced substantial finished work — campaign assets, Diwali shots, a 13-slide Spanish catalogue, a branded PDF catalogue — none of which the event counters captured; "0 generations" is an instrumentation artefact. Her upgrade was triggered by a credit wall mid-work, not bought on promise. Added the 2026-07-08 demo-request 502 (her first-ever action, dropped by us), the mid-session chat deletion, and three other output-path bugs. Brand identified as Habana Resortwear; onboarding was via Instagram URL, not a website; she works in Spanish. Status, Who they are, Lifecycle, Usage, Touchpoints, Read, Open questions and Next action all rewritten.
- 2026-09-20 — Re-verified in PostHog: no activity since 2026-07-23, no cancellation event. Documented that her credit/subscription person properties are frozen at the Jul 23 snapshot and are not a live billing read. Added the reported 2026-09-20 renewal and rewrote Next action around confirming it in Stripe.
- 2026-09-13 — File created from PostHog (Pro Prod) + Sep 11 paying list.

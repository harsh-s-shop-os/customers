# PointTaken (Sharath Ravishankar)

**Tag:** `deriving-real-value`
**Status:** Agency running client work on ShopOS daily; three seats; the closest thing ShopOS has to a design partner. Blocked from going further by Richard's context loss and credit cost. As of the 2026-09-17 feed call, a second and harder blocker is on the table: Gavin returned contradictory numbers for the same window in the same chat, and Sharath says he can no longer trust agent-reported data.

## Identity
| Email | Workspace | Why connected |
|---|---|---|
| sharath@pointtaken.in | `org_3ARZgG06CT7r1ZHs8ivf2akPaav` | Primary; plan "PointTaken - Sharath"; the person Lobster spoke to |
| pratik@pointtaken.in | same workspace | Colleague; works on Skills (per Sharath) |
| sunny@pointtaken.in | `org_3ARbJTjxKMQFhqLf08IAd1hAfxU` | Colleague; separate workspace; does the image/Spaces production Sharath handed off; made a `subscription_purchase_completed` on 2026-07-06 |
| promotions@vbexports.co.in | none recorded | On the same "PointTaken - Sharath" plan, active Apr 7 – Jul 15 2026; `[Likely]` a PointTaken client given a seat |

Each email also has an older person row without a workspace (Dec 2025 – Mar 2026). Aggregate by email.

## Who they are
Marketing/e-commerce agency (India). Sharath runs performance marketing, SEO and QA; clients include an Indian ethnic-wear brand now pivoting to Indo-Western fusion. Sharath has a game-development background (Unreal Engine), which is why he likes the node-based Spaces UI. Arrived Dec 2025, before self-serve purchase events were instrumented; the custom plan was hand-negotiated.

## Lifecycle
- 2025-12-24 Pratik first seen · 2025-12-29 Sharath first seen · 2026-03-06 Sunny first seen
- Custom plan "PointTaken - Sharath" (50,000 credits/mo per Sep 11 list); renewal on record 2026-09-19
- Continuous activity through 2026-09-20 (Sunny last seen Sep 20, Sharath and Pratik Sep 19) — all three seats active in the week after the Sep 17 call
- No `subscription_purchase_completed` event around the 2026-09-19 renewal date; custom plans appear not to emit one, so renewal must be confirmed on the billing side

## Usage (lifetime, re-verified 2026-09-20)
| | Sharath | Sunny | Pratik |
|---|---|---|---|
| Active days | 216 | 146 | 127 |
| Space generations completed / failed | 1,010 / 27 | 1,931 / 165 | 1 / 0 |
| Space searches / executions created | 412 / 62 | 1,005 / 96 | 622 / 40 |
| Canvas workflow runs (`canvas_workflow_run_started`) | 19 | 61 | 0 |
| Canvas node runs (`canvas_node_run_started`) | 39 | 255 | 0 |
| Creative Director prompts submitted / completions | 4 / 0 | 4 / 0 | 0 / 0 |
| Routines created | 3 | 0 | 0 |
| Connectors connected | 3 | 0 | 0 |
| Invites sent | 5 | 2 | 0 |
| `out_of_credits` | 5 | 2 | 0 |
| Pricing page views / upgrade clicks | 15 / 14 | 10 / 4 | 1 / 1 |
| Last seen | 2026-09-19 | 2026-09-20 | 2026-09-19 |

**Correction (2026-09-20):** the pointtaken.in filter now works in PostHog, so these are measured rather than carried over. Two rows were materially wrong. Creative Director was recorded as 37 / 85 / 2 generations — the real figure is 4 prompts submitted by Sharath, 4 by Sunny, **zero completions on any seat**, plus 2 retry clicks. Nobody at PointTaken has ever finished a Creative Director generation. Canvas was also overstated (33 / 127); the verified `canvas_workflow_run_started` counts are 19 / 61, with node-level runs listed separately.

Sharath's own time split (stated 2026-09-07): Gavin 30–40%, Richard ~50%, BigHead 10–15%, Monica ~5%. Image work is Sunny's.

## Health signal
Healthy and stable: 210 active days, output on every surface, routines running daily. Two risks: (1) credit pressure — 4 `out_of_credits`, and he shut off "Jobs" when they leaked ~2k credits per run; (2) Richard is "fairly broken" for him (context loss), which blocks every SEO routine and the multi-agent workflow he actually wants.

## What works / what doesn't (plain read for design handoff)
*See "Read" below for the sourced, tagged version this summarizes.*

**What works**
- Richard — most-talked-to agent, 391 of 454 chat messages.
- Big Head — heavy real backend work: 258 Shopify edits, 26 GEO content pieces, mostly unattended.
- Gavin — heavy real backend work: 130 Meta ads calls, trusted to run without supervision.
- Image generation (Spaces) — heavy daily use, 1,010 completions for Sharath and 1,931 for Sunny.
- Team adoption — 3 people, real division of labor, daily habit, not a trial.

**What's not working**
- Richard breaks under automation — a batch job was killed after burning ~2k credits per run.
- Orchestrator loses context on the way to Richard — no direct entry point like Gavin has.
- Publishing is fully manual — Spaces -> Canva -> Shopify, five hand steps.
- Monica loses context even with brand memory on — handed off to a colleague instead of fixed.
- Credit fear caps experimentation — features get shut off rather than risked.
- Agent-reported numbers contradict themselves — Gavin gave two different Meta/Shopify purchase counts and two different spend figures for the same 30-day window, inside one chat (2026-09-17).
- Credits cannot be pooled or shared across workspaces on a custom plan — blocks Pratik from onboarding the next two brands under one pool.

**For product design to pick up**
1. Give Richard a direct chat entry point, same pattern as Gavin's "Ask Gavin" — removes the Orchestrator detour for a known, high-use agent.
2. Design a lighter publish path from Spaces/Monica output straight to Shopify — collapse the 5 manual steps.
3. Audit Monica's brand-memory adherence — it's not holding brand consistency despite being on.
4. Show credit cost/risk before a job runs — right now users only learn a job is expensive after it breaks.
5. Make context-loss visible when it happens — right now a broken run just burns credits silently, no failure state shown.
6. Put the driving signal on the feed card itself — Pratik asked twice what generates a card and neither verbal answer satisfied him. "We scraped your URL" is not a signal.
7. Give the feed a persona dimension inside one workspace — founder, catalog manager and performance marketer should not share a feed. Pratik raised this unprompted; today it does not exist.
8. Show provenance on any number an agent reports — which source, which window, which pull. The Sep 17 discrepancy is a trust problem before it is a model problem.

## Feed concept feedback (2026-09-17 call)
*Prototype shown live by Harsh/Vedant to Sharath + Pratik. This is their read on the feed itself, separate from the product they use today.*

**Overall stance:** conditional buy-in, not enthusiasm. Pratik: "broadly happy… it's in the right direction." Neither took the demo at face value — both went straight to what generates the cards.

**Their core ask — signal transparency**
- What routines and signals actually produce each card. Pratik asked twice; the answer given on the call (scrape the URL, benchmark the category) was not concrete enough for him.
- Whether the feed is persona-specific inside one workspace — a founder, a catalog manager and a performance marketer should not see the same feed. Today it isn't.

**Credit model** — the one part that landed clean. Sharath asked whether surfacing a draft, dismissing it, or moving to the next one costs credits. Confirmed live: drafts are free, credits are deducted only on action. He accepted it and did not return to it.

**Cards they stress-tested**
- *CPM rising* — Pratik asked exactly what the card would show. Answer: a flagged delta, no root-cause dive, to keep credit cost down. He accepted it and clocked it as shallow.
- *Rotate creative* — Sharath walked through what should happen on click: separate fatigue-from-overexposure from fatigue-from-the-creative before proposing a replacement, then offer two or three options within the same SKU, a variant, or a different SKU. That is the stated intent; it is not built.
- *Catalog recommendations* — Pratik rejected SEO hygiene tags as the signal ("that's hygiene") and named landing-page → add-to-cart conversion as the real one. Logged live as a correction.

**v0 gaps they named in the feed itself**
- No custom or tunable prompts in the daily feed — told it may merge with Routines later.
- No SEO/keyword signals behind the visibility column — told nothing lands before end of October.

**Where it stands:** they are buying the idea and withholding judgment on the execution. Pratik and Sharath are sending five jobs-to-be-done for their feed. Until those land, nobody knows whether the feed produces decisions as good as the ones Pratik already makes by hand — and his own manual decision-making is the benchmark he stated.

## Touchpoints
- 2026-09-07 — First call with Lobster/Harsh (45 min; Amie transcript + Fathom summary). Agreed: Lobster shares feedback with design/eng; recurring catch-ups via Slack.
- 2026-09-17 — Second call, group (Harsh, Shobhit, Vedant, Adarsh, Manish + Sharath, Pratik; ~68 min, Gemini transcript in `interviews/point-taken/`). Two halves: feed prototype walkthrough, then Gavin/Meta ads questions where the data discrepancy surfaced. Follow-up session agreed with Shobhit and a developer.
- Ongoing — Sharath reports bugs directly to Manish (routine-instructions save bug, acknowledged, unfixed), and has worked with Nambi, Madhu Madhur and Prashant on Spaces/Richard. He says the agent UI has improved on his recommendations over 3–4 months.

## Read
- `[Certain]` Sharath is a self-described "extreme quality tester" who deliberately breaks workflows and reports them. His numbers include stress-testing; do not read PointTaken as a typical user.
- `[Certain]` His success criterion for a routine is *actionable recommendations* (his KTK method: Kill / Tweak / Keep). A routine that only summarises is a failed run to him.
- `[Certain]` Current publish workflow: Spaces → Canva (fix text/typography) → PNG → webp → manual Shopify upload. Five manual steps per asset.
- `[Certain]` The ask that would collapse those steps: a routine where Richard fetches SKUs → Monica builds desktop+mobile banners → Richard publishes to the Shopify theme. Impossible today because of Richard's context loss and Monica's off-brand output.
- `[Likely]` Credit anxiety, not feature gaps, is the main brake on him trying more. Orchestrator routing is a credit cost in his mental model.
- `[Likely]` The Richard UI asymmetry (Gavin has "Ask Gavin / recipes", Richard has no direct entry) is the *design* root of the orchestrator detour he complains about.
- `[Certain]` (2026-09-17) He no longer trusts agent-reported figures. He screen-shared one Gavin chat returning Meta 53 / Shopify 42 purchases in one view and Shopify 57 / Meta 39 in another, plus spend of 7,700 against 12,800 — same brand, same 30-day window, same chat. Adarsh's working theory is the model fetching partial data across paginated pulls (Claude Sonnet 4.6 on auto mode); unconfirmed.
- `[Certain]` (2026-09-17) Pratik's benchmark for the feed is his own manual decision-making, not a competitor product. He described pulling a top-20%-of-revenue SKU report that morning and acting on variant-level detail, then asked how the feed would have produced that same decision.
- `[Certain]` (2026-09-17) Pratik is onboarding two more brands (an ethnic-wear and a menswear label) over the next four to five weeks, and expects the feed's day-zero value to carry them. Credit pooling across workspaces is what blocks that today.
- `[Likely]` The feed does not route around either of their existing problems. It moves the question from "can I trust this agent's output" to "can I trust this card" — the same trust gate, relocated. Both of them tested it that way on the call rather than reacting to the UI.
- `[Certain]` Creative Director is unused here — 8 prompts between them, zero completions, 2 retries. An agency producing 2,900+ Space generations has never once finished a CD generation. Either it does not fit their workflow or it fails them early; nobody has asked which.
- `[Guessing]` Pratik, not Sharath, is the economic buyer for the feed. He drove the signal and roadmap questions; Sharath drove the mechanics. Worth confirming before the next session.

## Open questions
**To check in data**
- Which agent/surface consumes most of the 50k credits per month? (Needs billing-side credit ledger; PostHog has no consumption event.)
- What are Sunny's 165 space generation failures — model errors or user cancellations?
- Is promotions@vbexports.co.in still active, and is it a client seat?
- Did the custom plan renew on 2026-09-19? No purchase event fired; confirm on the billing side.
- Why has no PointTaken seat ever completed a Creative Director generation despite 8 prompt submissions and 2 retry clicks? Check the retry events and any failure states.
- The Sep 17 Gavin discrepancy: pull the reasoning logs for that chat and confirm whether sub-agents returned partial rows (Adarsh owns this; Sharath to share the chat link and date range).

**To ask on the next call**
- To Sunny, not Sharath: image quality and brand-memory adherence for the ethnic/Indo-Western catalogue.
- Which specific Richard task loses context first — SKU fetch, meta write, or publish?
- Would he pay more for a plan without orchestrator overhead, or does he expect it to be free?
- Has anything shipped since Sep 7 (agent-targeting in Routines, node-connection deletion) changed his workflow?
- Have the five jobs-to-be-done arrived, and do they map to signals v0 can actually produce?
- Is Pratik or Sharath the decision-maker on whether PointTaken keeps expanding on ShopOS?
- After the data discrepancy: what would it take to restore his confidence in a reported number — provenance on the card, a re-run, a manual cross-check he can trigger?

## Next action
Three open commitments from Sep 17, in priority order:
1. **Credit pooling across workspaces on custom plans** — Harsh committed to a same-day fix and a WhatsApp update. This is the one that blocks Pratik onboarding two brands; check whether it shipped.
2. **The Gavin data discrepancy** — Adarsh to review sub-agent reasoning logs and report back. Until this is answered, every other feature conversation with this account is downstream of a trust problem.
3. **Chase the five jobs-to-be-done** from Pratik and Sharath, and confirm each maps to a signal v0 can produce. Without them the feed ships to this account untailored.

Still outstanding from Sep 7: the recurring Slack catch-up, and the three design/eng items with his name on them (agent-targeting dropdown in Routines; delete-connection affordance in Spaces canvas; routine-instructions field not persisting).

## Changelog
- 2026-09-13 — File created from PostHog (Pro Prod) + 2026-09-07 call transcript + Sep 11 paying list.
- 2026-09-20 (later) — Usage table re-verified against PostHog now that the pointtaken.in filter works. Corrected: active days 210/141/124 → 216/146/127; Space generations 1,008 → 1,010 and 1,901 → 1,931; searches/executions filled in for all three seats; Canvas 33/127 → 19/61 workflow runs (node runs listed separately); **Creative Director 37/85/2 → 4/4/0 prompts with zero completions on any seat**; routines 5 → 3; out_of_credits 4/0 → 5/2. Added last-seen row and a correction note.
- 2026-09-20 — Added the 2026-09-17 feed call: new "Feed concept feedback" section, two What's-not-working items (Gavin data discrepancy, credit pooling), design pickups 6–8, four Read claims, new open questions, rewritten Next action. Transcript at `interviews/point-taken/pointtaken-2026-09-17-transcript.md`. Usage figures above still date from 2026-09-13 and were not re-verified.
- 2026-09-14 — Added plain what-works/not-working/design-pickup summary above, drafted 2026-09-13. PostHog still cannot read any pointtaken.in-filtered data as of this session (broad queries return data, filtered queries return zero rows, same failure signature as yesterday) — figures here carry over from data verified earlier in the previous session, not re-verified today.

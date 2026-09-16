# PointTaken (Sharath Ravishankar)

**Tag:** `deriving-real-value`
**Status:** Agency running client work on ShopOS daily; three seats; the closest thing ShopOS has to a design partner. Blocked from going further by Richard's context loss and credit cost.

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
- Continuous activity through 2026-09-13 (Sharath last seen Sep 13, Sunny Sep 11, Pratik Sep 13)

## Usage (lifetime to 2026-09-13)
| | Sharath | Sunny | Pratik |
|---|---|---|---|
| Active days | 210 | 141 | 124 |
| Space generations completed / failed | 1,008 / 27 | 1,901 / 165 | 1 / 0 |
| Space searches / executions | 327 / 60 | — | — |
| Canvas workflow runs | 33 | 127 | 0 |
| Creative Director generations | 37 | 85 | 2 |
| Routines created | 5 | 0 | 0 |
| Connectors connected | 3 | 0 | 0 |
| Invites sent | 4 | 2 | 0 |
| `out_of_credits` | 4 | 0 | 0 |
| Pricing page views / upgrade clicks | 15 / 14 | 10 / 4 | 1 / 1 |

Sharath's own time split (stated 2026-09-07): Gavin 30–40%, Richard ~50%, BigHead 10–15%, Monica ~5%. Image work is Sunny's.

## Health signal
Healthy and stable: 210 active days, output on every surface, routines running daily. Two risks: (1) credit pressure — 4 `out_of_credits`, and he shut off "Jobs" when they leaked ~2k credits per run; (2) Richard is "fairly broken" for him (context loss), which blocks every SEO routine and the multi-agent workflow he actually wants.

## What works / what doesn't (plain read for design handoff)
*See "Read" below for the sourced, tagged version this summarizes.*

**What works**
- Richard — most-talked-to agent, 391 of 454 chat messages.
- Big Head — heavy real backend work: 258 Shopify edits, 26 GEO content pieces, mostly unattended.
- Gavin — heavy real backend work: 130 Meta ads calls, trusted to run without supervision.
- Image generation (Spaces) — heavy daily use, 1,000-1,900 completions per seat.
- Team adoption — 3 people, real division of labor, daily habit, not a trial.

**What's not working**
- Richard breaks under automation — a batch job was killed after burning ~2k credits per run.
- Orchestrator loses context on the way to Richard — no direct entry point like Gavin has.
- Publishing is fully manual — Spaces -> Canva -> Shopify, five hand steps.
- Monica loses context even with brand memory on — handed off to a colleague instead of fixed.
- Credit fear caps experimentation — features get shut off rather than risked.

**For product design to pick up**
1. Give Richard a direct chat entry point, same pattern as Gavin's "Ask Gavin" — removes the Orchestrator detour for a known, high-use agent.
2. Design a lighter publish path from Spaces/Monica output straight to Shopify — collapse the 5 manual steps.
3. Audit Monica's brand-memory adherence — it's not holding brand consistency despite being on.
4. Show credit cost/risk before a job runs — right now users only learn a job is expensive after it breaks.
5. Make context-loss visible when it happens — right now a broken run just burns credits silently, no failure state shown.

## Touchpoints
- 2026-09-07 — Call with Lobster/Harsh (45 min; Amie transcript + Fathom summary). Agreed: Lobster shares feedback with design/eng; recurring catch-ups via Slack.
- Ongoing — Sharath reports bugs directly to Manish (routine-instructions save bug, acknowledged, unfixed), and has worked with Nambi, Madhu Madhur and Prashant on Spaces/Richard. He says the agent UI has improved on his recommendations over 3–4 months.

## Read
- `[Certain]` Sharath is a self-described "extreme quality tester" who deliberately breaks workflows and reports them. His numbers include stress-testing; do not read PointTaken as a typical user.
- `[Certain]` His success criterion for a routine is *actionable recommendations* (his KTK method: Kill / Tweak / Keep). A routine that only summarises is a failed run to him.
- `[Certain]` Current publish workflow: Spaces → Canva (fix text/typography) → PNG → webp → manual Shopify upload. Five manual steps per asset.
- `[Certain]` The ask that would collapse those steps: a routine where Richard fetches SKUs → Monica builds desktop+mobile banners → Richard publishes to the Shopify theme. Impossible today because of Richard's context loss and Monica's off-brand output.
- `[Likely]` Credit anxiety, not feature gaps, is the main brake on him trying more. Orchestrator routing is a credit cost in his mental model.
- `[Likely]` The Richard UI asymmetry (Gavin has "Ask Gavin / recipes", Richard has no direct entry) is the *design* root of the orchestrator detour he complains about.

## Open questions
**To check in data**
- Which agent/surface consumes most of the 50k credits per month? (Needs billing-side credit ledger; PostHog has no consumption event.)
- What are Sunny's 165 space generation failures — model errors or user cancellations?
- Is promotions@vbexports.co.in still active, and is it a client seat?

**To ask on the next call**
- To Sunny, not Sharath: image quality and brand-memory adherence for the ethnic/Indo-Western catalogue.
- Which specific Richard task loses context first — SKU fetch, meta write, or publish?
- Would he pay more for a plan without orchestrator overhead, or does he expect it to be free?
- Has anything shipped since Sep 7 (agent-targeting in Routines, node-connection deletion) changed his workflow?

## Next action
Set up the recurring Slack catch-up Sharath offered, and route three items to design/eng with his name on them: optional agent-targeting dropdown in Routines; delete-connection affordance in Spaces canvas; routine-instructions field not persisting.

## Changelog
- 2026-09-13 — File created from PostHog (Pro Prod) + 2026-09-07 call transcript + Sep 11 paying list.
- 2026-09-14 — Added plain what-works/not-working/design-pickup summary above, drafted 2026-09-13. PostHog still cannot read any pointtaken.in-filtered data as of this session (broad queries return data, filtered queries return zero rows, same failure signature as yesterday) — figures here carry over from data verified earlier in the previous session, not re-verified today.

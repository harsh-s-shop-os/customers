# Patricia Noble

**Tag:** `stopped-forgotten`
**Status:** Highest-priced self-serve plan in the base ($199/mo Business). Bought 48 minutes after signup, tried across three sessions in her first eleven days, and has not been seen since 2026-07-23. Zero completed generations. Re-verified 2026-09-20: still nothing. Reported to have renewed on 2026-09-20 — nine weeks silent, paying $199/mo for zero output.

## Identity
| Email | Workspace | Why connected |
|---|---|---|
| patricia.noble.torres@gmail.com | `org_3GPvQoxzTtAdw8zfk6R5rNTFiDl` | Only identity; person row created 2026-07-07 (anonymous visit), identified 2026-07-12 |

## Who they are
Individual, Dominican Republic, direct traffic. Ran a brand-memory URL scan at onboarding, so she has a live site. Business monthly: 35,000 credits.

## Lifecycle (all times UTC)
- 2026-07-12 19:53 signup → 19:54 onboarding completed with brand URL scan → 19:57 upgrade button → 20:14 brand memory page → 20:37 checkout started → 20:41 pricing ×4, plan selected ×2 → **20:41 Business purchased** (48 min after signup)
- 2026-07-12 20:47 Creative Director landing → 3 prompts submitted → 21:30 chat "retry" clicked ×2
- 2026-07-13 00:49 share created + link copied · 01:27 35 Cowork messages started, 30 completed
- 2026-07-17 onboarding re-entered (6 starts) · 2026-07-23 last seen
- Renewal on record 2026-08-12 · 31,653 of 35,000 credits remaining on record
- 2026-09-20 renewal reported by Lobster (billing side; not visible in PostHog — see Health signal)

## Usage (lifetime)
- Active days 4 · Sessions 7 · Pageviews 59
- Creative Director prompts 3 · Generations completed **0** · Retry clicks 2
- Cowork messages 35 started / 30 completed · Tool executions 15 · Agents invoked 3
- Space generations 0 · Canvas 0 · Space searches 13 · Executions 0
- Share created 1 · Dead clicks 26 · Onboarding starts 6 (re-entered after completing)

## Health signal
Nine weeks of silence after a four-day burst. Re-checked in PostHog on 2026-09-20: last event is still 2026-07-23 18:51 UTC, zero events since, no cancellation or downgrade event either.

**Her person properties are frozen, not current.** `hasSubscription: true`, `subscriptionStatus: active`, `planType: Business`, `totalCredits` 31,653, `remainingMonthlyCredits` 31,653, `renewalDate` 2026-08-12 — all written at her last event on Jul 23 and unchanged since, because person properties only update when an event fires. Do not read these as live.

This is the limit of what product analytics can say about her: an auto-renewal that involves no login leaves no trace here. The reported 2026-09-20 renewal is invisible in PostHog and has to be confirmed in Stripe. Treat PostHog silence as "no product activity", never as "no billing activity".

## Touchpoints
None recorded. No outreach after purchase, none after she went quiet.

## Read
- `[Certain]` She bought on promise: purchase preceded any completed output.
- `[Certain]` She tried — 3 CD prompts, 35 Cowork messages, a share link — and 2 retries + 26 dead clicks say the product did not respond the way she expected.
- `[Likely]` Re-entering onboarding six times on Jul 17 means she came back looking for a way in and didn't find one.
- `[Likely]` Whatever she wanted to make on Jul 12–13 did not get made. That is the churn reason, not price.
- `[Guessing]` Spanish-speaking market; language may be a factor in the dead clicks and retries.

## Open questions
**To check in data**
- Session replays for 2026-07-12 20:47–21:30 and 2026-07-13 00:49–01:32: what did she ask Creative Director and Cowork for, and what came back?
- **Confirm the 2026-09-20 renewal in Stripe** and how many cycles she has now paid for with zero output (Jul 12 purchase, then Aug and Sep renewals = up to ~$600 for 3 completed generations of nothing).
- Does any renewal or invoice event reach PostHog for *any* customer, or is billing entirely invisible here? This affects every file in this workspace, not just hers.

**To ask (email; a call is unlikely)**
- What were you trying to create on your first day?
- What would have needed to happen for you to come back?

## Next action
She has now renewed at least once while completely silent, so this is no longer a "watch and see" account — it is an active refund/goodwill risk and the clearest single case of the product failing to carry someone who paid in good faith.

1. Confirm the renewal in Stripe.
2. Watch the two session replays (2026-07-12 20:47–21:30, 2026-07-13 00:49–01:32). The 2 retries and 26 dead clicks are in there.
3. Send one plain email from a person — not a nudge, not a campaign — asking what she was trying to make on her first day. If she doesn't reply, decide deliberately whether to keep billing her.

## Changelog
- 2026-09-20 — Re-verified in PostHog: no activity since 2026-07-23, no cancellation event. Documented that her credit/subscription person properties are frozen at the Jul 23 snapshot and are not a live billing read. Added the reported 2026-09-20 renewal and rewrote Next action around confirming it in Stripe.
- 2026-09-13 — File created from PostHog (Pro Prod) + Sep 11 paying list.

# Agilitas

**Tag:** `deriving-real-value`
**Status:** The heaviest user in the base by a wide margin — 20+ seats since November 2025 across three workspaces. The Sep 11 list's "NEW Sep 10, $199/mo retainer" describes at most a new add-on; it does not describe this account.

## Identity
Three workspaces:
| Workspace | Key |
|---|---|
| Agilitas | `org_3E4dgNsvPyADWlA25Yz0fxHrp1W` |
| Agilitas - Lotto | `org_3BJN6h4va2zaxsquexTxwSbvhSC` |
| Agilitas - One8 | `org_3BJNBB1AG9uxYqGKK5oeGTfHZlw` |

Seats seen (`@agilitas.in` unless noted), grouped by activity:
- **Heavy, current:** naresh.oblesh (Business, active), amit.bhandari (Business, active), nayantara.parikh (Business, past_due on one row), ananya.srivastava (Business, active), mashood.mubarak (Business, active, joined Jul 15)
- **Moderate / earlier:** geethika.nair (Custom Growth Plan, renewal 2027-03-28; last seen Jun 2), richa@agilitas.in (Custom Growth Plan; also richa@agilitas.com, Business, Aug 17), ambar.dange, uzair.jamshed, kartik.dogra, saurabh.bhandari, trushit.patel (Lotto workspace), vivek.chethan
- **Dormant since Q1 2026:** radhika.bagri, divya.unni, lottocatalog@, nikhil.chauhan, anirudh.singh, shaibal.mitra, nikita.goel, abhishek.singh, anant.jethalia, tanisha.modi, adithya.krishnan

Most seats have two person rows (with and without workspace). Aggregate by email.

## Who they are
Agilitas Sports — Indian sportswear group (Lotto and One8 licences are the two sub-workspaces). Enterprise-scale usage on a mix of Business monthly seats (32,500 credits each on record) and a "Custom Growth Plan" with renewal March 2027. Relationship predates PLG instrumentation.

## Lifecycle
- 2025-11-14 first seats (ananya, saurabh) · steady seat additions through Mar 2026
- 2026-03-04 / 03-14 Custom Growth Plan rows appear (geethika, richa)
- 2026-08-03 nayantara `subscription_purchase_completed` · 2026-08-25 nayantara `topup_purchase_completed` (the only top-up in the whole base)
- 2026-09-10 "$199/mo retainer" per Sep 11 list · 2026-09-13 amit last seen

## Usage (lifetime to 2026-09-13, top seats)
| Seat | Active days | Space gens | Canvas runs | Notable |
|---|---|---|---|---|
| naresh.oblesh | 167 | 1,577 | 0 | 6 downloads; 20 failed generations |
| amit.bhandari | 141 | 976 | 69 | **28 `out_of_credits`** |
| nayantara.parikh | 192 | 5 | 1 | 1 purchase, 1 top-up, 7 pricing views, 2 invites |
| ananya.srivastava | 108 | 8 | 2 | — |
| geethika.nair | 73 | 15 | 0 | last seen Jun 2 |
| richa | 33 (+1) | 62 (+3) | 1 | Custom plan |
| mashood.mubarak | 23 | 2 | 1 | onboarding completed |

## Health signal
Volume is not the risk. Credit friction is: Amit alone has hit `out_of_credits` 28 times — the plan attached to the heaviest seat is too small. Also watch seat consolidation: roughly half the seats have been dormant since Q1; the active core is ~5 people.

## Touchpoints
None recorded in this workspace. Nayantara appears to handle billing (purchase + top-up). Relationship owner at ShopOS unknown here.

## Read
- `[Certain]` This is an enterprise account being described in PLG terms. Ten months, 20+ seats, thousands of generations.
- `[Certain]` The only top-up purchase in the entire customer base came from this account, right after Amit's credit exhaustion streak — the pricing is under-provisioned for their production floor.
- `[Guessing]` The Sep 10 $199/mo is a sub-team or add-on (perhaps Lotto or One8), not the account.

## Open questions
**To check in data**
- Which workspace (main / Lotto / One8) does each active seat belong to, and which one is growing?
- When do Amit's `out_of_credits` events cluster — month-end, or after big batches?

**To ask**
- What exactly was signed on Sep 10, and how does it relate to the Custom Growth Plan renewing Mar 2027?
- Who is the champion — Naresh (volume) or Nayantara (billing)?
- Is the dormant half of the seats churned people, or seasonal users?

## Next action
Get the contract structure from whoever owns this account and correct the roster line; then flag Amit's credit exhaustion to that owner as an upsell/plan-fit conversation.

## Changelog
- 2026-09-13 — File created from PostHog (Pro Prod) + Sep 11 paying list.

# Feed prototype — customer actionables

One place for every design actionable from PLG customer calls about the feed.

**Sources:** PointTaken (Sep 17) · Fashnstack / Sidharth (Sep 16 call + Sep 17 Monica deep dive) · Patch&Bagel / Jessica Bong (Sep 28)
**Prototype under review:** https://feed-cosmix.vercel.app/

**How to read this**
- **Level 1** is the brand the feedback came from.
- **Level 2** splits it:
  - **Engineering snag**: something is broken or missing; the fix is to build it right. Design owns only the error, empty or disabled state.
  - **Product default**: it works as built, but the default behaviour is wrong. Design owns this.
- ⟡ marks an item another customer raised independently. The other brand is named in brackets. These carry the strongest evidence.
- `[call]` = from the meeting. `[data]` = backed by PostHog.

---

## PointTaken (Sharath + Pratik)
*Sep 17 feed call + ongoing account usage*

### Engineering snags
1. Gavin returns contradictory numbers for the same 30-day window inside one chat: Meta 53 / Shopify 42 in one view, 57 / 39 in another; spend 7,700 vs 12,800. `[call]`
2. Richard breaks under automation. A batch job was killed after burning ~2k credits per run. `[data]`
3. The Orchestrator loses context on the way to Richard. `[call]`
4. ⟡ Monica loses brand context even with brand memory on. *(Fashnstack)* `[call]`
5. Credits can't be pooled across workspaces on a custom plan, which blocks onboarding two more brands. `[call]`

### Product defaults
**Feed**
1. ⟡ Cards don't show the signal that produced them. Pratik asked twice and neither answer satisfied him. *(Patch&Bagel)* `[call]`
2. The feed isn't persona-specific inside one workspace: the founder, catalog manager and performance marketer all see the same thing. `[call]`
3. The rotate-creative card alerts without diagnosing. It should first separate fatigue from overexposure vs. from the creative itself, then offer 2–3 options: same SKU, a variant, or a different SKU. `[call]`
4. ⟡ The catalog card uses SEO hygiene as its signal. Pratik named landing page → add-to-cart conversion as the real one. *(Patch&Bagel)* `[call]`
5. ⟡ The CPM card is a flagged delta with no root cause. He accepted it but called it shallow. *(Fashnstack)* `[call]`
6. There are no custom or tunable prompts in the daily feed. `[call]`

**Product surfaces**
1. Richard has no direct entry point. It needs the "Ask Gavin" pattern. `[call]`
2. The publish path is five manual steps: Spaces → Canva → Shopify. `[call]`
3. ⟡ Credit cost isn't shown before a job runs. Users only learn a job was expensive after it breaks. *(Fashnstack, Patch&Bagel)* `[call]`
4. Context-loss isn't surfaced. A broken run burns credits with no failure state. `[call]`
5. Numbers the agents report carry no provenance: no source, time window, or pull shown. `[call]`

---

## Fashnstack (Sidharth)
*Sep 16 call + Sep 17 unsolicited Monica deep dive*

### Engineering snags
**Model availability**
1. Kling V3 Omni is listed in the UI but unusable. `[call]`
2. Seedance 2.0 is listed in the UI but unusable. `[call]`
3. Seedance 2.5 and Wan 3.0 are missing from the model roster entirely. `[call]`
4. ElevenLabs voiceover failures have no error state, so you can't tell processing from dead. `[call]`

**Output quality**
1. Colours come out wrong on uploaded garments. This is the June/July defect that caused his first churn. `[call]`
2. The product in the final video doesn't match the one uploaded. Reproducible: chat `7f1361fe-04b8-4f09-b22e-4c19f64ed504`. `[call]`
3. Videos end abruptly instead of concluding. `[call]`

**Context + UI**
1. ⟡ Creative Studio overrides brand styling. Brand memory set in onboarding doesn't carry through to generation. *(PointTaken)* `[call]`
2. The right-side pop-up obstructs content and has no obvious dismiss. `[call]`
3. Video mode shows image/static templates. `[call]`

### Product defaults
**Fidelity hierarchy**
1. Storyboards can show a different garment from the one uploaded. The default should be that the product's identity survives every stage. `[call]`
2. Product fidelity and creative quality are treated as interchangeable. It should be fidelity first, creative second. `[call]`
3. Brand constraints don't bind generation. The default should be creative freedom *inside* brand boundaries. `[call]`

**Spend safety**
1. ⟡ There's no cheap preview before an expensive generation, so credits are spent before a failure can be spotted. *(PointTaken, Patch&Bagel)* `[call]`
2. There's no voiceover preview. Voice, tone, pace and script go unheard until the credits are spent. `[call]`
3. ⟡ There's no check at each approval stage: Product → Direction → Storyboard → Preview → Generate → Edit. *(Patch&Bagel)* `[call]`

**Creative range**
1. Storyboards default to four shots: close-up, model turn, basic walk, static product. `[call]`
2. ⟡ Feed sample output reads as generic ("just a model wearing the garment"). He'd scroll past and go prompt manually. *(PointTaken)* `[call]`
3. ⟡ He judges the feed on its output, not on how it works: "at the end of the day the buck stops" at what comes back. *(PointTaken)* `[call]`
4. Blank-box prompting. He wants to be asked questions, not made to write a technical prompt. `[call]`
5. There are no built-in camera effects or animation templates. `[call]`
6. Mode and context don't persist across templates, references, models, presets and exports. `[call]`
7. AI generation and creative control aren't separated. The brand should keep control of product identity, styling, script, voice, music and the final edit. `[call]`

---

## Patch&Bagel (Jessica Bong)
*Sep 28 call: feed prototype review + live GEO review. She runs a small Singapore D2C brand on Growth ($99/mo), uses her monthly credits in about 2 days, and is our healthiest self-serve account.*

### Engineering snags
1. `out_of_credits` has **never fired** on her account, even though she runs out every month, so the credit wall is invisible in our data. `[data]` `[call]`
2. The weekly GEO audit silently pauses at zero credits. The only signal she gets is an email saying "we cannot generate it because no more credits." `[call]`
3. Only ChatGPT's bot has crawled her GEO subdomain; Gemini and Perplexity aren't indexing it. Shobhit suspects a Google indexing issue. Her visibility has dropped on every engine except ChatGPT. `[call]`
4. The interface had changed again when she logged in, and she couldn't find how to log in. `[call]`
5. 308 dead clicks in her first 14 days, meaning something she expects to be clickable isn't. `[data]`

### Product defaults
**Feed**
1. ⟡ **Spend-affecting creative cards should default to Save, not Publish.** Her workflow: save creatives through the week, audit live ads, turn off the losers, then push the saved batch to Meta once a week. Nothing goes live as soon as it arrives. *(Fashnstack)* `[call]`
2. ⟡ Anything touching live ad spend or the storefront needs a hold step and must feel "more secure." *(Fashnstack, PointTaken)* `[call]`
3. ⟡ The signals she wants: sessions, product page → add-to-cart conversion, and traffic by channel into Shopify. Retention signals only suit repeat-purchase brands. *(PointTaken)* `[call]`
4. ⟡ A new user's first question is "how confident are you that this helps the business?" Ad and storefront cards need to show why they can be trusted. *(PointTaken)* `[call]`
5. The card mix should follow the brand type. Her priority is performance-marketing creatives, then GEO, then storefront; a brand whose catalog rarely changes barely needs storefront cards. `[call]`
6. The weekly AI-visibility update should land in the feed, not in an email she has to click through from. `[call]`
7. Mobile as a companion for saving and quick decisions; desktop for doing the work. `[call]`

**Product surfaces**
1. Chat history is one undifferentiated tab. Group chats per agent or project, like Claude Projects. `[call]`
2. The audit cadence is fixed at weekly. Allow every two weeks. `[call]`
3. At zero credits: tell the user in the product, offer a top-up or custom plan right there, and don't silently pause routines. `[call]`
4. GEO results need a stated timeframe for when to judge them. She's asking whether month 3 is the right time. `[call]`

---

## Prototype check — feed-cosmix
*A rough pass, not a full audit. These controls exist in the prototype and partly cover the items listed:*
- **Tune Feed** → partly covers persona and card-mix tuning (PointTaken feed #2, Patch&Bagel feed #5)
- **Save to my preferences / Use it just this once** → a start on saving, but not yet the save → weekly bulk-push flow (Patch&Bagel feed #1)
- **Credit balance + Top up Credits + "free feed limit" message** → partly covers the zero-credit state (Patch&Bagel surfaces #3); it doesn't show cost before an action (PointTaken surfaces #3)
- **Jam with Team** → the human-help path Jessica understood and liked

**Not visible yet:** a signal or reason on each card, a hold step before anything touches live spend, per-agent chat history, and funnel-conversion signals.

---

## Changelog
- 2026-09-29 — File created. PointTaken and Fashnstack actionables carried over from the Sep 22 synthesis; Patch&Bagel added from the Sep 28 call; overlaps marked ⟡ inline. Written here because the Notion workspace is out of free blocks.

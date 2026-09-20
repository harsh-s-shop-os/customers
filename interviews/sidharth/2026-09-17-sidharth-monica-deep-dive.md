# Sidharth Suresh — Monica / Creative Director deep dive

**Date shared:** 2026-09-17 (emailed to Ajay, day after the 2026-09-16 call)
**Author:** Sidharth Suresh (sidharth037@gmail.com), founder of Fashnstack
**Source:** https://docs.google.com/document/d/1AFeiOdIwxOOOhdbxVTiq5aV9dFjf2pizwM1ysj-nWm0/edit
**Why it exists, in his words:** "Given that what I'm building at Fashnstack is closer to Monica's Creative Director offering, I decided to do a deeper dive into Monica." He asked for a coffee or a call to walk through it "from a contribution perspective."

> Unsolicited, unpaid, written the day after his first-ever call with ShopOS. Treat as the most detailed product critique any PLG customer has given.

---

## Brand onboarding

- **Creative Studio overrides brand styling.** It generates its own interpretation rather than following the brand's established visual language — styling, compositions, environments, models and treatments come out disconnected from the brand. The system should separate *creative freedom* from *brand constraints*: creativity inside the brand's boundaries.

## Creative Studio — video generation

- **Limited model selection.** Seedance 2.5 and Wan 3.0 are missing, both important for product-focused generation where accuracy and prompt adherence matter. A creative platform should offer multiple models and route by use case. For fashion, selection should prioritise: product accuracy, garment consistency, prompt adherence, motion quality, human anatomy, temporal consistency.
- **Model quality is inconsistent.** Existing video models frequently produce sub-par output, especially on holding the identity and detail of the source garment. A visually impressive video is unusable if the garment changes, the print disappears, the silhouette shifts, or details are hallucinated.

## Chat / storyboard experience

- **Storyboards do not preserve the actual product.** Even accepting that a storyboard is a sketch, it can depict a completely different garment from the one uploaded. "As a user, seeing a storyboard of a different product immediately reduces confidence in the generation that follows." Silhouette, proportions, key design elements, colour and product identity should survive even a rough sketch.
- **Storyboards lack creative variety.** They fall back on generic fashion-video patterns: close-up of the garment, model turning around, basic walk, static product shot. *(Same complaint he made verbally on the 2026-09-16 call.)* He wants narrative progression, product reveals, environmental interaction, movement and transitions, detail shots, camera choreography, styling-led compositions, editorial concepts, brand-specific visual language.
- **It doesn't feel like a creative-director layer.** It reads as a generic shot planner. The user should look at a storyboard and understand *why each shot exists* and how it serves the concept.

## Generated video quality & product accuracy

- **Severe product hallucination.** Output deviates materially from the supplied product — appearance, structure, colour, detailing, silhouette, styling. "Product accuracy is a hard requirement, not simply a quality preference." If the product in the output differs materially, the whole asset is worthless.
- **Input-to-output disconnect.** The expectation gap he names step by step: user provides product → provides creative direction → approves storyboard → **credits are consumed** → final output doesn't reflect the approved direction.
- **Credit burn makes failure worse.** A bad generation isn't just a quality issue when you paid for it. He asks for stronger pre-generation validation, better previews, or cheaper low-cost previews before committing to an expensive generation.
- **Reproducible case:** chat ID `7f1361fe-04b8-4f09-b22e-4c19f64ed504` — output materially differed from supplied product and direction; unusable asset.
- **Abrupt ending.** Videos stop rather than conclude; the final shot needs a deliberate transition, hold, camera move or product-focused ending.

## Technical issues

- **Kling V3 Omni listed but unavailable.** UI says available, model can't be used. "Users cannot distinguish between genuinely available capabilities and placeholder capabilities" — he frames this explicitly as a trust issue.
- **Seedance 2.0 listed but unavailable.** Same.
- **ElevenLabs API reliability** affects voiceover. Failures should surface as actionable error states rather than leaving the user unsure whether it's processing or dead.
- **Model availability should be a product state** — hide it, mark it unavailable, or give an expected-availability state.

## UI / UX issues

- **Right-side pop-up obstructs content** and has no obvious dismiss.
- **No voiceover preview.** Voice is subjective; he wants to hear voice, tone, pace, script and pronunciation before spending credits.
- **Templates don't match the mode.** He was in Video mode and was shown image/static templates. "Showing irrelevant templates can make users conclude that the platform does not support the type of content they are looking for, even when the underlying capability exists" — and first-time users form their judgment on exactly this.
- **Mode/context should persist** across templates, references, examples, models, presets and export settings. Inconsistent context "can contribute to early churn."

## His core product concerns

- **Product accuracy must be a non-negotiable constraint.** For fashion, an aesthetically good video of the wrong garment has almost no commercial value. Optimise for **product fidelity first, creative quality second** — not as interchangeable quality dimensions.
- **The system feels generative, not brand-aware.** It generates from generic fashion patterns instead of understanding the individual brand, product and references. The opportunity: make it feel like it has learned the brand's "taste, constraints, and way of seeing."
- **The approval loop must build confidence progressively:** Product → Creative Direction → Storyboard → Preview → Generation → Final Edit, with verification at each stage. "If the storyboard is already showing the wrong product, the user should not have to proceed to an expensive final generation to discover the problem."
- **Separate AI generation from creative control.** AI generates; the brand keeps control of product identity, brand styling, creative direction, script, voice, music, captions and final edit.

> His closing line: this would make the product feel less like a **video generator** and more like an actual **AI creative studio for fashion brands**.

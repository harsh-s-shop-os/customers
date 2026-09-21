# Patricia Noble Torres — session recordings, July 2026

**Source:** PostHog session replay, AI-generated summaries. Five recordings, all July 2026 — the only recordings that exist for this account.
**Gathered:** 2026-09-20 by Lobster.
**Account:** patricia.noble.torres@gmail.com · Business $199/mo · brand **Habana Resortwear** ("Habana PC")

> Read this before trusting the event counters in `active/patricia-noble.md`. The recordings show substantial finished output that the event schema never recorded.

---

## 1. Jul 8 — Demo request fails on `/contact-sales` *(four days before she signed up)*

- Navigated to the contact-sales page (00:02) and **completed the full lead-gen form** — email, name, company.
- Clicked **"Request a Demo"** (00:43). Form sat in a loading state ~4 seconds.
- Returned an error: **"Webhook responded with status 404"** (00:47).
- Network logs show the POST to the enterprise-demo lead endpoint actually failed with a **502 Bad Gateway**. The user-facing message did not match the real failure.
- **Session ended on the error state.** The demo was never booked and no lead reached ShopOS.

**This is the first thing she ever did on ShopOS, and it was an attempt to talk to a human.** She signed up self-serve four days later anyway.

## 2. Jul 13 (overnight session) — Creative Director, credit wall, plan upgrade, chat data loss

- Onboarded **Habana Resortwear by connecting an Instagram URL** (05:59) — not a website.
- Worked with the Creative Director agent (named **"Tere"**) on a social-media ad campaign, with a detailed discussion of brand direction.
- **Hit a credit limit mid-work and upgraded to the Business plan** (01:14:15) to keep going.
- **The active chat was unexpectedly deleted** (01:25:52), forcing her to start a new thread.
- **She expressed her frustration to the agent** (01:35:25).
- Recovered: re-uploaded her product assets and went on to generate **multiple campaign directions and final image assets**.

## 3. Jul 13 — Diwali campaign concepts and a client catalogue

- Opened chat history to continue the branding project (00:16).
- Analysed uploaded product images (00:39) and generated **lifestyle shots for a Diwali campaign drop**.
- Used the Image Editor to review batches (04:23) and **saved selected assets to Brand Memory** (08:18).
- Asked how to present the collection to clients (43:03), then ran a guided workflow to build a professional catalogue — **specifying Spanish language** and detailed product descriptions.
- **A 13-slide catalogue generated successfully.**
- Friction: **the in-app preview failed to load**, so she had to download the file to check the output.

## 4. Jul 13 — Refining the branded catalogue for "Habana PC"

- Used Creative Studio to iterate on the catalogue: asked to fix slide 6 (remove a checkmark, keep a colorway).
- Friction: **the catalogue downloaded as PowerPoint rather than PDF**; the agent worked around it by supplying a direct PDF link.
- Directed the agent to apply brand identity from Brand Memory — and caught it **using the Instagram logo as the brand logo**. She corrected it by uploading the real logo.
- Gave final instructions to update slide images and the cover.
- **Session ended with a fully branded PDF catalogue successfully generated.**

## 5. Jul 14 — Reviewing the finished work *(her last session ever)*

- Home page (00:08) → chat history → "Recovering branding project and product image analysis" (00:14).
- Scrolled a long interaction with the AI (Claude Sonnet 4.5) about the product catalogue (00:24).
- History confirms the AI analysed product images, **updated brand memory with logos and colour palettes** (00:35), and applied five design revisions to the presentation (00:44).
- She reviewed the final outputs and the confirmation logs (01:33).
- **No errors, no layout issues. Then she never came back.**

---

## What these recordings change

1. **She produced real, finished work.** Campaign image assets, Diwali lifestyle shots, a 13-slide catalogue, a fully branded PDF catalogue, populated Brand Memory. The account file said "zero completed generations" on the strength of event counters — the counters missed all of it because the output came through chat / Creative Director / Creative Studio flows.
2. **She did not buy on a promise — she bought at a wall.** The upgrade happened mid-session, after hitting a credit limit while actively producing. That is the opposite of the "fast conversion, no output" churn shape she was filed under.
3. **ShopOS dropped her first contact.** She asked for a demo on Jul 8 and the endpoint 502'd. Nobody knew she existed until she paid.
4. **The bug list is specific and fixable:** demo form 502 (with a misleading 404 message), chat deleted mid-session, in-app catalogue preview fails to load, PPTX served where PDF was asked for, Instagram logo picked up as brand logo from an Instagram-URL onboarding.
5. **She works in Spanish** and onboarded from Instagram, not a website — worth knowing before anyone writes to her.

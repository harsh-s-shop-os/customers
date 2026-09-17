# ShopOS <> Point-Taken (Sharath/Pratik) — Product pulse check (Sep 17, 2026)

**Attendees:** Harsh Singh, Shobhit Khurana, Vedant Vaibhav, Adarsh Mishra, Pratik Bajaj, Manish Mishra, Sharath Ravishankar
**Source:** Gemini notes + transcript, downloaded from Google Docs
**Original doc:** https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit

---

# **✍️ Quick notes**  

*Please* ***rate the new Quick notes tab*** *by taking a* [*short survey*](https://google.qualtrics.com/jfe/form/SV_5bXzKQfylMIhSXc?confid=iVj80jIDvrYcZ3gKPaIBDxISOBEBMgUIigIgABgECA&entryPoint=footerQuickNotes&isGoogler=False)*.*

  

## **Point-Taken\<\>ShopOS**

  

Sep 17, 2026

[Harsh Singh](mailto:harsh.singh@shopos.ai) [Shobhit Khurana](mailto:shobhit.khurana@shopos.ai) [Vedant Vaibhav](mailto:vedant.vaibhav@shopos.ai) [Adarsh Mishra](mailto:adarsh.mishra@shopos.ai) <pratik@pointtaken.in> [Manish Mishra](mailto:manish.mishra@shopos.ai) <sharath@pointtaken.in>

  

ShopOS feed introduction and creative features reviewed with data discrepancy discussions.

  

## **ShopOS Feed Concept and Prototype**

  - Harsh presented a prototype feed interface designed to replace blank prompt boxes with actionable cards related to brand performance, creative output, and AI visibility.
  - The feed leverages background agents to research categories and competitors, creating an echo chamber of relevant drafts for brand owners.
  - Draft suggestions do not consume credits until the user actively engages in actions like tweaking or finalizing a campaign.

  

## **Performance Signals and Data Capabilities**

  - The platform includes built-in performance marketing features like SKU quadrant analysis, fatigue detection, and catalog health monitoring from launch.
  - Future updates aim to integrate MS Clarity for filtering bot traffic versus human interactions, though this is not in the version 0 scope.
  - SEO and keyword research modules are excluded from the current development roadmap for the next few months.

  

## **Workspace and Credit Management**

  - Pratik raised concerns regarding the inability to distribute a centralized credit pool across multiple workspace containers.
  - Harsh confirmed that agency workspaces will support sharing plans and credits among connected workspaces once custom plan constraints are resolved.

  

## **Meta Ads Library and Creative Intelligence**

  - The library now contains over 24,000 analyzed ads, including approximately 14,000 videos, categorized by hook, funnel stage, and media type.
  - Adarsh demonstrated that image-based ads are remixable via the Monica agent, which utilizes brand memory to maintain formatting consistency.
  - Creative Pulse provides AI-driven suggestions based on ad performance data from the previous 14 days and competitor analysis.

  

## **Platform Integrations and Bug Fixes**

  - Adarsh confirmed MS Clarity is integrated and available for connection.
  - Resolved reported bugs concerning zero copy reporting and pixel firing failures.

  

## **Data Attribution and Model Performance**

  - Sharath flagged significant discrepancies between Meta and Shopify purchase data within single reports.
  - Identified a lack of trust in agent-generated data due to stark differences between report figures and manual verification.
  - Adarsh attributed inconsistencies to potential LLM behavior, where incomplete data fetching creates noise artifacts.
  - Pratik and Adarsh discussed leveraging higher-reasoning models to improve context maintenance and reporting accuracy.

  

## **Client Onboarding and Future Development**

  - Pratik targeted a 4-to-5-week timeline for onboarding a new client and implementing feature sets.

  

## **Next steps**

  - \[Pratik Bajaj, Sharath Ravishankar\] Define Agent Jobs: Define 5 jobs to be done by agents for the ShopOS feed implementation. Include specific signals and expected downstream actions for each.
  - \[Harsh Singh\] Fix Credit Allocation: Fix the workspace credit sharing and allocation issue for custom plans. Ensure that credits can be distributed and shared across workspaces.
  - \[Harsh Singh\] Notify Credit Fix: Notify the team in the WhatsApp group once the credit sharing and allocation feature is fixed. Provide an update once the functionality is operational.
  - \[Harsh Singh\] Implement Click Filtering: Incorporate bot versus human click filtering for MS Clarity signals in future ShopOS versions. Ensure that signals surface relevant user interaction data.
  - \[Pratik Bajaj, Sharath Ravishankar\] Provide Ad Feedback: Review the analyzed ad data and provide user experience feedback to the team.
  - \[Adarsh Mishra\] Schedule Meeting: Arrange a 1-hour call between 2:00 PM and 3:00 PM with the developer to discuss additional features.
  - \[Sharath Ravishankar\] Connect MS Clarity: Link the MS Clarity tool to the platform and report if it is helpful.
  - \[Sharath Ravishankar\] Share Chart Data: Share the full chart and date range details to assist in troubleshooting attribution data inconsistencies.
  - \[Adarsh Mishra\] Investigate Agent Performance: Review the performance agent reasoning logs to address the data inconsistency issues and report findings.
  - \[Pratik Bajaj, Sharath Ravishankar\] Send Job IDs: Send the list of job IDs for the upcoming client onboarding and feature setup.

  
  

  
**Want to see more?** [View the full notes  
](about:blank)Tip: You can always access your full notes from the left sidebar.

  
  
  

*You should review Gemini's notes to make sure they're accurate.* [*Get tips and learn how Gemini takes notes****  
***](https://support.google.com/meet/answer/14754931)

# **ð Full notes***  
*

 Sep 17, 2026

## **Point-Taken\<\>ShopOS**

Invited [Harsh Singh](mailto:harsh.singh@shopos.ai) [Shobhit Khurana](mailto:shobhit.khurana@shopos.ai) [Vedant Vaibhav](mailto:vedant.vaibhav@shopos.ai) [Adarsh Mishra](mailto:adarsh.mishra@shopos.ai) <pratik@pointtaken.in> [Manish Mishra](mailto:manish.mishra@shopos.ai) <sharath@pointtaken.in>

Attachments [Point-Taken\<\>ShopOS](https://calendar.google.com/calendar/event?eid=MGJiOWNsNWtibG42MTBodWxzczhnbzhzdjIgc2hvYmhpdC5raHVyYW5hQHNob3Bvcy5haQ)

Meeting records [Transcript](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?usp=drive_web&tab=t.860op2jur400) 

  
  

### **Summary**

ShopOS feed introduction and creative features reviewed with data discrepancy discussions.  
  
**ShopOS Feed And Features**  
Introduction of ShopOS feed replaced prompt boxes with agent driven insights. Credit usage clarified for initial ideas.  
  
**Meta Ads And Analytics**  
Demonstration of Gavin meta ads library and creative pulse dashboard. Discussion highlighted tracking metrics and SEO timelines.  
  
**Data Discrepancies And Models**  
Review of product report data inconsistencies attributed to model behavior. Decision made to investigate sub agents performance.

  
  

### **Next steps**

  - \[Pratik Bajaj, Sharath Ravishankar\] Define Agent Jobs: Define 5 jobs to be done by agents for the ShopOS feed implementation. Include specific signals and expected downstream actions for each.
  - \[Harsh Singh\] Fix Credit Allocation: Fix the workspace credit sharing and allocation issue for custom plans. Ensure that credits can be distributed and shared across workspaces.
  - \[Harsh Singh\] Notify Credit Fix: Notify the team in the WhatsApp group once the credit sharing and allocation feature is fixed. Provide an update once the functionality is operational.
  - \[Harsh Singh\] Implement Click Filtering: Incorporate bot versus human click filtering for MS Clarity signals in future ShopOS versions. Ensure that signals surface relevant user interaction data.
  - \[Pratik Bajaj, Sharath Ravishankar\] Provide Ad Feedback: Review the analyzed ad data and provide user experience feedback to the team.
  - \[Adarsh Mishra\] Schedule Meeting: Arrange a 1-hour call between 2:00 PM and 3:00 PM with the developer to discuss additional features.
  - \[Sharath Ravishankar\] Connect MS Clarity: Link the MS Clarity tool to the platform and report if it is helpful.
  - \[Sharath Ravishankar\] Share Chart Data: Share the full chart and date range details to assist in troubleshooting attribution data inconsistencies.
  - \[Adarsh Mishra\] Investigate Agent Performance: Review the performance agent reasoning logs to address the data inconsistency issues and report findings.
  - \[Pratik Bajaj, Sharath Ravishankar\] Send Job IDs: Send the list of job IDs for the upcoming client onboarding and feature setup.

  
  

### **Details**

  - **ShopOS New Feed Experience Overview**: Harsh Singh introduced a new ShopOS experience designed to replace blank prompt boxes with an Instagram-like feed driven by background agents that research brand URLs, creative performance, and storefront data. Pratik Bajaj and Sharath Ravishankar were shown how feed cards provide actionable suggestions—such as approving, dismissing, or remixing ideas—or engaging expert teams via WhatsApp or Slack ([00:04:08](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.xd12uxdde1o3)).

  - **Brand Onboarding and Signal Integration**: Harsh Singh explained that background agents analyze category competitors and upcoming events like Diwali to generate drafts and assets ([00:06:17](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.dehgd5xhfhga)). Pratik Bajaj noted that for active stores like their women's western wear and upcoming men's wear brands, connecting Shopify, Meta, Google Analytics, and past conversations provides essential context for signals like high impressions without add-to-carts, while pro modes offer deeper behavioral insights like cart abandonment tracking ([00:08:47](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.dkcg8v1ilkfn)).

  - **Credit Consumption for Initial Ideas**: Sharath Ravishankar inquired about credit usage for performance marketer and storefront manager ideas, and Harsh Singh clarified that initial drafts and ideas are free of charge, with credits only being deducted once a user decides to act on or tweak them ([00:12:46](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.bsnqukvpznz6)).
  - **Bot and Rage Click Filtering Limitations in V0**: Sharath Ravishankar suggested integrating MS Clarity to filter out bot and rage clicks from human interactions to improve data accuracy for business decisions ([00:14:33](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.hs3ow3lwhizg)). Harsh Singh responded that filtering specific bot or rage clicks is out of scope for version zero, which will focus on standard signals like top-viewed pages and user geography, alongside custom routines ([00:15:30](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.gvacgsqdtns9)).

  - **SKU Quadrant Analysis and Performance Marketing Metrics**: Pratik Bajaj discussed using SKU quadrant analyses to identify top-performing revenue drivers and variant-specific sales patterns ([00:17:27](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.l5urkz1fauv1)). Harsh Singh confirmed that SKU quadrant analysis, ROAS performance, fatigue detection, and catalog health are baked into Gavin from day zero, offering high-level overviews with options to deep dive via agent chats ([00:18:55](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.9z8bih890urn)).

  - **Handling Increasing CPM Costs**: Pratik Bajaj asked how rising CPM costs are handled by the system ([00:22:49](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.x4u3524674ac)). Harsh Singh explained that a feed card will highlight the CPM drop using cheaper models without deep-dive root-cause analysis to conserve credits, leaving it to the user to approve, remix, or dismiss the suggestion ([00:24:14](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.hnc4s2nbu28o)).
  - **Creative Fatigue and Ad Rotation**: Sharath Ravishankar and Harsh Singh discussed creative fatigue and ad rotation under Andromeda's algorithm, where Harsh Singh noted that the creative pulse dashboard utilizes a meta ad library analyzing 50,000 ads and competitor hooks to provide chat-based replacement suggestions ([00:26:26](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.sruwswoxdhra)).
  - **Catalog-Level Recommendations and Conversion Metrics**: Pratik Bajaj and Harsh Singh discussed catalog-level recommendations, identifying landing-page-to-add-to-cart conversion metrics as a critical signal for catalog changes rather than basic SEO hygiene tags ([00:28:35](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.lqj28jjcehhl)).

  - **Keyword Research and SEO Pipeline**: Pratik Bajaj requested keyword research modules for intent-based purchases and catalog enrichment, but Harsh Singh clarified that SEO and keyword management are not on the pipeline until at least the end of October, with visibility currently focused on AI and GEO visibility ([00:32:39](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.u5knkaobmd9p)). Following this, Pratik Bajaj and Sharath Ravishankar agreed to compile five specific jobs to be done for their feed to ensure day-zero value ([00:33:48](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.dy1u6doodsvl)) ([00:37:38](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.twpg2tkhron4)).
  - **Workspace Credit Sharing and Custom Plan Blockers**: Pratik Bajaj shared their screen to highlight an ongoing struggle with allocating and sharing credits across workspaces ([00:36:35](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.gdctxt20plrl)) ([00:39:20](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.w8dtzwvlec41)). Harsh Singh acknowledged that the feature is blocked on custom plans and promised a fix the same day, though they noted that distributing a single credit pool directly among workspaces is currently unsupported ([00:40:33](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.o78wvvvgwtlg)).

  - **Gavin's Meta Ads Library and Universal Ad Repository**: Adarsh Mishra demonstrated new features on Gavin, including the meta ads library where users can track public competitor ads by brand or keyword and analyze them within a universal repository segregated by category, media type, hook, funnel stage, and awareness level ([00:42:42](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.ei7j0kuxp44b)). Adarsh Mishra also showed how image ads can be remixed through the Monica agent using brand memory ([00:46:34](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.oh3ilcrkv5v0)).

  - **Creative Pulse Dashboard Review and Next Steps**: Sharath Ravishankar shared their screen to review the creative pulse dashboard, confirming it displays fatigue graphs, top competitors, and top performers based on set metrics ([00:50:34](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.e3apsc42u006)). The meeting concluded with plans to schedule another session from 2:00 to 3:00 PM the next day with Shobhit and the developer to further discuss feed jobs and demos ([00:56:07](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.3jzs7io2o8uz)).

  - **Microsoft Clarity Integration and Bug Resolution**: Adarsh Mishra stated that Microsoft Clarity had been added to the tool and requested that Sharath Ravishankar connect it to evaluate its usefulness and provide feedback. Additionally, regarding a previous bug involving zero-copy issues and pixels failing to fire, Adarsh Mishra asked Sharath Ravishankar to notify them when the next report runs so they can compare the fixes and confirm the issue is resolved. Sharath Ravishankar agreed to connect Microsoft Clarity and report back when the next report runs ([00:57:14](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.blh0419n2tmw)).
  - **Data Inconsistency in Product Reports**: Sharath Ravishankar raised an issue regarding data inconsistencies in product reports generated over the last 30 days, screen-sharing examples where meta purchases were listed as 53 and Shopify purchases as 42, while another view within the same chat showed 57 Shopify purchases and 39 meta purchases ([00:57:56](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.ce5tjlk98mqy)). Furthermore, a second pulled report showed a spend of 7,700 compared to 12,800 in another instance, prompting Sharath Ravishankar to question which figures are accurate and express concern that customers making business decisions without verification would rely on incorrect information ([01:02:18](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.l6u8xv2v0s6)). Adarsh Mishra initially attributed discrepancies to differing tracking sources, but Sharath Ravishankar clarified the conflicting numbers came from the same source (Gavin) within the same chat interface ([00:57:56](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.ce5tjlk98mqy)). Pratik Bajaj added that such data discrepancies undermine trust in agent recommendations, noting that they perform similar activities using Claude-based connectors for Shopify and Meta ([01:00:58](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.np1t0wmj96m5)) ([01:04:15](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.1etcu2h6uz15)).

  - **LLM Model Analysis and Client Onboarding Timeline**: Adarsh Mishra examined the conflicting reports and suspected that LLM behavior, such as the model becoming lazy and fetching partial data when multiple pages are requested, contributed to the discrepancies ([01:03:30](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.mfxip61cwpot)). When Pratik Bajaj inquired about the underlying model, Adarsh Mishra confirmed that the system might have been using Claude Sonnet 4.6 on auto mode. Pratik Bajaj noted that higher models with better context maintenance and reasoning capabilities yield different results ([01:04:15](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.1etcu2h6uz15)). Adarsh Mishra instructed Sharath Ravishankar to check the sub-agents performance quantities returns in the chat interface, and Sharath Ravishankar agreed to share the chat link in the call chat. Concluding the meeting, Pratik Bajaj stated they would send a list of job IDs and expressed optimism about building new features over the next 4 to 5 weeks to support a new client onboarding ([01:05:28](https://docs.google.com/document/d/1iC8VhKQ2UdErjuldt1r38MLKxPEpeKhcmR1V0WZBeLM/edit?ouid=103018488318832137054#heading=h.czommdy225r3)).

  
  

*You should review Gemini's notes to make sure they're accurate.* [*Get tips and learn how Gemini takes notes*](https://support.google.com/meet/answer/14754931)

*How is the quality of* ***these specific notes?*** [*Take a short survey*](https://google.qualtrics.com/jfe/form/SV_5bXzKQfylMIhSXc?confid=iVj80jIDvrYcZ3gKPaIBDxISOBEBMgUIigIgABgECA&detailLevel=standard&hasImages=True&entryPoint=footerMain&isGoogler=False) *to let us know your feedback, including how helpful the notes were for your needs.****  
***

# **ð Transcript***  
*

 Sep 17, 2026

## **Point-Taken\<\>ShopOS - Transcript**

### **00:00:08**

  

**Adarsh Mishra:** I thought you had something on the Okay, We'll wait.

**Harsh Singh:** to join. So there are two things for the call. Uh the first one that we want to showcase a new experience that we're building around shop OS. Uh want to ensure that if it's landing for brand owners like you you think any relevance is there in that experience. And the second part of it is uh you had some doubts on Perf marketing and the Gavin flow. So Adarshis here to walk you through that.

**Sharath Ravishankar:** Mhm.

**Adarsh Mishra:** Please start that.

**Sharath Ravishankar:** Oh, it's going a second. Just bring

**Adarsh Mishra:** Yeah.

**Sharath Ravishankar:** it. Let's just give it a couple minutes.

**Harsh Singh:** Shut it.

**Pratik Bajaj:** Hey guys, good evening.

**Sharath Ravishankar:** Okay. Yeah.

**Harsh Singh:** Right. Uh so should we start with the okay so

**Sharath Ravishankar:** Mhm. Mhm.

**Harsh Singh:** SharathI think we when we last spoke you spoke about something along the lines of having an entire workflow being handled on ShopOSso that you don't have to lift too many fingers to get something published right so I I am just

  
  

### **00:02:36**

  

**Sharath Ravishankar:** Mhm. Yes.

**Harsh Singh:** presenting my screen hold

**Pratik Bajaj:** Okay.

**Harsh Singh:** have to quit. No, it was it was no we okay returning.

**Pratik Bajaj:** These Please

**Harsh Singh:** I have to quit and reop. Yeah. Okay. Can you see the screen right?

**Sharath Ravishankar:** Um, nope.

**Pratik Bajaj:** start.

**Sharath Ravishankar:** I can't see the screen. Sorry. All right. Now I can see a screen.

**Harsh Singh:** Yes. Right. So the idea here is first of all when we enter the brand for example when we enter pointt.in The idea here is the moment you start we want to understand everything about your brand and by and everything I mean every aspect of your let's say from your creative performance to how your ads running to how your storefront is performing everything so that we already have certain idea on where your brand is headed and we set up certain loops in the background and then by the time we are done by the time those routines are done by the time we are finished with with building a complete understanding.

  
  

### **00:04:08**

  

**Harsh Singh:** Instead of landing you on a blank prompt box where you're trying to figure out what to do next and what all can you do, we start with things that are already running for your brand and uh things that you can act directly take action on, approve, deny or to use your language last time that you mentioned uh kill, tweak or keep something along those lines. We can give you those actions and you can start quiet with those actions. decide what to do or create actions of your own. So right now what you saw was I entered a brand brand URL. We the system understood your brand, ShopOSunderstood your brand and you land on a feed like this, a homepage like this where you can just scroll through a whole bunch of cards related to performance, related to creative, related to AI visibility, anything you prefer, anything that's relevant and we are giving you not just like just useful information that you that you might be glad to know. Here we can actually each card has a couple of actions associated with it.

  
  

### **00:05:09**

  

**Harsh Singh:** You can approve that action. You can dismiss that action. Depending on that, these cards may come more often or less often. These kind of suggestions will come more often or less often. Another option you have is that you can go ahead and remix this idea with an agent jam with it. decide what works, what doesn't or you can actually have a team by the end of it that have an option for jamming with an entire team where our own experts sort of join on let's say any channel of your choice let's say WhatsApp, Slack, wherever and we can uh decide how to get the final output that you like that you really want to get published. So this is broad overview that we have. We'd like to know your thoughts. What do you think first? I'll just add a little more to it. Uh so we had a few conversations with uh other brands. The problem that a lot of them are facing is that they land in any AI software to a brown box and they sort of have to figure out that what exactly do they want for the brand here instead of that we are running a bunch of agents in the background for your particular brand.

  
  

### **00:06:17**

  

**Harsh Singh:** So let's take example for any shoe brand that you have entered as an URL. Now based on your brand, we'll research the category, the competitors and everything and every day you come to an Instagram like feed which is more like an echo chamber of your own brand. So we going to create a bunch of assets and drafts ready for you. For example, let's say Diwali is coming in. So the creative agent might come in and say you know Diwali is coming around the corner and your competitors are creating posts like this. how about this campaign that I've thought about and let's go forward with this AI visibility would come in like you know these are the couple of prompts where your competitors are being cited you are not how about we write a blog for that so that is the idea you can of course go ahead tune whatever agent you want to see more or less of course all the campaigns that are there doing them with either agents

**Pratik Bajaj:** That's

**Harsh Singh:** or get a human in the loop but the idea is that we always give you a bunch of drafts to go through and then it's up to you to decide which ones do you want to go forward with,

  
  

### **00:07:18**

  

**Pratik Bajaj:** heat.

**Harsh Singh:** which ones you just want to kill, which ones you want to tweak and go forward with.

**Pratik Bajaj:** Can I can I uh jump in over here?

**Harsh Singh:** Yeah.

**Pratik Bajaj:** I'm broadly happy that those recommendations and the processes that uh we sort of recommended right like the keep

**Harsh Singh:** Yeah.

**Pratik Bajaj:** concept uh but we are applying those basis a certain set of signals right. Can I can I get an understanding one?

**Harsh Singh:** Yeah.

**Pratik Bajaj:** I'm assuming this is a feed URL, right?

**Harsh Singh:** Yeah.

**Pratik Bajaj:** A feed URL depending on uh whoever is say managing the store. Uh it's a feed URL basis that persona. I mean it could be the founder, it could be the uh cat catalog owner, it could be the performance marketer owner or uh it could be a general generic feed that's there as well. Something for to optimize later. But what is happening underneath especially what signals are being considered? Can you give an overview and understanding of

**Harsh Singh:** Yeah. So this is still an early prototype but the idea is that based on your URL of course we're going to scrape a bunch of things and see in that category what are the things which are trending uh check what your competitors are doing and based on those signals create more and more drafts

  
  

### **00:08:47**

  

**Harsh Singh:** in those aspects of creative generation performance marketing visibility and storefront. Do a general audit of your store. See what are the signals coming in where the customers are not taking an action and then recommend actions right there also. So in order for it to be less generic, you'll have to give in a bit of your connection access as well. So you might connect your Shopify and Meta. So whatever drafts that come up after that will be more backed with real data and the real usage of the brand.

**Pratik Bajaj:** So once again I'm repeating right so we we currently have one active store uh which we are using and it's surrounding the women's web right and uh Shopify meta Google analytics uh these are assets that's already connected including memory update uh including all past

**Harsh Singh:** Yep.

**Pratik Bajaj:** conversations uh with agents as well as uh generic conversations and all generations that we have done right so it it holds a whole lot of context especially with respect to this one particular brand my idea is I want to onboard another brand uh tomorrow which is an inway brand then I want to onboard another men's wear brand right so that context uh will automatically get provided I I'll give you a little more understanding right when you say when I say signals my signals could be

  
  

### **00:10:16**

  

**Pratik Bajaj:** related to hey I'm I'm running the ads the ads are getting impressions but uh they are getting landing pages as well but they are not getting let's say add to car right uh that's a signal that's a very strong signal to very specifically tweak something uh uh in lines with the uh description or the imagery itself, right? It could be a video that I want to add. It could be a lifestyle hero image that I want to add or it could be that hey,

**Harsh Singh:** It's good.

**Pratik Bajaj:** I'm getting some natural traction uh on a particular product, right? Uh say Richard identifies that, right? And now I want to uh scale the ad performance of this and especially considering uh uh Diwali coming in like you said here are some festive uh creatives around it. So these are all uh things that we are doing right now for the brand which we are which has a certain workflow but we are expecting let's say the agent kind of uh works toward it. Okay, I'll I'll let you move forward with the demo.

  
  

### **00:11:28**

  

**Pratik Bajaj:** I understand that this is like a feed. The feed has a certain uh request human in the loop request uh and then you can accept it. You can remix it or you can simply uh you know deny or not move forward with it. What else? What what are we moving ahead with?

**Harsh Singh:** Uh apart from this, there is just another mode to if you're an upgrade, if you're a pro member, you can just see them in a different view That's You have a bunch more quantity of drafts that we are preparing for you and we've included something called signals where you have to make sure that you connect the right stores, give it the right access and then based on that it will start giving you a bunch of uh uh drafts on how your customers are behaving within your store and what are the right signals and what according to it can be tweaked in order to make that particular ular thing a little better. So if let's say some customer comes spend some time and adds an item to your cart but did not check it out, you can later the agent can later recommend that you know we should offer them a discount or you know stuff like that here as well.

  
  

### **00:12:46**

  

**Harsh Singh:** But I'm also looking for input of things to include here which makes it a little bit more meaningful for you guys.

**Sharath Ravishankar:** Yeah. So to add to this now I like the way the dashboard is looking and things and the UI aspect of it is really clean and it giving a lot of information. Now when it comes to the storefront manager right if you scroll to the left a bit right so here all of these things you know we have a performance marketer uh thing there right on your left now this one is creating it will tell you what ads to create essentially correct

**Harsh Singh:** Yeah.

**Sharath Ravishankar:** what campa camp campaigns so on and so forth now my question is for it to come up with all these little ideas and concepts u for for the user that is Now obviously there is a

**Harsh Singh:** H

**Sharath Ravishankar:** credit cost attached to this. Now for example if I don't have if I don't feel like the first one that is suggested is is something that we should build a campaign upon and move on to the next one.

  
  

### **00:13:43**

  

**Sharath Ravishankar:** Now obviously it's consumed credits for that. Correct. It's consume credits to create the campaign in the back end already or is this just an idea that is giving you and

**Harsh Singh:** no

**Sharath Ravishankar:** then once you approve it then it starts using more credits to create the entire campaign.

**Harsh Singh:** the drafts initially whatever drafts you see will not consume any credits in when you start

**Sharath Ravishankar:** Uh-huh.

**Harsh Singh:** acting on it like when you decide to tweak it a little bit or do something around that then we'll start deducting credits.

**Sharath Ravishankar:** Understood. Understood. Now,

**Harsh Singh:** So the first and ideas are free.

**Sharath Ravishankar:** if perfect, understood. Now, I I I like the way it's broken down in different columns. Now, if you go back to the right, which is your signals area. Now in the signals it will be a lot more accurate and it'll probably give us a bit more information

**Harsh Singh:** Yeah.

**Sharath Ravishankar:** when after you uh I I think I erased this as well to kind of connect my MS clarity to it as well.

  
  

### **00:14:33**

  

**Sharath Ravishankar:** So that will not only show items that's been added, but it'll also show the users uh you know the screen the movement or or or what which page they landed on more or what they tried to click on. Are they rage clicks? And then we wanted to be able to kind of differentiate what is actual user clicks and what are bot clicks because there's a lot of these rage clicks that happen that are basically bots bot agents that are just basically We bend. to uh scrape and test the sites as well and kind of take that out of the equation and kind of uh filter out the human interactions and then you'll be able to have more accurate data to kind of make a lot more business decisions.

**Harsh Singh:** Got it. So, uh sh Manish said I'll take that one. So,

**Sharath Ravishankar:** Yeah.

**Harsh Singh:** uh the particular use case that you're talking about, right? B clicks, reach clicks, that's a bit specific.

**Sharath Ravishankar:** Yeah.

**Harsh Singh:** I I'm not really sure if you'll be doing that in the first version.

  
  

### **00:15:30**

  

**Sharath Ravishankar:** Nice.

**Harsh Singh:** Right. So the first version for example if you have connected to MS clarity or a mix pan the signals will ensure that the uh things like okay the these are your most viewed pages or these are the geography from where your users are coming which are the standard stuff right that that will start surfacing up if we see adding that B thing right I mean again uh it will just be a small change we can do that but uh

**Sharath Ravishankar:** Okay.

**Pratik Bajaj:** I had enough punch.

**Harsh Singh:** given that one you I've given that one very specific example. So I'm not we'll keep that in mind and make sure that that it is there. But to start with signals be more around the uh the generic things that people look out for right. So those will surface surface out based on whatever connectors you have done.

**Sharath Ravishankar:** Okay.

**Harsh Singh:** But obviously routines feature will still be there. So anything specific that is not being surfaced out right you can go ahead and create your own routine.

  
  

### **00:16:27**

  

**Harsh Singh:** Maybe some somewhere down the line the routine and feed might just merge and we will have that

**Sharath Ravishankar:** Mhm.

**Harsh Singh:** option. So so for example uh Vedantand Harshwill show you we have option to tweak the feed itself

**Sharath Ravishankar:** Mhm.

**Harsh Singh:** right maybe you want more of signals and more of creatives less of the ad thing or visibility thing.

**Sharath Ravishankar:** Okay.

**Harsh Singh:** So those things can right but custom content okay I I want these kind of prompts to run in

**Sharath Ravishankar:** Mhm.

**Harsh Singh:** my daily feed is not scope of v zero.

**Sharath Ravishankar:** Mhm.

**Harsh Singh:** So

**Sharath Ravishankar:** Okay. Okay. Understood.

**Pratik Bajaj:** also uh Manish and I I get it right like uh

**Harsh Singh:** yeah.

**Pratik Bajaj:** these use cases are also typically dependent on what maturity of client you are dealing with right if you are if you're dealing

**Harsh Singh:** Yeah.

**Pratik Bajaj:** with a store which is highly scaled versus a store which is trying to scale uh the use cases uh change quite a bit right uh and so so I'll I let me work with a

  
  

### **00:17:27**

  

**Harsh Singh:** Hello.

**Pratik Bajaj:** couple of more examples right and like I said I'm trying to bring this from my daily work

**Harsh Singh:** Mhm.

**Pratik Bajaj:** routine uh so just today this morning uh I asked Sharathto pull a report of uh my uh top 20 or or top 20% products which are giving me 80% of the revenue. Okay. uh everything from Meta 2 uh Shopifes I uh to return uh he created a quick report. Why I asked this report from him was if a particular variant is getting sold and not the other variant. I wanted to take a couple of quick decisions which is uh okay I want to show these other variants in the ads and maybe I want to create a collection in the store uh which is of similar products uh sort of thing right so these are decisions that I have taken now as a store manager I'm just working you with examples tell me how does that fit into something like this

**Harsh Singh:** Great.

**Pratik Bajaj:** because I'm assuming what you're showing me today is a pure play prototype and then the expectation is that we will work on one or two solid use cases to be implemented in vio.

  
  

### **00:18:55**

  

**Harsh Singh:** Right. So, uh just just give me a second. I'm just checking one thing. So, uh what you are talking about is kind of based on the SKU quadrant analysis, right? Which of my products are driving most of my right?

**Pratik Bajaj:** Yes. Yes.

**Harsh Singh:** So, again, this is a standard performance ad metric, right?

**Pratik Bajaj:** Okay.

**Harsh Singh:** Which people look at.

**Pratik Bajaj:** Add performance. Okay.

**Harsh Singh:** Yeah. performance. So we already have for example in routines inside Gavin there is a SKU quadrant analysis report which if you enable it already runs VT so this thing will be baked in right now there could be nuances to it okay so this product is driving let's say 80% of your sale but inside that product this particular variant is driving most of the sale

**Pratik Bajaj:** Okay.

**Harsh Singh:** and if it go and it should monitor okay this is going out of stock frequently or Sorry.

**Pratik Bajaj:** No, sorry. Go ahead.

**Harsh Singh:** Yeah. So again this particular use case should be there from day zero itself.

  
  

### **00:19:57**

  

**Harsh Singh:** Right. Any of the four from the performance marketing perspective right. So there is rorowass performance, fatigue detection, catalog health, scale quadrant analysis. These will be baked in from day zero itself in in the if the relevant connectors are connected and and again so one part is surfacing the signals itself right it might not be very deep dive that is you're not getting most value out of it but then at any point of time if you see okay this has caught your attention there is a chat with agent option you click on it and then you can deep dive into it.

**Pratik Bajaj:** Okay.

**Harsh Singh:** uh I don't know if you guys have tried the skew quadrant analysis and the catalog dash dashboard which has this

**Sharath Ravishankar:** Well, yeah. I'm already using that and I've also done an additive one on top of that. of using them.

**Harsh Singh:** okay yeah so but yeah those will be surfaced but uh again just to reiterate it might not be like very indepth the it will follow the current uh skill architecture where it will call out the products and all but for deep diving you can always go and chat with it and it will invoke the agent and you can deep dive but it will give you a high level overview and when you are in that pro mode view it will be there as part of the first column.

  
  

### **00:21:17**

  

**Harsh Singh:** Uh, does that answer your question, Pratik?

**Pratik Bajaj:** uh it does uh I'm just trying to connect the existing report that's there with the with the added performance or specifically from a Gavin point of view how does it uh give action that I can ask let's say Gavin to

**Harsh Singh:** Yep. Can you just open the left panel? So in fact uh just one sec uh this board view that you saw right we are I mean if you guys have suggestions around these are the default let's say five or 10 types of job that these agents should do or every day I would like to see I mean uh would like that suggestion because we are also trying to figure out what what are the right relevant signals to surface here for example creatives is kind of straightforward right we just look at your highest setting products or whatever there's a fatigue detection and we generate new c creatives we analyze your competitive brand ads and generate creatives based on that on perf it could be the standard same thing sk quadrant analysis roas dipping those kind of things do you have anything specific as let's we are calling it jobs to be done right in a way so which we should take care of as part of your feed which and that that will be available from day zero another thing is since this is a prototype and we are actively we will start developing it in a while.

  
  

### **00:22:49**

  

**Sharath Ravishankar:** Mhm.

**Harsh Singh:** So for the initial set of customers we are anyway going to create the feed. We will take that input from you. Okay, these are the specific things that I would like to see in my feed on a daily basis or on a weekly basis and the feed will be tailored accordingly. And just to add a small point to that the left panel contains all the existing surfaces that you're used to. So you can always access those chat with the agent to interact with them or directly go on the surfaces create your own routines and all of them ultimately just surfaces on one homepage which is the feed.

**Sharath Ravishankar:** Mhm.

**Harsh Singh:** Uh but it change every existing surfaces that you're already familiar with.

**Pratik Bajaj:** Okay. Uh, another one, right? Uh, let's say my CPM costs are increasing, right? Uh, it's a it's a signal. I'm assuming this falls right under let's say Gavin's uh this thing,

**Harsh Singh:** Yeah.

**Pratik Bajaj:** right? So, that's a signal. uh how can this entire feature what what should I expect in this feature if uh let's my CPM costs are increasing and we we have something that catches that uh specific to uh the ads uh or the products that's being run ads are being run

  
  

### **00:24:14**

  

**Harsh Singh:** It should show one of these posts as highlighting that as a problem and with suggestions or uh things or maybe actions that you should take or maybe some new uh routines it might set up and it'll ask you for your final approval whether you want to go ahead with that or remix it to create your own strategy around the problem that is being highlighted. So uh think again for example this card that you see right the initial card that you

**Pratik Bajaj:** Mhm.

**Harsh Singh:** will that will be surfaced here would be okay your CPM is dropping right and some delta

**Pratik Bajaj:** Mhm.

**Harsh Singh:** maybe based on the rolling window or whatever is the industry standard it won't it wouldn't have deep dived into it why it has got why is it dipping because we will be using cheaper models here we are going to provide the feed we are not going to charge any credit for it right so it will surface information in

**Pratik Bajaj:** Yeah.

**Harsh Singh:** in a way like it can have a let's say orange warning signal or something the UI could be set different for that whatever needs attention but it won't have a deep analysis why it is going down or anything I mean at least to begin with because that is going to consume a lot many credits and I

  
  

### **00:25:18**

  

**Pratik Bajaj:** Okay.

**Harsh Singh:** don't think we'll be doing that in the

**Pratik Bajaj:** Understood. Understood. But because uh we can run that broadspectctrum analysis at least a feed card will get created and it'll get shown to the user on the dashboard or on the seed and then it's about the user actioning upon it in terms of do I want to uh go deeper into it or do I want to simply kill it or implement it.

**Harsh Singh:** Yes.

**Pratik Bajaj:** Yeah, same thing I think goes with uh frequency above 4 years. So that's essentially your fatigue decision.

**Harsh Singh:** Yes.

**Pratik Bajaj:** And then uh do you want to rotate the creative? Okay, let's assume I'm doing a rotate creative, right? Uh sh this goes to our tof uh uh creative that we are currently rotating. Uh the underlining signal also was fatigue. At the same time, our uh cost of uh landing uh was increasing essentially,

**Sharath Ravishankar:** Mhm.

**Pratik Bajaj:** right? Uh so if I click on rotate creative over here,

**Sharath Ravishankar:** Okay.

  
  

### **00:26:26**

  

**Pratik Bajaj:** what happens next?

**Harsh Singh:** Okay.

**Sharath Ravishankar:** Okay. Great.

**Harsh Singh:** So if you click

**Sharath Ravishankar:** Yeah. So essentially in in my mind in for me as a user if I'm from what I can gauge from this. So it says okay fine it's giving me this information. It says rotate creative. Once I click on it it should give me essentially like what whether it's going to be create rotating the existing SKU creative whether it is fit. It needs to kind of decipher whether the fatigue is because or or based on what it's being shown to a lot of people or the same or the creative because how Andromeda works is it's image based creative based sort of algorithm that they're using. So if I say rotate creative, it's got to kind of figure out whether whatever is currently trending, it needs to give me suggestions based on or give me like two to three examples based on what creatives can kind of rotate it through or kind of replace it with to kind of reduce that fatigue within the same SKO

  
  

### **00:27:27**

  

**Harsh Singh:** Right.

**Sharath Ravishankar:** or variant of that same SKO or a completely different SKO all together.

**Harsh Singh:** Yes. s\*\*\*. So, uh more or less like exactly the same thing, right?

**Sharath Ravishankar:** Mhm.

**Harsh Singh:** Even today if you post a creative fatigue analysis, if you will ask the agent, right? Uh we in fact we have a creative pulse dashboard which shows you which of your ads are fatiguing and if you

**Sharath Ravishankar:** Yeah.

**Harsh Singh:** click on it it there are two three signals that it tries to look into. We have this meta ad library where we have analyzed a bunch of ads right it takes signals from there if you have added any competitors to look out for. It looks at their trending ads. It checks for what was what was the hook or anything. If it's a simple image ad there won't be any hook per se, right? There could be call outs depending on whether it's a catalog ad or a simple image ad. So it will analyze those two three things give you a list of suggestions or directions you pick it will generate two three samples basically it will be a chat based flow right so a couple of turns to get to that creative but yeah those things will be taken into account what is trending the analysis repo that we have of around 50,000 ads in our system today those things

  
  

### **00:28:35**

  

**Pratik Bajaj:** Okay. Uh could you Oh, okay. Storefront. Uh uh can can we look at catalog level uh recommendations or catalog uh panel?

**Harsh Singh:** uh that will be there. I I guess one of the recurring issues you guys have been facing is with the catalog or the Shopify manager. Uh so we are making changes there. Like I I had told Shah that last time also we had updated all our other agents but this was this one was not updated but uh once that is done uh it should be better but are you guys can you looking for some specific signals that should be surfaced out right for example it could be things like uh the SEO tags are missing on these products right or this product was your highest selling product last month but it's out of stock for let's say 20 days this month so those kind of signals it it will surface. But again uh this is just top of my head. If you have any suggestions here since you guys actively manage stores so that would be helpful.

  
  

### **00:29:42**

  

**Pratik Bajaj:** You know I uh I think in general uh with the first one is landing page to part uh basically moving from consideration to convert. conversion, right? So, landing page to add to cart is uh one of the strongest signals we use to change uh the catalog, right? Uh now that what to change on the catalog at this point in time is primarily a stylist driven or a catalog manager driven decision. uh whether whether they want to add new imagery, whether they want to uh add or replace imagery, whether they want to change the copy. Uh but the primary signal that we are looking for is uh uh at this point in time uh landing page to uh add to car uh what you are talking about the SEO tags uh that I generally consider as hygiene. ethic hygiene, right? Like why is the SEO tag or SEO metatitle missing?

**Harsh Singh:** Right. No, this is a fair call out. So, conversion metric, right? So, if you uh Shopify is connected, Shopify exposes its own analytics.

  
  

### **00:31:06**

  

**Harsh Singh:** On top of that, if GA is connected, so those signals will be mixed, right? I should have called it or I have noted it down also. conversion metric will be one of the northstar metrics for storefront I guess across the board. So that that will keep it in mind.

**Pratik Bajaj:** Okay. And as I mentioned right the the so look look at it this way. This is one of the things that I wanted to discuss with Shobhitas well as a uh as a utility that I could use. Right? So we are there is no keyword research module at this point in time within shops. Right? Uh now the keyword research essentially helps in uh two three areas. One is intentbased purchase which is directly on my catalog pages. Am I essentially using those on indexed fields? Uh at the same time it helps me with my big head level decisions on the visibility aspect as well. Right. Uh so that for me is more like a hygiene model that okay is there something that is outside the store trending can I can I bake that into my uh non-performing uh cataloges or non-performing listings enrich those listings and then make them live again that's the workflow we typically follow uh for uh our uh listings with our clients

  
  

### **00:32:39**

  

**Harsh Singh:** Yeah. So Pratik I'll be honest here like uh keyword and SEO is not on the pipeline at least for next couple of months when it lands.

**Pratik Bajaj:** So what visibility here

**Harsh Singh:** So visibility is mostly around AI and GEO visibility. It will uh it once we extend to SEO then we will have the keyword manager and everything in the suite right now any changes or major changes that will come would be around creative per and Shopify store manage I mean on the store manager it's more about stability because internally we have all the hooks and everything in place we just need to stabilize that platform on the visibility bit the focus or at least the geo tool has been built out and at least

**Pratik Bajaj:** Sure.

**Harsh Singh:** till October end I don't see us moving into SEO or keyword management But yeah, if we get the bandwidth, we'll be happy to pick it up.

**Pratik Bajaj:** Okay, fair enough. uh uh how how do we proceed like what what is your expectation from us at this point in time if if you could name some

  
  

### **00:33:48**

  

**Harsh Singh:** I mean there there are a couple of things. One was to get the feedback itself. Do you think this will be useful for you guys if you get such a view? Right. First is that second for your feed what are the primary items that you would like to look for so that when we roll it out your feed is tailored accordingly and you start getting value from day zero. So basically the jobs to be done by different agents on a daily basis.

**Pratik Bajaj:** Understood. Uh I think from a utility point of view and how useful could this be? Uh I I would probably say it's in the right direction. As you mentioned that a whole lot of things depends on uh what we what a user does. Let's say after they see something like this, right? So it's a it's a game of uh okay Shhat is the user Shhat is getting these uh feeds because it's extremely important for him and his job right whereas uh Smithy is another user in my team uh she's getting a feed which is more on the creative side of things right whereas Shhat is getting more on the performance side of things or Pratik is getting more on the storefront uh CRO related conversion rate related things But the flow is promising that okay give me a signal based feed.

  
  

### **00:35:16**

  

**Pratik Bajaj:** Let me take an action basis that and uh whether this is coming from our existing analysis or the new jobs that you will that we could take in it's useful which jobs it's making sense for us today. I sharat and I will sit and work out five jobs uh from our side. uh right from signals to what we expect in the feed to what possible downstream actions are expected. Would that help?

**Harsh Singh:** Yeah, that would be super helpful. Uh just one call out here. Uh so currently the feed itself is workspace scoped. Uh, But uh it's a fair call out.

**Pratik Bajaj:** No, that's understood.

**Harsh Singh:** I mean you have multiple teammates. One might be creative focused, another might be more per focused. So they can hide their individual feed to show less of perf right. But overall generation is on a workspace level itself that

**Pratik Bajaj:** Yeah, that's understood. And even I want it that way because if If Sharathis working on client A, he wants to take decisions on that client A and tomorrow if we want this entire thing to be used by the client, they are only interested within their workspace.

  
  

### **00:36:35**

  

**Pratik Bajaj:** Right? uh so I'm anyway have been requesting uh bum and uh the development team hmon as well to have my workspace sorted only from a point of view of uh credit usage and credit sharing whereas the workspace is dedicated to a particular client that's how I I would also like to use the

**Harsh Singh:** Yeah, it it is that way. I mean the memory everything is workspace scope. I guess one of the ask from you guys was to share credit across workspaces, right?

**Pratik Bajaj:** Correct.

**Harsh Singh:** So that is also there now.

**Pratik Bajaj:** It's not there.

**Harsh Singh:** Uh I just wanted to call out sorry.

**Pratik Bajaj:** Okay. It's not there. Are you responsible for that? Then I would like to showcase something to you. If we are done with this conversation,

**Harsh Singh:** Yeah.

**Pratik Bajaj:** then we'll proceed to that. But it's I'm still struggling with uh uh allocating uh credits to a particular workspace.

**Harsh Singh:** Yeah, we can go through it. Uh so we'll wait for like maybe four or five

  
  

### **00:37:38**

  

**Pratik Bajaj:** If

**Harsh Singh:** jobs each for different agents, right? That you guys like like to have but yeah from our side we are done. We can move to that thing. Please let us know what you're facing.

**Pratik Bajaj:** noted, noted. I will uh I will have this uh shared in a couple of days uh to you guys. I'm hoping that it helps both of us from there.

**Sharath Ravishankar:** Yeah, but I do like the way this feed is from the the way the dashboard is looking along with actionable uh things within it. Um it's a nice it's a nice fresh look on the overall aspect of what um top can do on all fronts.

**Harsh Singh:** Glad to hear that.

**Pratik Bajaj:** Okay, I'm sharing my screen. Uh, so this is my primary workspace, right?

**Harsh Singh:** Good.

**Pratik Bajaj:** Uh, I have credits on this workspace. Uh, I also have users added into this workspace. Okay.

**Harsh Singh:** Okay.

**Pratik Bajaj:** Uh now uh there point taken. Is this how it is?

**Harsh Singh:** Yeah.

  
  

### **00:39:20**

  

**Pratik Bajaj:** So available once this workspace is on paid theme.

**Harsh Singh:** Okay. You have a custom plans. It's not one of our primary plans. Uh I'll get this fixed today. I'll update you. So once this is fixed, basically you can add the workspace from here.

**Pratik Bajaj:** Huh?

**Harsh Singh:** And the other Mhm.

**Pratik Bajaj:** So how how I see it is the point taken workspace which is an agency workspace will have that itself will work like a workspace because for example if I'm doing one-time generations for clients whether it's videos or images or whatever it is I don't need to create a deep dive uh workspace with their memory etc etc into but if a client gets into a routine work with me which is more like a retain

**Harsh Singh:** Wait.

**Pratik Bajaj:** container work from with me which is across their catalog, storefront, ads, geo doesn't matter then I will create a workspace for them right so right now I have two major workspaces I have uh one which is monzen mars which I just created which is not on a paid this thing and then there is Sharath'sworkspace which we converted into uh uh like that euthnic uh workspace But

  
  

### **00:40:33**

  

**Sharath Ravishankar:** You think so expression?

**Pratik Bajaj:** uh so as a primary thing uh whatever credits eventually I will purchase the credit as an

**Harsh Singh:** There you go.

**Pratik Bajaj:** agency and then however I want to distribute it across users reserve his uh workspace that's sort of is is on me at least that's what I would like to achieve

**Harsh Singh:** Right. So uh basically uh this point taken workspace that you have right where you have the plan you can add the workspaces with which you want to share the credit and plan. This blocker will get it sorted today itself because it works on normal plan just the custom plan it's not working. So but yeah after that you can share this clan with mons and mars and any other if you want now individually in those workspaces you can go I mean the same member can be part of multiple workspaces right so inside different workspaces you can give the members different credit limit that he should be able to use 2,000 in this workspace and let's say 3,000 max other workspace so those things are

  
  

### **00:41:28**

  

**Pratik Bajaj:** Yes. Yes.

**Harsh Singh:** configurable one thing which is missing is let's say you have a credit pool of 20,000 you can't distribute that among the workspaces itself. Give 10,000 credit to this workspace. That is not possible today.

**Pratik Bajaj:** Okay. All right. That is not possible.

**Harsh Singh:** Yeah.

**Pratik Bajaj:** Fair enough. Any particular reason of restricting that?

**Harsh Singh:** Uh no, it was just not scoped out. Well,

**Pratik Bajaj:** Fair enough. No, I I get it and I'm assuming that it's not too many agencies that you're currently working with, which yeah,

**Harsh Singh:** It was just built for you guys and then we didn't uh so

**Pratik Bajaj:** I and I'm I'm very happy from that context. It's just a requirement. I'm very I I know that I will request you guys and get some of these things done. So that should not be a challenge immediately.

**Harsh Singh:** yeah perfect. So we'll drop a text in the WhatsApp group once this is sorted.

**Pratik Bajaj:** Perfect. while while we are on the call and considering this is Gavin specific team right uh I do want to cover a few feature drops that happened in the last couple of weeks I don't think so we went through it either uh this has got to do with the the signals primarily

  
  

### **00:42:42**

  

**Pratik Bajaj:** on meta ads library or being able to track a few few other brands so if you can give us a quick rundown of uh uh new features let's say that came on Gavin in the last two weeks that or any other region

**Harsh Singh:** Yes. So, we'll let answer that one.

**Adarsh Mishra:** Yep. Um, can you see my screen?

**Pratik Bajaj:** Yes.

**Adarsh Mishra:** Yes. Okay. So, I think firstly I'll start go top to bottom. No specific order. Um into in the inspirations what we have done is um initially we had added meta ad library which you had already seen um where we you can add a competitor either by searching the domain or the brand name and based on that you can add competitors for example here I've added offduty India and wild oak boutique so I'll be seeing ads these brands are running over here um from the meta ads public library so you can search for any competitor here add them and see their ads which they are running publicly. So for example these ads are being run by OBD2 India.

  
  

### **00:44:19**

  

**Adarsh Mishra:** Similarly you can switch to wild look and you'll see the ads wild look is running. Similarly you can search via the keywords as well if you don't want to search by a specific um competitor and certain filters. This I think something we went through already. What we have additional here that is new is let's say you um see this ad you like it you can click on it and there is an option to analyze the ad um yeah so you you get more details about this and once you do the analysis for the ad that all the ads now come to this Tropical. is analyze tab uh which is here. So every analysis that is done in meta ads library can be done by any brand any workspace across shoppers. Um everything comes over here and gets collected and it gets segregated by multiple filters based on the category of ads which we have um

**Pratik Bajaj:** Wow.

**Adarsh Mishra:** yeah

**Pratik Bajaj:** So this is this is like a universal repository for

**Adarsh Mishra:** correct.

**Pratik Bajaj:** Okay.

  
  

### **00:45:26**

  

**Adarsh Mishra:** So let me just switch to apparel or something. Yeah. So let's say I switch to apparel. Then I can have choose by media type it. And if you go further down because each ad is run through an AI and it's being analyzed, it's broken broken down into what format it is, what sort of ad it is. Um sorry and then um broken down on what the hook is in this. We have certain categories predefined. it automatically classifies the ad into certain um category of let's say hook or format or whatever it is. Similarly, the funnel stage and um awareness level for the same. So each and every ad that analysis is done on it automatically get categorized. So you can easily filter and find ads for you to clone or copy or whatever. So now let's say these are analyzed ads. So if you open any of the ads that is analyzed, let it be a video ad or an image ad um it gives you a breakdown of the ad on um everything like the color palette, what you can borrow from it, what you should not borrow from it, which would which is specific to that brand.

  
  

### **00:46:34**

  

**Adarsh Mishra:** Um and if I open something which has let's say yeah this this video ad if I open it also like transcribes the entire video ad. It uh summarizes the frames and you can see like what the hook was, what the setup was and everything. It it breaks down the entire ad. Um yeah so these this detailed analysis you can utilize for seeing what works, what doesn't work. Um and if you let's say like a ad all the image based ads as of today um have an option to remix them. Uh the videos don't again but the image base do. So you can click on remix and it will open it in a chat and from that particular chat you can get the same ad in the same exact format for your brand with your brand memory.

**Pratik Bajaj:** Just out of curiosity,

**Adarsh Mishra:** So that Yeah.

**Pratik Bajaj:** just out of curiosity, are we are we when you say remix, are we handing it over to like Mika or this is a completely different channel?

**Adarsh Mishra:** Can you can you go again?

  
  

### **00:47:34**

  

**Pratik Bajaj:** Just out of curiosity this question is when you say remix does it get hand over to a specific agent like Monica or is it just some prompt instructions uh uh working

**Adarsh Mishra:** Yeah, it gets handed over to Monica actually.

**Pratik Bajaj:** All right.

**Adarsh Mishra:** Yeah, with some specific prompts passed to it on how to use this ad for your generation. Yeah. So there is definitely a skill there which guides on how to remix this.

**Pratik Bajaj:** Just

**Adarsh Mishra:** Um, but Monica is the agent which drives the remix of it. So if I just go ahead and remix this, it'll ask me if I want to use my brand memory, my pawns or not, what product I want to use. All of these questions are asked and based on that, the final remix is created.

**Pratik Bajaj:** we'll try this out.

**Sharath Ravishankar:** Yeah,

**Adarsh Mishra:** Yeah.

**Sharath Ravishankar:** I'm keen on trying this one out. This is interesting.

**Adarsh Mishra:** Sure. Yeah. So that is how like I mean we what we did is we already went ahead and took like around 24,000 ads including 14,000 videos and a mix of carousels and static images as well and we have analyzed them all already.

  
  

### **00:48:34**

  

**Adarsh Mishra:** So if I just clear the filter you'll see like uh we have like around 20 22,000 ads over here which are filtered out based on brands and uh different categories and everything. So and as and when each and every brand or which is onboarded onto shop OS uses the meta ads library as well to find their competitor ads analyzes it our library keeps expanding as well. So the agent when you talk to it uh it has a context about the analyzed ads analysis we have. So if you ask it like what is the common pattern between XYZ type of ads. So it can look at the analysis um we have stored and it can give you suggestion based on that as well.

**Pratik Bajaj:** How are these uh um ads right now? Like see as a once again from a user experience point of view as an agency this is fantastic. Okay, 22,000 uh analyzed ads. But the moment I give this to a brand uh to sift through, right, they will be like why would I be doing something like this?

  
  

### **00:49:41**

  

**Pratik Bajaj:** Uh so consider it as a feedback or whatever however it is.

**Adarsh Mishra:** So,

**Pratik Bajaj:** But I know this is still in the initial things and the idea is to kind of improve

**Adarsh Mishra:** one thing that

**Pratik Bajaj:** upon the end user experience as well, right?

**Adarsh Mishra:** yes, for example, let's say you're a nutrition brand, right? You don't really have to go through the entire ad set. I mean one of the ways of using it is you don't have to go through it. You just come to the chat you say okay I'm planning to do generate a new ad creative what are the trending hooks in this category it will already go through we have all this data stored the

**Pratik Bajaj:** Okay.

**Adarsh Mishra:** agent will comb through it give you the feedback okay these are the trending things or these are the kind of books that that we see working which one do you want to proceed with so you don't really have

**Pratik Bajaj:** Done. No,

**Adarsh Mishra:** to

**Pratik Bajaj:** this is this is this is definitely useful.

  
  

### **00:50:34**

  

**Pratik Bajaj:** uh we'll we'll we'll give this a shot.

**Sharath Ravishankar:** Mhm.

**Pratik Bajaj:** We'll get back with the uh feedback on this as well.

**Adarsh Mishra:** Okay, sure. Um I think apart from that a creative pulse is something that we did go through um last time

**Sharath Ravishankar:** Uhhuh.

**Adarsh Mishra:** but I think you wanted to go through it yourself and get back with questions right?

**Sharath Ravishankar:** Yeah. So, I I think I did the creator pulse and I set it up um and it's

**Adarsh Mishra:** Yes.

**Sharath Ravishankar:** uh and it's given me like a graph and and and a whole lot of things. I just need to kind of go through it. It obviously says there's no fatigue. It's telling me shows me what the top competitors are, top performance performers are etc.

**Adarsh Mishra:** Yeah,

**Sharath Ravishankar:** And it gives me bench line or like okay what's the current thing now again this is a dashboard right now I'm Oh yeah

**Adarsh Mishra:** right.

**Pratik Bajaj:** Can you bring it up? Can you bring it up if it's already set?

  
  

### **00:51:26**

  

**Sharath Ravishankar:** sure. getting my screen.

**Adarsh Mishra:** So while you share I'll just add to it that while this is a dashboard all the context that is there

**Sharath Ravishankar:** Yeah. Mhm.

**Adarsh Mishra:** here that is what are your top performers what is fatiguing and each and every ad that has been analyzed over

**Sharath Ravishankar:** Mhm.

**Adarsh Mishra:** here let's say I open this video and um if I go to full analysis and if this this if I analyze this ad um once the analysis is done it is stored in the database and agents do have the context about the analysis.

**Pratik Bajaj:** Okay.

**Adarsh Mishra:** Yeah.

**Sharath Ravishankar:** Thank you.

**Adarsh Mishra:** So you can then utilize it when let's say you are talking about the top performers um in the last two weeks. You can ask the agent that what was working for me in the last two weeks what was not working and this

**Sharath Ravishankar:** Mhm.

**Adarsh Mishra:** analysis which you did over here is available with the agent. So it can look at that analysis uh the creative breakdown what worked what did not and if you ask it for suggestions like what sort of creative I can try next based on this based on the improvements it can suggest it'll give you in the chat so I think even currently the team apart from analyzing the ad and looking at um what's working what's not for a single ad the team has been actually using this part internally as well that um in general what works so they go ahead and select let's say a

  
  

### **00:52:44**

  

**Adarsh Mishra:** 14-day timeline over here that is the last two weeks when the ads were being run for a new creative and they see what worked what did not and the test next which is there it gives some suggestions on based on what was working on what the team can try next. So internally as well this is something that is being used right now

**Pratik Bajaj:** What?

**Sharath Ravishankar:** So essentially this section is my potential recommendations that is it's given on top of on top of on top of these recommendations like scale

**Adarsh Mishra:** Yes. No, no. If you scroll down,

**Sharath Ravishankar:** and other things. Yeah.

**Adarsh Mishra:** so all of these which you see apart above what's working and needs attention. Um everything above that is based on your data and what's working needs

**Sharath Ravishankar:** Mhm.

**Adarsh Mishra:** attention in tests. All of these are based on AI analysis and signals on what actually like which did an analysis of your ads in that particular period and it's giving you suggestions.

**Sharath Ravishankar:** Okay.

**Adarsh Mishra:** Yeah. And if you open a specific ad and you do a full analysis that is again based on Yeah.

  
  

### **00:53:49**

  

**Sharath Ravishankar:** Mhm.

**Adarsh Mishra:** Anything above that, it's based on the metrics you set for your ad to um be called a qualified ad or not. It it categorizes into top performers, fatiguing, etc., etc.

**Sharath Ravishankar:** I'm sorry.

**Adarsh Mishra:** So, you can go and pull analysis for this ad. For example, I think these are if um just go ahead and full analysis and yeah, it is now doing an AI analysis. It's a video. If you scroll up, I think um yeah, so for video ads, it also has the data from meta is where the users are dropping off, how how much percentage of the video is being watched and all of this.

**Pratik Bajaj:** What's Yeah.

**Adarsh Mishra:** So all that you can see, you can understand if the hook is working or not. Yeah, if you see this and if you do the read the script as well, it it transcribes certain frames of uh your video, it was uh right above this section.

**Sharath Ravishankar:** right above here.

**Adarsh Mishra:** Yeah,

**Sharath Ravishankar:** Read the script.

**Adarsh Mishra:** just correct.

**Sharath Ravishankar:** Okay.

  
  

### **00:54:59**

  

**Sharath Ravishankar:** All

**Adarsh Mishra:** So it takes certain frames,

**Pratik Bajaj:** Yes.

**Adarsh Mishra:** it transcribes it and also analyzes that what was happening over there and where the users are dropping off. So it breaks down your creative based on the data which is there and gives you an understanding is where the users are dropping.

**Sharath Ravishankar:** right.

**Pratik Bajaj:** Okay. All right.

**Sharath Ravishankar:** Okay.

**Pratik Bajaj:** Fair.

**Sharath Ravishankar:** Good.

**Pratik Bajaj:** Uh, anybody from the big head team also over here by any chance?

**Adarsh Mishra:** Not right now.

**Pratik Bajaj:** Okay, no worries. Well, thanks for this. Uh, I think we needed to see a couple of I think there are a couple of more features on the big

**Sharath Ravishankar:** Yeah,

**Pratik Bajaj:** side of business.

**Sharath Ravishankar:** I just I like the like uh I like the new feed format to be honest. I quite like it.

**Adarsh Mishra:** You guys have another call tomorrow,

**Sharath Ravishankar:** Um we have another call tomorrow.

**Adarsh Mishra:** right?

**Sharath Ravishankar:** Uh I think it's from 1 to 2.

**Pratik Bajaj:** So Madur is also asking for when to set up the

  
  

### **00:56:07**

  

**Sharath Ravishankar:** Yeah. Yeah. So I I was now my question is um we have we can do the demo tomorrow.

**Adarsh Mishra:** Thank you.

**Sharath Ravishankar:** Uh we have a call one to two if we don't have a lot to cover during that period of time. We can kind of overlap it with that and and this but I'd rather keep like one a good an hour

**Pratik Bajaj:** All

**Adarsh Mishra:** Sure.

**Sharath Ravishankar:** at least for this session. So probably like two to three or something like that.

**Adarsh Mishra:** I'll ask Shobhitto set up a call for two to three with and the

**Sharath Ravishankar:** Okay.

**Adarsh Mishra:** developer who works on this.

**Sharath Ravishankar:** Okay. Check.

**Adarsh Mishra:** Yeah.

**Sharath Ravishankar:** Yeah.

**Adarsh Mishra:** Okay.

**Pratik Bajaj:** right guys, just last note I know there is conversations on Slack that is happening uh as well from Shhat and our side primarily Shhat What we are doing is we are ensuring that we are keeping the slack channels.

**Adarsh Mishra:** Sure.

**Pratik Bajaj:** is updated uh in terms of our requests just just putting the information out there and WhatsApp we are keeping it more as a immediate conversation if something needs immediate attention or something

  
  

### **00:57:14**

  

**Adarsh Mishra:** Okay. By the way, Sharath,in case um you missed the chat, I have already added MS clarity on the tool. So,

**Sharath Ravishankar:** Oh, you have.

**Adarsh Mishra:** you can go ahead and connect it.

**Sharath Ravishankar:** Okay,

**Adarsh Mishra:** Yeah,

**Sharath Ravishankar:** perfect. Okay,

**Adarsh Mishra:** you can go ahead and connect it and see if it's helpful or not and like the feedback if something else is needed.

**Sharath Ravishankar:** I will I will connect it and uh see how that goes. Sounds good.

**Adarsh Mishra:** Sure. Yeah. And also like um the bug you were getting with the um report right. I think the next report when it runs just please do let me know so I can compare because I fixes um and

**Sharath Ravishankar:** Uh available. Mhm.

**Adarsh Mishra:** it should probably reflect and you should not see that issue anymore of um zero yeah zero copy or pixels not firing etc.

**Sharath Ravishankar:** Yeah. Yeah. Yeah. Okay.

**Adarsh Mishra:** Sure.

**Sharath Ravishankar:** Sounds good.

**Adarsh Mishra:** So both of them are there.

  
  

### **00:57:56**

  

**Adarsh Mishra:** Um just let me know if you surface any other issues like

**Sharath Ravishankar:** Yeah. And the the other thing is again uh same thing, right?

**Pratik Bajaj:** Okay.

**Sharath Ravishankar:** It's the inconsistency of what the data is showing versus what it's saying is is is kind of changing a lot about a lot. For example, I'm just sharing my screen quickly here. Now you can see here I pulled a I pulled like a product report sort of thing over the last 30 days. Okay. So this one's giving meta purchases.

**Adarsh Mishra:** This

**Sharath Ravishankar:** Yeah I I pulled it out. I I copy pasted the info here. You can see here the meta purchases of this particular SKU is at 53 and Shopify purchase at 42. Now I can see here Shopify purchase is 57 meta is 39 for the same product and the same period of time. And this is within the same chart.

**Adarsh Mishra:** actually the data in in terms of attribution right like I it it's not going to match if you look at two sources because the way they track is always different for example I think this was something I got to know as

  
  

### **00:58:53**

  

**Sharath Ravishankar:** Okay.

**Adarsh Mishra:** well yesterday from uh one of our performance yeah so let's say you're checking

**Sharath Ravishankar:** What do you mean by what do you mean by two sources?

**Adarsh Mishra:** the purchases on meta or any uh

**Sharath Ravishankar:** No, no, no, no. I'm talking about I'm talking about Okay. between meta. This is 53 for the same product. Okay. 53.

**Adarsh Mishra:** right

**Sharath Ravishankar:** The same product 39. It's giving me two different numbers.

**Adarsh Mishra:** and This is from now can you tell me the data sources for

**Sharath Ravishankar:** It's giving me two different numbers.

**Adarsh Mishra:** them like it's both meta I understand and same products is giving two numbers but it's two different data sources right

**Sharath Ravishankar:** No, this is Gavin.

**Adarsh Mishra:** one is

**Sharath Ravishankar:** It's Gavin for both within the same chat. I think it is this one.

**Adarsh Mishra:** so within the same

**Pratik Bajaj:** And here are the data in well validated as well.

**Sharath Ravishankar:** It's this chat. Yeah. So this is this is within. So I said okay give me like a a product uh product funnel thingy ver I said verify report again.

  
  

### **00:59:50**

  

**Sharath Ravishankar:** So it told me um re I said revisit line 23 for example here this particular product here it shows me that uh Shopify purchases meta purchases checkouts and shows that check out to purchases but it's there's a difference between Shopify and meta purchase obviously I understand that now it's showing me 75% here but then if I go back to this and I asked it the question but it's recorded zero purchases it said okay yeah this is let me read the exact data shop for purchase that is it's correct for that one but it's not correct for this one understood So it says it's a noise artifact. It should not be considered as basically what it says. It's basically meaningless and should not be should have been flagged rather than highlighted as a proven closer.

**Pratik Bajaj:** the the idea.

**Sharath Ravishankar:** So I'm trying to figure out what with what to do with this information too.

**Pratik Bajaj:** Uh did did you understand what's happening over here?

**Sharath Ravishankar:** Yeah, it's giving me it's giving me a percentage data for only one of them versus the other one.

  
  

### **01:00:58**

  

**Sharath Ravishankar:** It's not giving me a percentage data is what I'm thinking.

**Pratik Bajaj:** Sorry guys. Uh I was asking the top team like did you get a context of what what's

**Adarsh Mishra:** No, no,

**Pratik Bajaj:** happening?

**Adarsh Mishra:** we are trying to make u get an understanding of it. Just

**Pratik Bajaj:** We are highlighting this only from a uh okay like should we trust uh the information that's getting pulled out right uh at this point in time we are doing very similar activities using claude as well as uh cloud-based connectors for Shopify as well as uh meta right so these these conversations are happening over there as well uh but just giving you a context that if something like this comes it it it throws us off our uh conversation flow and then trusting the decision or trusting the information shown over here uh becomes a little uh tricky

**Sharath Ravishankar:** shaky.

**Adarsh Mishra:** Yeah. And further in this chat, it showed a different number for the same product.

**Sharath Ravishankar:** So here so I so this is come back to this. So this I I said revise the whole thing and re redo the report again.

  
  

### **01:02:18**

  

**Sharath Ravishankar:** So it gave me this. So basically this sheet here is me. This is the first uh report and this is the second report that I pulled that I pulled from it. Now all of these are catalog ads not image ads. So for me, so for me I will have to kind of go to my meta meta performance manager, break it down by product ID and then do a lot of that math accordingly. Like even here the spend is 7,700 and here it's showing me spend 12,800. Now, for me to verify this, I will need to do a bunch of manual work, which is fine. understandable verification requires manual work but there's a stark difference between these two numbers and my thing is I'm just trying to figure out like I don't know like which one do I trust between the two which one is closer to the accurate um if if I don't verify a lot of customers don't a lot of other brands or users don't verify this they're going to be making business decisions based on wrong information

  
  

### **01:03:30**

  

**Adarsh Mishra:** Can you scroll up once again? What was the click count?

**Sharath Ravishankar:** 2708 the range

**Adarsh Mishra:** It looks like a completely different date range to me. Yeah.

**Sharath Ravishankar:** is very different exactly like add to cards sorry date range is

**Pratik Bajaj:** No, no.

**Adarsh Mishra:** No,

**Pratik Bajaj:** The date range the date range. What is

**Sharath Ravishankar:** the same date range is the same it's last 30 is

**Adarsh Mishra:** do you mind sharing u the the sheet the date range which you used and the chart so that we can

**Sharath Ravishankar:** I I'll share I'll share the entire chart with you.

**Adarsh Mishra:** analyze like Yeah.

**Sharath Ravishankar:** So I'll just double check that for me as well.

**Adarsh Mishra:** because sometimes what happens is that like I mean it's sometimes the LLM behavior itself I

**Sharath Ravishankar:** Mhm.

**Adarsh Mishra:** I don't want to just put it onto the LM I know it's it's our system but um what it does it it

**Sharath Ravishankar:** Yeah. Yeah. Yeah.

**Adarsh Mishra:** attacks lazy sometimes and when it that okay I have to fetch 20 different pages what I'll do is I'll

  
  

### **01:04:15**

  

**Sharath Ravishankar:** Mhm.

**Adarsh Mishra:** just fetch this much and I'll give the user and I'll see so sometimes all of the all of that goes into

**Pratik Bajaj:** Correct.

**Adarsh Mishra:** the thinking blocks and it is it is not surfaced to the if

**Pratik Bajaj:** What's your underneath model? What's the underneath model we are using over here?

**Adarsh Mishra:** if you were on the auto mode. It might have been using Claude Sur 4.6 for this one.

**Pratik Bajaj:** Donnet 4.6 is what you're using, right?

**Adarsh Mishra:** Yeah.

**Pratik Bajaj:** That's so a a subtle difference around this is obviously I'm using a higher model on cloud right now for similar set of activities right so uh I understand completely where you're coming from that's why we are citing it more as a uh my confidence to take decisions based on agents recommendation because I get it if you use a

**Adarsh Mishra:** Right.

**Pratik Bajaj:** higher model uh with a better uh context maintenance with a better uh uh reasoning capability uh these these these will be a lot more different right as answers these will be a lot more different but that's that's for you to decide how how you will optimize or correct it uh cuz I get it it may have just changed the data for the first look that is what my question to sh was as well is that has the data changed

  
  

### **01:05:28**

  

**Adarsh Mishra:** Yeah, because we are also guessing that because even the clicks and the views every metric is like quite smaller in the second one and like bigger. So um can you uh sh can you go back to the chat once on the right side you see sub aents right can you hover after that sub

**Sharath Ravishankar:** Yeah.

**Adarsh Mishra:** agents can you hover over the performance yeah click on that uh click on performance quantities returns it won't show the thinking here thinking thinking for the I mean there is the um is

**Pratik Bajaj:** I I I I thought shop I thought Claude in general General stop showing thinking or is that only work that the shop think?

**Adarsh Mishra:** no no actually some models some models do um they just hide it once the response is given actually let me add we can see it in the app shared

**Pratik Bajaj:** Okay.

**Adarsh Mishra:** right yeah yes we can have just we have the ID lang we'll check this and get

**Sharath Ravishankar:** Mhm.

**Adarsh Mishra:** back yeah Okay,

**Sharath Ravishankar:** Yeah, sure. Let me know.

**Pratik Bajaj:** Share the chat. Yeah.

**Sharath Ravishankar:** I have I have I'll share it in the in the in the call chat right now.

**Adarsh Mishra:** sure. Thank you so much.

**Pratik Bajaj:** Okay guys, hoping this time was useful for both of us.

**Sharath Ravishankar:** Yeah. Yeah.

**Pratik Bajaj:** You will guys will get the uh the list of job ids from our side. Uh I'm looking forward to building this uh because especially because I have a new client uh that I want to get on board uh and set up those things for the client, right? Uh so I'm I'm looking forward to the next uh four to five weeks on this new features in

**Sharath Ravishankar:** Okay,

**Adarsh Mishra:** Perfect.

**Sharath Ravishankar:** awesome. Thanks,

**Adarsh Mishra:** Okay.

**Sharath Ravishankar:** guys.

**Adarsh Mishra:** Thank you for your time.

**Sharath Ravishankar:** Thank you. Thank you.

**Pratik Bajaj:** Thank

**Sharath Ravishankar:** Cheers.

  
  

### **Transcription ended after 01:07:40**

  

*This editable transcript was computer generated and might contain errors. People can also change the text after it was cre
# Awesome-Sales-Prospecting-SDR-Workspace

## Top Sales Prospecting & SDR Workspace Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Multi-Channel Outreach, Lead Enrichment & Self-Hosted Sales Engagement*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Sales Prospecting & SDR Workspaces**. These tools enable sales development teams to find leads, enrich contact data, run multi-channel sequences (email, LinkedIn, WhatsApp), and manage replies in a unified inbox—turning outbound from a manual grind into a measurable, scalable engine.



**Examples** include HubSpot Prospecting Workspace, Apollo.io, Outreach, Salesloft, ZoomInfo Engage, Groove, Mixmax, Lemlist, Reply.io, and Close (the category leaders).



**Open-source emphasis**: Sales Prospecting & SDR Workspaces is a domain where open-source tooling has **matured rapidly and now offers genuinely viable self-hosted alternatives to commercial sales engagement platforms**. **AgentSDR** is the standout—an MIT-licensed, self-hosted AI SDR that runs email sequences from your own Google Workspace mailboxes, LinkedIn campaigns via Unipile, and WhatsApp messages/calls, with an AI CRM that classifies replies and drafts answers for human approval . **Pigeon** focuses on cold email deliverability with mailbox warm-up, inbox rotation, and automated DNS configuration . **OpenCRM** provides a self-hosted CRM with lead automation, AI email generation, and kanban pipelines . The critical caveat: **open-source SDR tools require you to supply the lead data**—they are not bundled with Apollo/ZoomInfo-scale contact databases, so you pay for enrichment APIs (Apollo, Hunter, Lusha) separately .



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[HubSpot Prospecting Workspace](https://www.hubspot.com/)**  

  Lead prospecting within HubSpot's Sales Hub; contact and company records, email tracking, sequences, and meeting scheduling tied directly to CRM data.



- **[Apollo.io](https://www.apollo.io/)**  

  The leading all-in-one prospecting platform with a massive B2B contact database, enrichment, email sequences, and dialer; the benchmark for lead data depth.



- **[Outreach](https://www.outreach.io/)**  

  Enterprise sales engagement platform with multi-channel sequences, conversation intelligence, and revenue intelligence analytics.



- **[Salesloft](https://salesloft.com/)**  

  Sales engagement platform with cadences, dialer, and coaching tools; positioned for enterprise SDR teams.



- **[ZoomInfo Engage](https://www.zoominfo.com/)**  

  Sales engagement within ZoomInfo's data platform; sequences, dialer, and enrichment backed by ZoomInfo's contact database.



- **[Groove](https://www.groovehq.com/)**  

  Sales engagement platform for Salesforce and Gmail/Outlook; sequences, auto-logging, and meeting scheduling.



- **[Mixmax](https://www.mixmax.com/)**  

  Email engagement platform with sequences, tracking, scheduling, and polls; positioned for individual reps and small teams.



- **[Lemlist](https://www.lemlist.com/)**  

  Cold outreach platform with multichannel sequences (email, LinkedIn, calls, WhatsApp), built-in lead enrichment, and deliverability tools .



- **[Reply.io](https://reply.io/)**  

  AI-powered sales engagement platform automating multi-channel outreach with email, calls, LinkedIn, and SMS for SDR/BDR teams .



- **[Close](https://close.com/)**  

  Conversation-first CRM with built-in calling, email, and SMS; sequences, smart views, and reporting for small sales teams who need to move fast .



## Open-Source GitHub Projects



### Full SDR Workspaces (Multi-Channel + AI CRM)



- **[AgentSDR](https://github.com/kandid-ai/agentsdr)**  

  The most comprehensive open-source **self-hosted AI SDR** available (MIT, v0.3.1) . Features: **email sequences** from your own Google Workspace mailboxes with merge fields, spin text, per-mailbox daily limits (30 default), sending windows, and one-click unsubscribe; **LinkedIn campaigns** via Unipile with invite, accept message, and follow-ups paced at 30 invites/day on premium accounts (5 on free); **WhatsApp** message campaigns and calls dialed via Chrome extension, recorded to Cloudflare R2 and transcribed by your chosen model . **AI CRM** classifies every reply (Interested, Customer, Not interested, Other), drafts grounded replies from your knowledge base, and **holds all drafts for human approval**—nothing sends automatically; the AI only moves a lead forward when confident . Features **enrichment tables** with AI columns, HTTP calls, formulas, and 15 providers (Apollo, Hunter, Lusha, etc.); **multi-organization** support with roles; analytics by channel for replies, meetings, and customers; Do Not Contact honored everywhere; Docker Compose deployment with Postgres 16 . **Best for teams wanting multi-channel outbound with AI assistance and full data ownership**—you pay for your server and your own AI/API usage, not per-seat fees.



### Cold Email & Deliverability Focused



- **[Pigeon](https://github.com/tarinagarwal/Pigeon)**  

  Open-source **cold email outreach and deliverability platform** (Next.js, MongoDB, Docker) . Features: **multi-step sequences** that stop on reply/bounce/unsubscribe; **A/B testing with auto-selected winner** (60% reply rate, 40% open rate); **inbox rotation** across Gmail and SMTP mailboxes; **three layers of volume control** (campaign daily cap, per-inbox cap hard-limited to 50/day, ramp-up tier scaling with inbox age); **mailbox warm-up** with multi-turn threaded conversations and correct In-Reply-To/References headers; **automatic spam rescue** (opens messages, marks important, moves out of spam); **DNS automation** writing SPF/DKIM/DMARC to Cloudflare/GoDaddy/Namecheap/Google Cloud DNS; **inbox placement testing** via real Gmail/Outlook seeds; **per-recipient AI writing** using your own OpenAI/Anthropic/Gemini/DeepSeek/Grok key . **Best for teams where deliverability is the primary concern**—the warm-up and placement testing depth exceeds most commercial tools.



- **[Emareach](https://github.com/ritik-prog/emareach)**  

  Open-source **cold email outreach and deliverability platform** (FastAPI, Next.js, MongoDB, Docker) . Features: campaigns with sequences and A/B templates; **mailbox warm-up with LLM-generated threads**; **spam→inbox recovery**; SPF/DKIM/DMARC checks; inbox connection via Gmail/Outlook OAuth or SMTP/IMAP; open/click tracking with custom domains; **billing integration** (Razorpay for India, Lemon Squeezy for international); admin panel for user/plan/infrastructure management; support bot via ChromaDB RAG . **Best for teams wanting a production-grade cold email stack with billing and admin included**—heavier stack than Pigeon but more complete operations.



### CRM & Lead Management



- **[OpenCRM](https://github.com/arkitekt-ai/OpenCRM)**  

  Open-source, self-hosted **CRM with lead automation and email campaigns** (Docker, SQLite) . Features: **automated Meta Lead Ads polling** and **webhook ingestion** for any external source; lead pipeline with status tracking (intake → emailed → contacted → qualified → closed); notes, follow-up reminders, deal tracking, pipeline value aggregation, lead assignment, and tagging; **AI email generation** with OpenAI/Anthropic/Ollama or any OpenAI-compatible endpoint; **campaigns** with AI copy and one-click send; **multi-step email sequences** with configurable delays; **Kanban board** with deal values and reminder badges; reports (conversion funnel, leads by source, pipeline value by status, leads over time) . **Best for teams wanting a lightweight, self-hosted CRM with built-in lead automation and AI email generation**—simpler than AgentSDR but focused on CRM rather than multi-channel sequences.



### Lead Scraping & Enrichment



- **[Contractor Lead Scraper](https://pypi.org/project/contractor-lead-scraper/)**  

  Open-source **Google Maps lead scraper** with deep website email crawling (Python/Playwright, PyPI) . Features: **asset-blocked Playwright scraper** for 10x faster scraping (disables images, stylesheets, media, trackers); extracts business name, rating, review count, category, address, website; **multi-vector deep email extraction** crawling high-probability routes (/, /contact, /about, /team, /terms, /privacy, /estimate); **E.164 phone normalization**; CSV output with 10 fields; **100% free** with no proxy or API costs . **Niche**—best for local service businesses (contractors, roofers, HVAC) rather than general B2B SaaS prospecting, but demonstrates the pattern for zero-cost lead sourcing.



- **[ColdPost](https://github.com/Avika2211/ColdPost)**  

  Open-source **lightweight cold email automation tool** (Python/Flask, Zenodo) . Features: CSV upload, `{name}` personalization, file attachments (resumes, pitch decks), bulk sending via Gmail SMTP, clean web interface. **Best for students and entrepreneurs** wanting free cold outreach without platform subscriptions—**not a production SDR platform**, but a starting point for simple personalized bulk email .



- **[Helio](https://github.com/achref-soua/helio)**  

  Open-source **growth platform** with CDP, segmentation, cross-channel journeys, email, and analytics (self-hostable, data-sovereign) . Features: multi-tenant isolation via PostgreSQL row-level security; Temporal-backed journey sends with retry policies; **hot-path ingestion load-tested at 20,000 events/s**; SSO/SCIM, TOTP 2FA, encrypted credential vault; Docker/Helm deployment . **Best for teams wanting marketing automation infrastructure** (CDP + journeys) rather than SDR-specific sequences—complements a prospecting tool rather than replacing it.



### Additional Strong Open-Source Options



- **Twenty** — Open-source CRM with customizable data models, workflows, and APIs; positioned as a modern Salesforce alternative . **Best for teams wanting a self-hosted CRM foundation** to build prospecting workflows on top of.

- **DenchClaw** — Locally running AI CRM built on OpenClaw; natural language database queries, LinkedIn/email automation, and Kanban pipeline . **Early-stage/local-first**—verify production maturity, but the natural-language CRM interaction is novel.



**Frameworks for building custom systems**: For **multi-channel SDR with AI CRM**, AgentSDR provides the most complete open-source foundation with email, LinkedIn, WhatsApp, and human-approved AI drafts . For **deliverability-first cold email**, Pigeon (warm-up depth) or Emareach (billing + admin) . For **CRM with lead automation**, OpenCRM . For **marketing automation infrastructure**, Helio . No open-source project bundles a **lead database** comparable to Apollo or ZoomInfo—you supply enrichment via APIs (Apollo, Hunter, Lusha) or scrape your own leads .



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Sales prospecting platforms handling lead data and outreach must comply with applicable regulations (GDPR, CAN-SPAM, CCPA, local anti-spam laws) and platform terms of service; **LinkedIn automation, bulk WhatsApp messaging, cold email, and call recording carry legal and platform risks** that self-hosted tools do not eliminate .

- **Open-source SDR workspaces are mature for sequencing and AI assistance**—AgentSDR provides multi-channel outreach with human-approved drafts , Pigeon provides deliverability depth , and OpenCRM provides CRM + lead automation . However, **no open-source project bundles a B2B contact database** comparable to Apollo or ZoomInfo—budget for enrichment APIs or lead scraping separately.

- Verify license terms for commercial use; AgentSDR uses MIT , Pigeon and Emareach are open-source (check repositories), and OpenCRM is open-source .



---



**Made for SDR leaders, sales operations teams, and founders building outbound infrastructure.**  

Let's make sales prospecting more open, but with clear eyes about the lead data costs and compliance responsibilities that self-hosting does not eliminate.

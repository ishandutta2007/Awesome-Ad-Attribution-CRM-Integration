# Awesome-Ad-Attribution-CRM-Integration

# Awesome-Ad-Attribution-CRM-Integration

**Top Ad Attribution CRM Integration (Opensource) 🌟 Star if you like it! 🌟**



**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Multi-Touch Attribution, Mobile Measurement, First-Party Data & Self-Hosted Attribution Models*

**Last updated: November 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Ad Attribution & CRM Integration**. These tools enable marketing and revenue teams to connect ad spend to CRM outcomes—mapping touchpoints across channels, measuring true ROI, and closing the loop between acquisition and revenue—from fully managed mobile measurement partners (MMPs) and B2B attribution platforms to open-source libraries that implement Shapley, Markov, and media mix modeling without vendor lock-in.



**Examples** include AppsFlyer, Singular, Branch, Adjust, Rockerbox, Triple Whale, Ruler Analytics, Dreamdata, HockeyStack, and Zoho CRM's native Google Ads integration (the category leaders in commercial space).



**Open-source emphasis**: This section is expanded with every relevant project for self-hosted attribution, mobile measurement, and open marketing analytics. **Critical note**: The open-source landscape is nascent but functional—**Attributor** implements Shapley value, Markov chain, and Bayesian MMM in Go , while **Open Attribution** is building an open-source MMP for mobile app marketers . No open-source project matches AppsFlyer's SKAN modeling depth or Dreamdata's B2B company identification, but for teams wanting model transparency and data ownership, the building blocks exist.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [Sector Overview & Market Dynamics](#sector-overview--market-dynamics)
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## Sector Overview & Market Dynamics

The global marketing attribution software market is estimated at approximately **$5.5 billion to $6.0 billion in 2026**, projected to expand rapidly toward **$15B–$21B by 2030–2032** at a 15–20% CAGR driven by privacy shifts, signal loss, and AI-driven cross-channel measurement. The industry exhibits a **hybrid, moderately fragmented landscape**: while enterprise cloud giants (such as Salesforce, Adobe, and Google) dominate generalized CRM/marketing cloud budgets, the specialized attribution space remains dynamic and fragmented across distinct sub-verticals (mobile measurement partners, B2B pipeline attribution, and e-commerce multi-touch attribution) where niche, specialized platforms prevent a single winner-take-all outcome.

## SaaS/Hosted Platforms

| Platform | Company Size (Valuation / Revenue) | Pricing (Starting Tier) | Free Tier / Trial Limits | Key Features & Focus |
|---|---|---|---|---|
| **Zoho CRM (Google Ads Integration)** | **~$12.5B Valuation** / ~$1.5B ARR (FY25) | Starts at **$23/user/month** (billed annually) for Professional edition (required tier for Google Ads integration) | **Permanent Free tier** for up to 3 users (Google Ads integration excluded); **15-day free trial** of paid Professional/Enterprise tiers with no credit card required | Native Google Ads campaign management and offline conversion tracking directly within CRM. |
| **Adjust** | **$1.0B Acquisition** by AppLovin (Parent ~$90B Market Cap) / ~$100M+ ARR | Starts at **$0** (Base tier); paid commercial plans start at custom quote (~**$500–$1,500/month** min. contract commitment) | **Base Free plan**: Up to 1,500 monthly conversions (capped at 18,000 annual conversions) for the first year with core attribution & Datascape analytics | Mobile Measurement Partner (MMP) for mobile app attribution, deep linking, and campaign analytics. |
| **Branch** | **$4.0B Valuation** (Series F) / ~$125M ARR | Starts at **$39/month** (Intro plan after trial) or **$199/month** (Activation Basics); Performance Basics at **$499/month** | **30-day free trial** of paid tiers (requires credit card with temporary $10 hold); defaults to $39/mo plan if not cancelled | Enterprise deep linking, cross-platform attribution, SKAdNetwork modeling, and mobile web-to-app tracking. |
| **AppsFlyer** | **$2.7B Valuation** (Series E) / ~$500M ARR | Starts at **$0** (Zero plan); paid Growth tier starts at **$0.07/conversion** (pay-as-you-go after free allowance) | **Zero Free plan**: Free forever for owned media (unlimited organic installs); **Growth Welcome Package**: First 12,000 paid conversions free for 12 months + 30-day trial of premium add-ons (no credit card required) | Industry-leading mobile attribution and marketing analytics with SKAN modeling and fraud prevention. |
| **Triple Whale** | **~$380M Valuation** (Series B) / ~$21.6M ARR | Starts at **$219/month** (Foundation tier for lower GMV stores) | **Free Plan**: Free forever for early-stage stores (Triple Pixel, first/last-click attribution, 12-month data retention, up to 10 users; no multi-touch MTA) | E-commerce attribution, BI, and AI analytics platform purpose-built for Shopify and DTC brands. |
| **Singular** | **~$150M–$200M Est. Valuation** / ~$52.6M ARR | Free Starter tier; paid Growth plan starts around **$795/month** (or ~$0.05/conversion custom) | **Starter Free plan**: Up to 15,000 free attributed conversions per month (organic installs always free, no credit card required); **14-day free trial** for analytics/ETL | Unified marketing analytics, mobile attribution, automated cost aggregation, and ROAS calculations. |
| **Rockerbox** | **$85M Acquisition** by DoubleVerify / ~$10M–$15M ARR | Enterprise custom quotes starting at ~**$2,000/month** ($24,000/year minimum contract) | **No free tier and no free trial** (previous Starter tiers retired; access requires scheduling a sales demo) | Multi-touch attribution (MTA), Media Mix Modeling (MMM), and incrementality testing on first-party data. |
| **HockeyStack** | **~$80M–$100M Est. Valuation** / ~$9M ARR | Baseline plans start around **$599–$1,200/month** (typical annual contracts range $12,000–$30,000/year) | **No free tier and no free trial** (interactive demo available online; full stack onboarding requires sales engagement) | B2B multi-touch attribution, cookieless account tracking, and AI revenue agents. |
| **Dreamdata** | **~$30M–$50M Est. Valuation** ($67M total raised) / ~$3M ARR | Starts at **$0/month** (Free plan); paid Team/Growth tiers start at **$750–$999/month** (billed annually) | **Free Plan**: Free forever (B2B web analytics, cookieless tracking, company reveal, 2 months data history, up to 5 seats) | B2B revenue and pipeline attribution connecting marketing activities to CRM deals and revenue. |
| **Ruler Analytics** | **Private / Bootstrapped** / ~$3M ARR | Starts at **$149–$179/month** for entry-level tier (scaling up to $999/month for enterprise) | **No free tier and no free trial** (evaluation requires scheduling a guided product demo with sales) | Multi-touch attribution, closed-loop revenue tracking, form tracking, and dynamic call tracking for lead gen. |



## Open-Source GitHub Projects



- **Attributor**

  **Open-source marketing attribution engine** (Go) — **the most complete open-source attribution library** found in this research, implementing the three major attribution methodologies . **Features**: **Shapley Value Attribution**—measures marginal contribution of each channel across all possible channel combinations (the only method satisfying symmetry, linearity, and efficiency); **Markov Chain Attribution**—removal effect: remove a channel and measure the drop in conversion probability; **Bayesian MMM**—media mix model using Hamiltonian Monte Carlo with **adstock transformations** (carryover effects), **saturation curves** (Hill functions), and **90% credible intervals**; **CLI** for Shapley, Markov, MMM fit, budget simulation, and JSON export; **API server** with endpoints for attribution, MMM fit, and simulation . **Tech stack**: Go. **Deploy**: CLI (`attributor attrib shapley --journeys journeys.json`); API server. **Trade-off**: **Library, not a platform**—requires your own journey data; no CRM integration, no UI, no real-time collection. **Best for**: data scientists and marketing analysts wanting to compute Shapley, Markov, or MMM attribution on their own customer journey data—especially those wanting model transparency and no vendor lock-in.



- **Open Attribution**

  **Open-source MMP for mobile app marketers** (Apache-2.0) — **the only open-source mobile measurement partner (MMP) project** found in this research, created to "bring control of advertising data back to the app creators and developers who it belongs to" . **Features**: **Mobile attribution** for app installs and in-app events; **SDKs** for iOS (Swift) and Android (Kotlin); **ClickHouse** backend for event storage; **example apps** for integration reference . **Tech stack**: Svelte (web), Swift (iOS SDK), Kotlin (Android SDK), ClickHouse. **Deploy**: Self-hosted. **Trade-off**: **Early-stage project**—latest activity September 2025; no SKAN modeling, fraud protection, or deep linking; **not production-ready** for paid campaigns at scale. **Best for**: developers wanting to build or contribute to an open-source alternative to AppsFlyer/Adjust—accepting early-stage maturity.



### Additional Strong Open-Source Options



- **No mature open-source CRM-integrated attribution platform exists.** AppsFlyer, Singular, Branch, Adjust, Rockerbox, Triple Whale, Ruler, Dreamdata, and HockeyStack are proprietary. **Attributor** provides the attribution math but not the data pipeline or CRM integration. **Open Attribution** aims to replace MMPs but is early-stage. For production ad-to-CRM attribution, commercial platforms are required.



**Frameworks for building custom systems**: **Attributor** provides the attribution models (Shapley, Markov, MMM) and **Open Attribution** provides the mobile SDK foundation. **Neither includes CRM integration, ad platform connectors, or real-time data pipelines**—those must be built or sourced separately.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, license (for open-source), and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Ad attribution platforms handling user behavior and CRM data must comply with data protection regulations (GDPR, CCPA, ePrivacy, etc.) and implement appropriate consent management.

- **The "mobile MMP" vs. "B2B attribution" vs. "e-commerce attribution" vs. "call tracking" distinction is critical.** **AppsFlyer, Singular, Branch, and Adjust** are **mobile MMPs**—they measure app installs and in-app events across ad networks . **Rockerbox, Dreamdata, and HockeyStack** are **B2B attribution**—they connect marketing touchpoints to company-level revenue . **Triple Whale** is **e-commerce attribution**—it tracks Shopify orders and ad spend . **Ruler Analytics** is **call tracking + CRM attribution**—it connects phone calls and forms to revenue . **Zoho CRM** provides **native Google Ads integration**—not multi-channel attribution . **Choose based on whether you need mobile, B2B, e-commerce, or lead-gen attribution.**

- **AppsFlyer's Zero plan is for owned media only**—it cannot measure paid campaigns. **Growth requires $0.07 per conversion after 12K free**—model your paid install volume before committing .

- **Adjust's anti-fraud is consistently criticized.** Reviewers describe it as "very poor," "very bad designed," and "ineffective" at distinguishing invalid from clean traffic . **If fraud protection matters, Protect360 or AppsFlyer is worth the premium.**

- **Rockerbox's free tiers are gone.** The plans page has no pricing, warehouse integration is a paid add-on, and /signup-free redirects to /demo . **Do not expect self-serve evaluation.**

- **Dreamdata's free plan is genuinely usable** for small B2B teams—5 seats, 2 months history, company identification, and ad spend reporting at $0 . **For B2B startups testing attribution, it is the pragmatic starting point.**

- **HockeyStack's onboarding risk is real.** One reviewer cancelled after 4 months because data could not be connected; 90% of touchpoints required manual mapping . **Request a proof-of-concept with your actual data sources before signing.**

- **Attributor is the most complete open-source attribution engine**—Shapley, Markov, and Bayesian MMM in one Go library with CLI and API . **The trade-off**: you own the data pipeline and CRM integration. **For teams wanting model transparency without vendor lock-in, it is the starting point.**

- Self-hosted open-source solutions require proper infrastructure (Go for Attributor, ClickHouse for Open Attribution), data pipeline development, and ongoing maintenance. **Attribution models handle sensitive customer journey data**—ensure your deployment meets your organization's privacy and compliance requirements before processing production data.



---



**Made for marketing analysts, growth teams, and organizations building transparent attribution solutions.**

Let's make Ad Attribution & CRM Integration more open, data-driven, and revenue-accountable.

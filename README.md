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
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **AppsFlyer**
  **Mobile attribution and marketing analytics** platform. **Pricing**: **Zero (free)** for owned media only (12K free conversions first year); **Growth (pay-as-you-go)** with **$0.07 per conversion** after 12K free; **Enterprise** custom pricing . **Free tier**: Yes, Zero plan for owned media. **Best for**: mobile-first companies needing the industry's most mature SKAN modeling, fraud protection, and deep linking—**trade-off**: per-conversion costs scale with paid campaigns; premium features (Protect360, raw data API) require Enterprise.

- **Singular**
  **Marketing attribution and analytics** platform. **Pricing**: **Starting at $795/month** per Software Advice . **Free tier**: None. **Best for**: teams wanting unified data aggregation across partners with API-driven ETL for ROAS calculations—**trade-off**: saved reports can become cluttered; no public free tier .

- **Branch**
  **Mobile linking and attribution** platform. **Pricing**: **Basics, Essentials, Enterprise** tiers; Essentials adds unlimited partners and SKAN clarity; Enterprise adds CTV/OTT attribution, advanced SKAN modeling, and API flexibility; **pricing scales with growth** (no public rates) . **Free tier**: Basics tier available (feature-limited). **Best for**: teams prioritizing deep linking and cross-platform attribution alongside measurement—**trade-off**: SKAN modeling and CTV require higher tiers .

- **Adjust**
  **Mobile measurement partner (MMP)** with attribution and analytics. **Pricing**: **Quote-only**; reviewers describe pricing as "competitive" and "cost effective" compared to competitors . **Free tier**: None. **Best for**: cost-conscious teams wanting core MMP capabilities—**trade-off**: reviewers report **weak anti-fraud** and **poorly designed cost API**; platform has "not evolved at the same pace as the market" .

- **Rockerbox**
  **Unified marketing measurement** (MTA + MMM + incrementality). **Pricing**: **No public pricing**—plans page is "Talk to an Expert" only; **warehouse integration is a paid add-on**; free/Starter tiers retired . **Free tier**: None (retired). **Best for**: teams wanting multi-touch attribution and media mix modeling on first-party data with warehouse-native delivery—**trade-off**: no self-serve; warehouse integration costs extra; no public API .

- **Triple Whale**
  **E-commerce analytics and attribution** for Shopify brands. **Pricing**: **Foundation, Automate, Enterprise** tiers; **Sonar (AI) included in all paid packages**; attribution models include First Click, Last Click, Linear, Triple Attribution, and Total Impact (with post-purchase survey data); **SOC 2 compliant** . **Free tier**: None. **Best for**: DTC brands wanting attribution and BI in one platform with fast setup (~15 minutes)—**trade-off**: e-commerce-focused; not B2B or mobile-app-centric .

- **Ruler Analytics**
  **Marketing attribution for lead-gen** with call tracking and CRM integration. **Pricing**: **Quote-only**; reviewers note it is **cheaper than competing call-tracking platforms** and offers good value; discounts available for multi-year commitments and volume . **Free tier**: None. **Best for**: B2B and service businesses needing call tracking, form tracking, and CRM revenue attribution—**trade-off**: setup effort; contract flexibility noted as a concern by some reviewers .

- **Dreamdata**
  **B2B revenue attribution** platform. **Pricing**: **Free $0/month** (B2B web analytics, cookie/cookieless tracking, company identification, audience builder, ad spend report; limits: 2 months history, 5 seats, 3 stage models); **Advanced** custom pricing (AI attribution, advanced activation, MCP server, data warehouse add-on) . **Free tier**: Yes, genuinely usable for small B2B teams. **Best for**: B2B companies wanting company-level attribution with a free starting point—**trade-off**: advanced AI and activation require custom pricing .

- **HockeyStack**
  **B2B attribution and analytics** platform. **Pricing**: **Quote-only**; reviewers cite **lengthy onboarding** (one reviewer cancelled after 4 months due to data connection failure) and **90% of touchpoints requiring manual mapping** . **Free tier**: None. **Best for**: teams wanting cookieless funnel tracking with automatic goals—**trade-off**: onboarding risk is significant; support structure "visibly strained" per reviewers .

- **Zoho CRM for Google Ads**
  **Native Google Ads integration** within Zoho CRM. **Pricing**: Included with Zoho CRM Professional (₹1,400/user/month) and above . **Free tier**: Limited (CRM free tier for 3 users). **Best for**: Zoho CRM users wanting to manage Google Ads campaigns and track ROI within their CRM—**trade-off**: Google Ads only; not a multi-channel attribution platform .

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

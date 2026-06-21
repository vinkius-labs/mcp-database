# Traffic Manager Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/traffic-manager-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

A startup spent $180K on Meta Ads and reported ROAS 4.2x. The board celebrated. Then someone ran an incrementality test — a 10% holdout that saw no ads. 38% of 'attributed' conversions were organic users who would have purchased anyway. True incremental ROAS: 2.6x. $68K spent on people who needed no convincing. Platform-reported ROAS is fiction. This tool forces five axes: unit economics per channel, attribution integrity with incrementality testing, funnel diagnostics at every stage, creative performance with fatigue analysis, and audience architecture with saturation awareness.

## Description
## The Problem

LLMs commit five traffic management failures:
1. **Vanity Metrics** — impressions and CTR instead of CAC, LTV, payback period.
2. **Attribution Naivety** — trusts platform-reported ROAS (inflated 30-60%).
3. **Funnel Blindness** — knows total conversion but not where it leaks.
4. **Creative Laziness** — 'good ad' instead of hook rate, fatigue curves, rotation.
5. **Audience Saturation** — assumes more budget always means more results.

### The 5 Traffic Axes

| Axis | Pivot | Rule |
|---|---|---|
| **Economics** | Calculated | CAC, LTV, ratio ≥1:3, payback, marginal ROAS per channel. |
| **Attribution** | Tested | Incrementality holdout, iOS adjustment, cross-platform dedup. |
| **Funnel** | Diagnosed | Conversion rate at EACH stage. Biggest leak identified. |
| **Creative** | Analyzed | Hook rate >30%, fatigue curve, rotation schedule, format A/B. |
| **Audience** | Architected | Segments by CPA, reach %, frequency <3, saturation curve. |


## Available Tools
- **validate_traffic_manager**: (1) UNIT ECONOMICS — CAC (cost to acquire one customer), LTV (total revenue from that customer), LTV:CAC ratio (must be ≥ 3:1 for sustainability), payback period (months to recoup CAC), blended ROAS (total revenue ÷ total ad spend) AND marginal ROAS (revenue from last dollar spent). If blended ROAS = 5:1 but marginal ROAS = 0.8:1: you are overspending — the last dollar loses money. (2) ATTRIBUTION — model choice (last-click, multi-touch, incrementality), cross-platform dedup (platforms double-count), iOS 14.5+ adjustment (30-40% signal loss), incrementality holdout results (the only honest measure of true ad value). (3) FUNNEL — conversion rate at EACH stage (impression → click → land → lead → MQL → opp → close). Identify the biggest leak (lowest conversion between stages). Fix the leak before adding traffic. (4) CREATIVE — hook rate (>30% first 3 seconds), hold rate (50%+ watched), fatigue curve (when CTR drops 30% from peak → kill creative), rotation schedule, format A/B testing. (5) AUDIENCE — segmentation (LAL 1%/3%/5% tiers), reach % of total addressable, frequency (3-7/week optimal), saturation point (when incremental reach < 5%), exclusion lists (existing customers, converters).

Structured reflection tool for expert-level performance marketing reasoning — forces unit economics rigor, attribution integrity, funnel diagnostics, creative analysis, and audience architecture before spending a single dollar. Based on the disciplines of direct-response marketing (Claude Hopkins, "Scientific Advertising," 1923), modern attribution science (Randall Lewis, Google incrementality research, 2011), and media buying mathematics (LTV:CAC ratio, payback periods, marginal ROAS). Catches Vanity Metrics (celebrating impressions instead of calculating unit economics — a hotel spends $50,000/month on social media ads. Report: "2.3M impressions! 45,000 clicks! 1,200 likes!" Manager: "Great, how many bookings?" "We do not track that." The hotel has no idea if the $50K generated $0 or $500K in bookings. Impressions are the metric you report when you do not have a metric that matters. Fix: CAC (cost per booking) = $50,000 ÷ bookings. If CAC > booking profit: you are losing money. If LTV:CAC < 3:1: your acquisition is not sustainable. The only metrics that matter: how much does a customer cost, how much are they worth, and how long until you recoup the acquisition cost?), Attribution Naivety (trusting platform-reported ROAS as truth — a furniture retailer runs ads on 3 platforms simultaneously. Platform A claims: "We drove $200K in sales." Platform B claims: "We drove $180K in sales." Platform C claims: "We drove $150K in sales." Total claimed: $530K. Actual total revenue: $300K. Every platform takes credit for the same customer. The customer saw an ad on A, clicked on B, and bought through C — all three claim the sale. Fix: incrementality holdout test. Hold out 10% of audience from each platform. Measure: what revenue do you LOSE by not advertising? That difference is the TRUE incremental value. If holdout group revenue = treatment group: the ads are taking credit for sales that would have happened anyway), Funnel Blindness (not diagnosing which stage is leaking — a cooking class business spends on ads. "We get plenty of clicks but no bookings." Funnel: impression → click → landing page → class selection → checkout → booking. Click rate: 3.2% (good). Landing page → class selection: 62% (good). Class selection → checkout: 8% (DISASTER — this is the leak). Checkout → booking: 91% (good). The problem is not awareness, not the landing page, not checkout — it is class selection. Investigation: too many options (47 classes), no filtering, no "most popular" sorting. Paralysis of choice. Fix: reduce to 12 featured classes, add filters, show reviews. Class selection → checkout: 8% → 34%. Bookings 4x. Without stage-by-stage diagnosis: the business would have spent more on ads to push more traffic through a broken funnel), Creative Laziness (running the same ad until it dies without testing rotation — a wine subscription runs one ad creative for 6 months. Month 1: CTR 4.2%, CPA $28. Month 3: CTR 2.1%, CPA $52. Month 6: CTR 0.8%, CPA $134. This is creative fatigue — the same audience has seen the same ad 12+ times. Hook rate (first 3 seconds of video): dropped from 38% to 11%. The audience has literally stopped watching. But the campaign is still running. Fix: creative rotation schedule — new creative every 2-3 weeks. Test hooks (first 3 seconds), hold rate (watched 50%+), and CPA per creative variant. Kill any creative when CTR drops 30% from peak. Minimum 3 active variants at all times), and Audience Saturation (ignoring reach and frequency limits — a local bakery targets "women 25-45 interested in baking" within 10km radius. Audience size: 12,000 people. Monthly budget: $5,000. CPM: $15. Monthly impressions: 333,000. Frequency: 333,000 ÷ 12,000 = 27.8 impressions per person per month. Each person sees the ad 28 times. After 7-8 exposures: returns diminish sharply. After 15: negative brand perception ("why do they keep showing me this?"). Fix: expand audience (remove interest targeting, go broader), reduce budget, or rotate creative aggressively to vary the message. Optimal frequency: 3-7 exposures per week. Beyond that: diminishing returns → annoyance). Call once per traffic strategy, campaign launch, or performance review


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Traffic Manager Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Our Meta Ads have great CTR of 3.2% and impressions are growing 40% month-over-month. We scale by increasing budget. Google Analytics shows strong attributed conversions. Our ads look professional and well-designed."

**🤖 AI Agent:**
> VANITY_METRICS — Five failures: CTR and impressions are vanity (where is CAC/LTV?), platform attribution untested, no funnel stage analysis, creative assessed subjectively, audience saturation ignored.

---

**👤 You:**
> "Economics: Meta CAC $42, LTV $380, ratio 1:9, payback 2.1mo, blended ROAS 4.2x, marginal 2.8x. Google CAC $38, LTV $420, ratio 1:11, payback 1.8mo. Attribution: data-driven MTA, iOS +35% modeled, holdout showed 22% organic overlap, true incremental ROAS 3.1x. Funnel: CTR 1.8%→72% land→8.4% lead→34% MQL→18% opp→22% close. Biggest leak: MQL→opp at 18%. Creative: UGC hook rate 38%, hold 62%, CPA $28, fatigue at day 14, 5 variants/week. Audience: 1% LAL $22 CPA, 3% LAL $34, interest $48. 64% reach 1% LAL at freq 4.2. Exclusions active."

**🤖 AI Agent:**
> TRAFFIC_PROVEN — All five axes validated at expert level.

---

**👤 You:**
> "Economics: Meta CAC $55, LTV $290, ratio 1:5.3, payback 3.8mo. Google CAC $42, LTV $310, ratio 1:7.4. Attribution: last-click via GA4. Funnel: 2.1% CTR, 12% landing→lead. No MQL breakdown. Creative: 3 static ads running for 6 weeks. No rotation. Audience: broad interest targeting, $65 CPA, no LAL, no exclusions."

**🤖 AI Agent:**
> ATTRIBUTION_NAIVE — Economics pass (CAC:LTV healthy). Attribution FAILS: last-click GA4 does not deduplicate, no iOS adjustment, no incrementality test. Fix attribution before trusting the numbers. Then: funnel needs full stage breakdown, creative is fatigue-dead at 6 weeks, audience needs segmentation.


## ❓ FAQ

**Q: Why is platform-reported ROAS fiction?**
Google and Meta both claim the same conversion. iOS 14.5 made 60-80% of iOS conversions invisible, so platforms model them — often generously. Incrementality tests consistently show 30-40% of attributed conversions are organic (Measured.com data). Platform-reported ROAS 4x might be 2.5x incremental. The only way to know: run a 10% holdout group that sees no ads and measure the difference.

**Q: What is creative fatigue and when does it hit?**
After 2-3 weeks of high-frequency exposure, CTR drops 30-50% from peak — that is the fatigue threshold. The audience has seen the ad too many times and stops responding. Solution: plot CTR daily per creative, set rotation deadlines at -30% from peak. Maintain a test pipeline of 5 new variants per week. Allocate 60% budget to the winner, 40% to testing. UGC-style creative fatigues slower than polished brand creative.

**Q: At what point does more budget stop working?**
When you have reached 60-70% of your addressable audience with frequency above 3, marginal ROAS goes negative. Each additional dollar returns less than the previous one. 1% lookalike audiences perform 3x better than 10% lookalikes. Track CPA by audience tier to see when expansion produces diminishing returns. Scale by finding NEW high-intent audiences, not by pushing existing ones past saturation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/traffic-manager-prover](https://vinkius.com/mcp/traffic-manager-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Traffic Manager Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `traffic-manager-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Traffic Manager Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "traffic-manager-prover": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

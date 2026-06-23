# Pricing Strategy Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pricing-strategy-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

An AI recommended '$29/month per seat' because that is what three competitors charge. No value metric analysis — seat count has nothing to do with value delivered. No WTP research — the price was copied, not discovered. No segmentation — enterprise pays the same as a 3-person startup. No unit economics — CAC was $380 and LTV at $29/month with 14-month retention was $406. LTV/CAC of 1.07x. The company grew revenue 12% while burning 40% of cash on acquisition. This tool forces value metric definition, WTP research, segment pricing, unit economics, and packaging design.

## Description
AI agents pick prices from competitor pages and call it strategy. They default to per-seat because SaaS uses per-seat. They skip WTP research. They charge enterprise the same as startups. They ignore unit economics until the board asks why CAC exceeds LTV.

### The Problem

LLMs commit five pricing failures that destroy margin:

- **Value Metric Undefined** — Per-seat pricing for a product where seat count does not correlate with value. An analytics platform charges per seat — but a 5-person team generating $2M in insights pays the same as a 5-person team checking dashboards once a week.
- **WTP Unresearched** — '$29/month because competitors charge $25-35.' That is copying, not pricing. No Van Westendorp PSM. No customer interviews about current spend. No data on acceptable range or too-cheap threshold.
- **Segmentation Absent** — One price for all. A 3-person startup and a 500-person enterprise get identical pricing. The startup over-pays relative to value. The enterprise under-pays by 10x relative to ROI.
- **Unit Economics Broken** — Price set without calculating CAC, LTV, LTV/CAC ratio, payback period, or gross margin. Revenue grows while the company burns cash — a price that does not cover acquisition cost is a subsidy.
- **Packaging Misaligned** — Free tier includes everything. Premium adds 'priority support.' No natural upgrade trigger. The free-to-paid conversion rate is 1.2% because there is no reason to upgrade.

### How It Works

5 Decision Pivots:

1. **valueMetricDefined** — Pricing tied to a metric that scales with customer success. API calls, events, active contacts, revenue processed — not arbitrary per-seat.
2. **wtpResearched** — Customer WTP studied with data. Van Westendorp, Gabor-Granger, conjoint, or interviews. Acceptable range, optimal price, and anchor spend documented.
3. **segmentationApplied** — Different segments priced differently. Profiles, value perception, price sensitivity, and fencing defined.
4. **unitEconomicsValid** — CAC, LTV, LTV/CAC ≥3x, payback ≤12 months, gross margin ≥70%.
5. **packagingAligned** — Tiers with natural upgrade triggers. Free/trial demonstrates value. No anti-patterns.

### The Verdict Matrix

| First Failing Pivot | Verdict | Meaning |
|---|---|---|
| valueMetricDefined = false | VALUE_METRIC_UNDEFINED | Pricing not tied to value delivered. |
| wtpResearched = false | WTP_UNRESEARCHED | Price copied, not discovered. |
| segmentationApplied = false | SEGMENTATION_ABSENT | One price for all. Money left on table. |
| unitEconomicsValid = false | UNIT_ECONOMICS_BROKEN | Revenue without margin is a subsidy. |
| packagingAligned = false | PACKAGING_MISALIGNED | No upgrade trigger. Free tier kills conversion. |
| All pivots pass | PRICING_PROVEN | Value-aligned, researched, segmented, profitable, packaged. |

### Why It Works

- **Tool calls are obligations.** The agent cannot recommend a price without stating the value metric, citing WTP research data, defining segment-specific prices, and calculating unit economics.
- **Consistency engine catches contradictions.** If the agent claims `wtpResearched=true` but says 'based on competitor pricing,' the engine rejects.
- **Semantic traps detect lazy pricing.** 'Per seat,' 'competitive pricing,' 'we keep it simple,' and 'we will figure out margins later' trigger automatic rejection.


## Available Tools (1)
- **validate_pricing_strategy**: You must: (1) VALUE METRIC — identify the unit that scales with customer success. Not per-seat unless seats = value. API calls, events, storage, revenue processed, active contacts, (2) WTP RESEARCH — Van Westendorp, Gabor-Granger, or customer interviews with N= sample size. Not "competitor charges $X." Your customers are not their customers, (3) SEGMENTATION — different prices for segments with different value perception. Feature fencing to prevent cross-segment arbitrage. Freelancer ≠ Enterprise, (4) UNIT ECONOMICS — CAC by channel, LTV ADJUSTED FOR GROSS MARGIN, LTV/CAC ≥ 3x, payback ≤ 12 months, gross margin ≥ 70%. Raw LTV without gross margin adjustment is fiction, (5) PACKAGING — tiers with natural upgrade triggers. Zero anti-patterns: no generous free, no minor premium, no "call us" enterprise. If rejected, the pricing has a revenue-killing structural flaw. Fix before launching.

Structured reflection tool for pricing strategy validation — forces value metric identification, willingness-to-pay research with named methodology, segment-specific pricing with fencing, unit economics verification at each tier, and packaging design with natural upgrade triggers before any pricing decision ships. Grounded in Van Westendorp PSM, Gabor-Granger, Simon-Kucher methodology, and SaaS benchmarks. Catches Value Metric Misalignment (pricing on a unit that does not scale with customer value — "We charge per seat." The product is a monitoring dashboard. One engineer monitors 500 servers — same value whether 1 seat or 50. Per-seat pricing: the customer adds 1 seat ($29/month) to monitor $2M in infrastructure. Value delivered: $2M in uptime protection. Price captured: $29. Value capture ratio: 0.0015%. Correct value metric: per server monitored, or per alert resolved, or per incident prevented. At $5/server/month × 500 servers = $2,500/month. Value capture: 1.5% — still low but 100x better. The value metric must grow AS the customer gets more value — not as they hire more people), WTP Guesswork (setting prices based on competitor pricing or founder intuition instead of research — "Our competitor charges $29, so we will charge $25." This assumes: (1) the competitor researched their price (they probably did not), (2) your segments have the same WTP (they probably do not), (3) lower price wins (it often does not — it signals lower quality). Van Westendorp Price Sensitivity Meter with N=200 from target segment: Too Cheap: $15 (below this, quality is suspect). Bargain: $35. Expensive: $65. Too Expensive: $95. Optimal Price Point: $49 (intersection of too-cheap and too-expensive curves). Acceptable Range: $35-$65. The competitor at $25 is BELOW the too-cheap threshold — they are losing revenue AND credibility), Segment Blindness (one price for all customers regardless of value perception — a project management tool charges $10/user/month for everyone. Freelancer: manages 3 projects, value delivered ≈ $50/month in time saved. $10 is appropriate. Enterprise team of 200: manages 500 projects, value delivered ≈ $50,000/month in coordination savings. $10/user × 200 = $2,000/month. Value capture: 4%. The enterprise is a 50x better customer being charged 1x. Correct: Freelancer tier $10/user. Team tier $25/user (includes integrations, reporting). Enterprise tier: custom pricing based on value delivered + SLA. Fencing: feature gates (SSO, audit logs, API access) that enterprises need but freelancers do not), Phantom Unit Economics (showing LTV/CAC ratio without adjusting for gross margin — "LTV/CAC = 5x! We are very efficient." CAC: $500. LTV: $2,500 (average lifetime × ARPU). But gross margin is 40% (heavy compute costs). Adjusted LTV: $2,500 × 0.40 = $1,000. Adjusted LTV/CAC: 2.0x. Below the 3x threshold. The business appears healthy but is actually unprofitable at unit level. LTV must ALWAYS be adjusted for gross margin. SaaS benchmark: gross margin ≥ 70%. Below 60% = structural problem. Payback period at 40% margin: $500 / (ARPU × 0.40) = much longer than expected), and Packaging Anti-Patterns (tier design that blocks upgrades or leaves money on the table — Anti-Pattern 1: "Generous Free" — free tier includes 95% of features. Result: 98% of users stay free. Conversion rate: 2%. Fix: free tier demonstrates value but creates friction at the natural expansion point (e.g., 3 projects free, paid at project 4 — when the user has invested enough to feel switching cost). Anti-Pattern 2: "Minor Premium" — premium adds only 1-2 features over free. Result: upgrade feels like a donation, not a value exchange. Fix: premium must unlock a workflow the user NEEDS as they grow (collaboration, integrations, reporting). Anti-Pattern 3: "Call Us Enterprise" — no price listed, forces a sales call. Modern buyers (especially developers) abandon at "Contact Sales." Fix: list enterprise starting price or price calculator + self-serve option). Call once per pricing decision, model change, or tier restructuring


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pricing Strategy Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We should price at $29/month per seat. That is what Competitor X and Competitor Y charge. It is a reasonable price point for the market."

**🤖 AI Agent:**
> VALUE_METRIC_UNDEFINED — 'Per seat because competitors use per seat' is not a value metric. Does each additional seat generate independent value? For an analytics platform, value comes from data processed — a 5-person team generating $2M in insights should pay differently than one checking dashboards weekly. Also: WTP_UNRESEARCHED — 'what competitors charge' is copying, not research. Run Van Westendorp on 100+ prospects.

---

**👤 You:**
> "Value metric: events processed — each event represents a user action tracked, more events = more behavioral data = more value. Van Westendorp on 142 product managers: acceptable range $0.001-0.003/event, optimal $0.002. Anchored to current Segment/Mixpanel spend ($300-800/month for same volume). Segments: Segment A — growth-stage SaaS (50K-500K events/month), price sensitivity high, target $150-400/month. Segment B — enterprise (5M-50M events/month), price insensitive, value = compliance + real-time, target $2,000-8,000/month. Fencing: volume tiers + SLA + data retention. Unit economics: CAC $420 (content + PLG), LTV Seg A $4,200 (24mo × $175), LTV Seg B $72,000 (36mo × $2,000), LTV/CAC 10x/171x, payback 2.4mo/0.2mo, gross margin 82%. Packaging: Free (10K events/month, 30-day retention, community support) → Growth ($0.002/event, 1-year retention, email support, upgrade trigger: hitting 10K limit) → Enterprise (volume discount, unlimited retention, SLA, dedicated CSM, upgrade trigger: compliance/real-time requirements)."

**🤖 AI Agent:**
> PRICING_PROVEN — Rigorous pricing strategy validated. Value metric: events processed, scaling with customer behavioral data value. WTP: Van Westendorp on 142 PMs with $0.002 optimal, anchored to Segment/Mixpanel spend. Segments: growth-stage ($150-400) vs. enterprise ($2,000-8,000) with volume/SLA/retention fencing. Unit economics: LTV/CAC 10x-171x, payback under 3 months, 82% margin. Packaging: free tier limited to 10K events (upgrade trigger), enterprise adds compliance/SLA. This pricing survives board scrutiny.

---

**👤 You:**
> "Value metric: active contacts stored. More contacts = more value for CRM. WTP: 85 interviews, acceptable range $0.05-0.10/contact/month. Segments: Segment A — solopreneurs (500-2K contacts, $25-50/month). Segment B — agencies (10K-50K contacts, $200-800/month). Fencing by contact limit. Unit economics: CAC $290, LTV solopreneur $600 (12mo avg retention), LTV agency $7,200 (18mo), LTV/CAC 2.1x / 24.8x, payback solopreneur 5.8mo, agency 0.7mo. Gross margin 76%. Packaging: Free (250 contacts), Growth ($0.08/contact), Agency (volume discount)."

**🤖 AI Agent:**
> UNIT_ECONOMICS_BROKEN — Value metric, WTP, and segmentation pass. But unit economics fail for Segment A: LTV/CAC of 2.1x is below the 3x threshold. Solopreneur segment has 12-month retention at $50/month = $600 LTV against $290 CAC. Options: (1) reduce solopreneur CAC to under $200 via PLG/referral, (2) increase retention to 18+ months via engagement loops, (3) increase ARPU to $65+/month, or (4) deprioritize solopreneurs and focus acquisition on agencies where LTV/CAC is 24.8x.


## ❓ FAQ

**Q: Does it calculate prices?**
No. It validates that your pricing strategy is grounded in value metrics, WTP research, segmentation, unit economics, and packaging design. It does not generate prices — it forces you to prove you derived them from data, not competitor pages.

**Q: What is Van Westendorp PSM?**
The Price Sensitivity Meter asks 4 questions: at what price is it too cheap (quality doubt), a bargain (great value), getting expensive (think twice), too expensive (never buy). The intersections define the acceptable price range. It requires 100-300 respondents from your target segment to produce reliable data.

**Q: Can early-stage startups use this before having revenue data?**
Yes. Pre-revenue startups use proxy data: Van Westendorp on 30+ prospect interviews, competitor pricing as anchor (not source), current workaround spend as floor, and projected CAC from channel tests. Unit economics use conservative assumptions. The tool forces you to document assumptions instead of skipping the analysis.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pricing-strategy-prover](https://vinkius.com/mcp/pricing-strategy-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pricing Strategy Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pricing-strategy-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pricing Strategy Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pricing-strategy-prover": {
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

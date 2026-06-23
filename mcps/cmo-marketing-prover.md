# CMO Marketing Prover MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cmo-marketing-prover)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

A CMO asked an AI for positioning. It said 'better and faster.' It proposes 'scale the ads' without a payback model. It trusts platform attribution 100%. It designs frictionless funnels that generate garbage leads. That is not marketing — that is a tactical wishlist. This tool forces five CMO-level marketing axes: category positioning, CAC payback physics, dark social attribution, intentional funnel friction, and budget allocation.

## Description
## The Problem

Every LLM commits five marketing reasoning failures:
1. **Positioning Weakness** — says 'better/faster' instead of creating a category.
2. **CAC Blindness** — proposes 'scale ads' without payback modeling.
3. **Attribution Naivety** — trusts platform dashboards 100%, ignoring dark social.
4. **Friction Absence** — designs frictionless funnels generating garbage leads.
5. **Budget Confusion** — allocates 100% to performance, zero to brand.

### The 5 Marketing Axes

| Axis | Pivot | Rule |
|---|---|---|
| **Category Positioning** | Polarized | Create category or name enemy — not 'better.' |
| **CAC Payback** | Calculated | CAC, LTV, payback months, diminishing returns. |
| **Attribution** | Dark Social | Self-reported + platform + incrementality. |
| **Funnel Friction** | Intentional | Pricing visible, work email, use case gate. |
| **Budget** | Split Defined | Brand + Performance + Experimental. |

### Verdict Matrix

```
Axis 1 fails → POSITIONING_WEAK
Axis 2 fails → CAC_PHYSICS_BLIND
Axis 3 fails → ATTRIBUTION_NAIVE
Axis 4 fails → FUNNEL_UNQUALIFIED
Axis 5 fails → BUDGET_MISALLOCATED
All pass     → MARKETING_PROVEN
```


## Available Tools (1)
- **validate_cmo_marketing**: Think like a wartime CMO — not vanity metrics, not "brand awareness," but revenue-accountable marketing with mathematical discipline. You must: (1) polarize POSITIONING — create a category or name an enemy. "Better/faster" is a feature comparison, not a market position. "We created Revenue Intelligence. The enemy is spreadsheet forecasting." Category creation makes you the default. Feature comparison makes you #2, (2) model CAC PHYSICS — calculate CAC by channel (not blended only), LTV with retention curve, payback period, and the DIMINISHING RETURN THRESHOLD — the spend level where incremental CAC exceeds LTV. "Scale the ads" without a ceiling is how you burn cash, (3) acknowledge DARK SOCIAL — platform attribution (Google, Meta, LinkedIn) takes credit for organic. "How did you hear about us?" (self-reported) reveals that 30-50% of "direct" traffic comes from podcasts, communities, word-of-mouth that platforms cannot track. UTMs do NOT track everything — implement self-reported attribution and weight it alongside platform data, (4) add FUNNEL FRICTION — intentional barriers that disqualify bad leads. Visible pricing filters budget mismatches. Work-email-only filters tire-kickers. Use-case dropdown routes to the right rep. "Seamless funnel" sounds good but generates garbage that burns 80% of sales capacity on unqualified leads, (5) define BUDGET SPLIT — Brand (30-40%: long-term memory, trust, category association), Performance (50-60%: short-term capture, demand harvesting), Experimental (10%: new channels, A/B tests). "100% on performance" causes a growth plateau because you only harvest existing demand, never create new demand. If the tool rejects, the marketing plan is a tactical wishlist, not a strategy.

Structured reflection tool for wartime CMO-level marketing strategy validation. Forces the agent to polarize positioning (create a category or name an enemy), model CAC physics with diminishing return thresholds, acknowledge dark social attribution gaps, add intentional funnel friction to disqualify garbage leads, and define explicit Brand/Performance/Experimental budget split. Catches Positioning Weakness (saying "better/faster" instead of creating a category or naming an enemy), CAC Blindness (scaling ads without payback modeling or diminishing return thresholds), Attribution Naivety (trusting platform dashboards 100%, ignoring dark social — podcasts, word-of-mouth, communities that platforms classify as "direct"), Friction Absence (seamless funnels generating garbage leads that burn sales capacity), and Budget Confusion (100% performance spend, zero brand — guaranteeing a growth plateau). Call once per marketing strategy evaluation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CMO Marketing Prover** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "We are better and faster than competitors. We will scale ads. Google Analytics tracks everything. Our funnel is frictionless. 100% budget on paid ads."

**🤖 AI Agent:**
> POSITIONING_WEAK — Five fatal gaps: generic positioning, no payback model, platform trust, no friction, no brand investment.

---

**👤 You:**
> "Created 'Revenue Intelligence' category. Enemy: spreadsheet forecasting. CAC $340, LTV $4,200, payback 2.8mo. Self-reported: 38% dark social. Gates: pricing visible, work email, use case. Brand 30%, Performance 60%, Experimental 10%."

**🤖 AI Agent:**
> MARKETING_PROVEN — Strategy validated. All five axes pass. Execute.

---

**👤 You:**
> "Our brand awareness is 45% in our target segment but conversion from awareness to trial is only 2.1%. Competitors average 8%. Content is producing 200K monthly impressions."

**🤖 AI Agent:**
> Awareness-to-trial gap indicates messaging-market mismatch. Impressions without conversion is vanity content. Audit the gap: is the value proposition clear in 5 seconds? Is the CTA friction-free? Test 3 positioning variants against conversion, not impressions.


## ❓ FAQ

**Q: Why does it reject 'better and faster'?**
'Better' and 'faster' are feature comparisons, not positioning. A wartime CMO creates a category or names an enemy. Polarize the market — make people choose a side.

**Q: What is dark social?**
Word-of-mouth that platform attribution cannot track. Meta and Google take credit for conversions driven by podcasts, Slack mentions, and private DMs. Self-reported attribution ('How did you hear about us?') reveals the truth.

**Q: Why add friction to funnels?**
Frictionless funnels generate garbage leads that burn sales capacity. Intentional friction — visible pricing, work email gates, use case selection — disqualifies bad fits before they reach Sales.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cmo-marketing-prover](https://vinkius.com/mcp/cmo-marketing-prover)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CMO Marketing Prover** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cmo-marketing-prover` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CMO Marketing Prover** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cmo-marketing-prover": {
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

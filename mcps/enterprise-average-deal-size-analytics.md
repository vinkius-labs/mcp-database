# Enterprise Average Deal Size Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-average-deal-size-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Analyze average deal size, segment breakdowns, and upsell opportunities.

## Description
This MCP server provides deep analytical insights into sales performance by calculating Average Deal Size (ADS) across various dimensions. Use `get_aggregate_ads` to find the total mean deal value, `get_segment_ads_analysis` to compare performance between SMB, Mid-Market, and Enterprise tiers, and `get_product_mix_impact` to see how product distribution affects revenue. It also identifies expansion potential via `get_upsell_opportunity_report` and measures pricing pressure with `get_discount_sensitivity_analysis`.


## Available Tools (5)
- **get_aggregate_ads**: Calculates the total average deal size across all provided deal data
- **get_discount_sensitivity_analysis**: Measures how heavily discounts are impacting the realized ADS
- **get_product_mix_impact**: Evaluates how the distribution of different products influences the total ADS
- **get_segment_ads_analysis**: Breaks down the average deal size by specific customer segments
- **get_upsell_opportunity_report**: Identifies specific accounts or deal types where the current value is significantly lower than the segment potential


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Average Deal Size Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is our current average deal size across all closed deals?"

**🤖 AI Agent:**
> The current average deal size is $45,000 across 120 closed deals.

---

**👤 You:**
> "Show me the ADS breakdown by customer segment."

**🤖 AI Agent:**
> The segment breakdown is: Enterprise: $120,000 (15 deals), Mid-Market: $45,000 (50 deals), and SMB: $12,000 (55 deals).

---

**👤 You:**
> "Are there any high-priority upsell opportunities in our pilot accounts?"

**🤖 AI Agent:**
> Yes, there are 3 high-priority opportunities from pilot conversions with a total potential upsell value of $85,000.


## ❓ FAQ

**Q: How does this tool handle multi-year contracts?**
You can use the `get_aggregate_ads` tool with the `isNormalized` parameter set to true to convert multi-year contract values into their annual equivalent for accurate comparison.

**Q: Can I identify high-priority expansion targets?**
Yes, the `get_upsell_opportunity_report` tool identifies accounts where the current deal value is below segment benchmarks, prioritizing pilot conversions as high-priority opportunities.

**Q: How is the impact of discounts measured?**
The `get_discount_sensitivity_analysis` tool calculates the average discount percentage and the total reduction impact on the realized ADS compared to list prices.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-average-deal-size-analytics](https://vinkius.com/ai-agent-connect/enterprise-average-deal-size-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Average Deal Size Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-average-deal-size-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Average Deal Size Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-average-deal-size-analytics": {
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

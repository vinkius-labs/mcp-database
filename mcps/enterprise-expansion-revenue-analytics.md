# Enterprise Expansion Revenue Analytics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/enterprise-expansion-revenue-analytics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Analyze land-and-expand efficiency with detailed expansion revenue metrics.

## Description
This MCP server provides specialized financial analytics to evaluate the efficiency of land-and-expand sales strategies. It allows AI agents to calculate expansion rates, decompose revenue mixes, and assess the health of growth drivers. Use `calculate_expansion_metrics` to get a full performance summary, `get_expansion_mix_distribution` to see how revenue is distributed across levers, `evaluate_land_and_expand_health` to identify strategic risks, and `get_expansion_opportunity_score` to forecast future growth potential based on current patterns.


## Available Tools (4)
- **get_expansion_mix_distribution**: Answers "How is our expansion revenue distributed across different growth levers?"
- **evaluate_land_and_expand_health**: Answers "Is our land-and-expand strategy balanced or over-reliant on a single driver?"
- **calculate_expansion_metrics**: Provides a comprehensive summary of expansion performance and the revenue composition
- **get_expansion_opportunity_score**: Answers "What is the potential for future growth based on current expansion patterns?"


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Enterprise Expansion Revenue Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate expansion metrics for a customer with 100000 existing ARR, 20000 upsell, 15000 cross-sell, 5000 seat expansion, and 10000 price increase."

**🤖 AI Agent:**
> The total expansion revenue is 50,000, resulting in an expansion rate of 50%. The revenue mix is 40% upsell, 30% cross-sell, 10% seat expansion, and 20% price increase, with an opportunity score of 0.85.

---

**👤 You:**
> "Is my land-and-expand strategy healthy if I have 50000 total expansion revenue, 45000 from upsells, 2000 from cross-sell, 2000 from seats, and 1000 from price increases?"

**🤖 AI Agent:**
> The strategy is rated as Concentrated with a High risk level because upsells account for 90% of the total expansion revenue.

---

**👤 You:**
> "What is the distribution of my expansion revenue if upsell is 30k, cross-sell is 20k, seat expansion is 10k, and price increase is 40k?"

**🤖 AI Agent:**
> The expansion revenue distribution is 30% upsell, 20% cross-sell, 10% seat expansion, and 40% price increase.


## ❓ FAQ

**Q: What is expansion revenue?**
Expansion revenue is the incremental revenue generated from existing customers through upsells, cross-sells, seat expansions, or price increases.

**Q: How can I check if my growth is too concentrated?**
You can use the `evaluate_land_and_expand_health` tool to determine if your expansion strategy is balanced or over-reliant on a single driver.

**Q: What does the opportunity score represent?**
The opportunity score evaluates the potential for future growth by combining current expansion momentum with the diversity of your revenue sources.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/enterprise-expansion-revenue-analytics](https://vinkius.com/ai-agent-connect/enterprise-expansion-revenue-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Enterprise Expansion Revenue Analytics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `enterprise-expansion-revenue-analytics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Enterprise Expansion Revenue Analytics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "enterprise-expansion-revenue-analytics": {
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

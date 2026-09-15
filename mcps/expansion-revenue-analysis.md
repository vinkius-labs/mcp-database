# Expansion Revenue Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/expansion-revenue-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Decompose revenue growth into expansion drivers and retention health metrics.

## Description
This MCP server provides deep financial insights into customer growth. It allows AI agents to calculate critical metrics like expansion rate and net revenue retention (NRR) by analyzing upsell, cross-sell, and price increase revenue. Using tools like `get_expansion_metrics` and `get_retention_health`, agents can identify if growth is driven by product depth or breadth and assess the stability of revenue streams.


## Available Tools (4)
- **get_expansion_metrics**: Calculates core growth and retention percentages based on revenue inputs
- **get_expansion_triggers**: Identifies the qualitative nature of growth based on revenue patterns
- **get_retention_health**: Evaluates the relationship between expansion and churn to determine if growth is healthy
- **get_revenue_mix**: Analyzes the composition of expansion revenue to understand growth drivers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Expansion Revenue Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the expansion metrics for a base revenue of 100000, upsell of 20000, cross-sell of 15000, price increase of 5000, and churn of 10000."

**🤖 AI Agent:**
> The expansion rate is 40%, the net revenue retention is 130%, the total expansion revenue is 40000, and the net growth is 30000.

---

**👤 You:**
> "What is the revenue mix if upsell is 5000, cross-sell is 3000, and price increase is 2000?"

**🤖 AI Agent:**
> The expansion revenue consists of 50% upsell, 30% cross-sell, and 20% price increases.

---

**👤 You:**
> "Analyze the expansion triggers for upsell: 50000, cross-sell: 10000, price increase: 5000."

**🤖 AI Agent:**
> The primary driver is Product Depth, the growth strategy focuses on usage-based expansion, and the stability index is High.


## ❓ FAQ

**Q: How does this tool calculate Net Revenue Retention (NRR)?**
NRR is calculated by adding total expansion revenue to the base revenue, subtracting churn revenue, and dividing the result by the base revenue using the `get_expansion_metrics` tool.

**Q: Can I identify my primary growth driver?**
Yes, the `get_expansion_triggers` tool identifies whether your primary driver is Product Depth, Product Breadth, or Pricing Optimization.

**Q: What is the difference between upsell and cross-sell in these metrics?**
Upsell refers to upgrades in tiers or seat counts, while cross-sell refers to the purchase of entirely new products. Both are analyzed via `get_revenue_mix`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/expansion-revenue-analysis](https://vinkius.com/en/ai-agent-connect/expansion-revenue-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Expansion Revenue Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `expansion-revenue-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Expansion Revenue Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "expansion-revenue-analysis": {
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

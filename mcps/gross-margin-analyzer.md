# Gross Margin Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gross-margin-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate product gross margins, identify underperforming products against industry benchmarks, and simulate COGS reduction impact.

## Description
The Gross Margin Analyzer is a financial diagnostic tool designed to evaluate product profitability. It allows you to compute gross margins for multiple products using `calculate_product_margins`, identify which items are falling below industry-specific thresholds with `detect_underperforming_products` (supporting SaaS, Marketplace, and Hardware benchmarks), and forecast the impact of cost optimization strategies via `simulate_cogs_savings_impact`.


## Available Tools
- **calculate_product_margins**: Compute the current profitability margin for a provided list of products
- **detect_underperforming_products**: Identify products failing to meet industry minimum profitability thresholds
- **simulate_cogs_savings_impact**: Forecast projected gross margin improvement from COGS reduction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gross Margin Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate margins for products A and B with revenue 100/cogs 30 and revenue 200/cogs 50."

**🤖 AI Agent:**
> Product A: 70.0%, Product B: 75.0%

---

**👤 You:**
> "Which of these products are underperforming in the SaaS industry? Margins: A (80%), B (65%)."

**🤖 AI Agent:**
> Product B is at risk because its margin of 65% is below the SaaS threshold of 70%.

---

**👤 You:**
> "If I reduce COGS by 10% for a product with 50 revenue and 40 COGS, what is the new margin?"

**🤖 AI Agent:**
> The projected gross margin will be 64.0%, an increase of 4.0 percentage points.


## ❓ FAQ

**Q: What industry benchmarks are used?**
The tool uses hardcoded thresholds: SaaS (70%+), Marketplace (20-40%), and Hardware (40-60%).

**Q: Can I use this for multiple products at once?**
Yes, the `calculate_product_margins` tool accepts an array of product objects to process them in a single call.

**Q: What happens if I provide an unknown industry type?**
The `detect_underperforming_products` tool will return an error stating that no benchmark exists for the provided category.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gross-margin-analyzer](https://vinkius.com/mcp/gross-margin-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gross Margin Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gross-margin-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gross Margin Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gross-margin-analyzer": {
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

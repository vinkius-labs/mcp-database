# UK ONS Economy — GDP, Inflation & Consumer Spending MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uk-ons-economy-gdp-inflation-consumer-spending)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Official UK economic data: quarterly and annual GDP by region, CPIH inflation (the UK's headline measure), retail sales index, real-time card spending indicators, and household income statistics from the Office for National Statistics.

## Description
Official UK economic statistics from the ONS.

### What you can do
- **GDP** — Quarterly and annual, by region
- **CPIH** — The UK's headline inflation measure (including housing)
- **Retail Sales** — Monthly consumer spending volumes
- **Card Spending** — Experimental real-time debit/credit indicator
- **Tax & Benefits** — Household income redistribution

### No API Key Required
Completely open and unrestricted.


## Available Tools (6)
- **get_gdp**: Main datasets: regional-gdp-by-quarter (quarterly), regional-gdp-by-year (annual). Covers England, Wales, and 9 English regions. Use time=* for the full time series.

Get UK GDP data — quarterly and annual, by region and sector
- **get_cpih**: Dataset: cpih01. The headline UK inflation measure used by the ONS. Filter by aggregate (cpih1dim1A0 = all items) and geography (K02000001 = UK).

Get UK inflation (CPIH) — the official consumer prices index including housing costs
- **get_retail_sales**: Dataset: retail-sales-index. Monthly data showing value and volume of retail sales in Great Britain. Base year 2019=100. Seasonally and non-seasonally adjusted.

Get UK retail sales index — value and volume of consumer spending
- **get_spending_cards**: Dataset: uk-spending-on-cards. Weekly data providing near real-time insight into consumer spending patterns.

Get UK debit and credit card spending — experimental real-time indicator
- **get_tax_benefits**: Dataset: tax-benefits-statistics. Shows redistribution effects of direct and indirect taxation and benefits in cash or kind.

Get the effects of taxes and benefits on UK household income
- **get_economy_dataset**: Common IDs: regional-gdp-by-quarter, cpih01, retail-sales-index, uk-spending-on-cards. Use get_dimensions to discover available filters.

Query any ONS economy dataset by ID with flexible filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UK ONS Economy — GDP, Inflation & Consumer Spending** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current UK inflation rate?"

**🤖 AI Agent:**
> 📊 **UK Inflation (CPIH)**

Latest: 3.2% (February 2026)
Previous: 3.4% (January 2026)

CPIH (Consumer Prices Index including owner occupiers' housing costs) is the ONS's headline inflation measure.

Key components:
- Food & non-alcoholic beverages: 4.1%
- Housing & household services: 5.8%
- Transport: 1.2%

Source: ONS, dataset cpih01

---

**👤 You:**
> "Show me UK GDP by region"

**🤖 AI Agent:**
> 🇬🇧 **UK Regional GDP (Q3 2025)**

| Region | Growth (QoQ) |
|--------|-------------|
| London | +0.4% |
| South East | +0.3% |
| North West | +0.2% |
| Scotland | +0.1% |
| Wales | -0.1% |

UK Total: +0.3% quarterly growth


## ❓ FAQ

**Q: What is CPIH?**
CPIH (Consumer Prices Index including owner occupiers' housing costs) is the UK's most comprehensive inflation measure. Unlike CPI, it includes housing costs for homeowners. The ONS considers CPIH its headline measure of inflation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uk-ons-economy-gdp-inflation-consumer-spending](https://vinkius.com/mcp/uk-ons-economy-gdp-inflation-consumer-spending)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UK ONS Economy — GDP, Inflation & Consumer Spending** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `uk-ons-economy-gdp-inflation-consumer-spending` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UK ONS Economy — GDP, Inflation & Consumer Spending** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "uk-ons-economy-gdp-inflation-consumer-spending": {
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

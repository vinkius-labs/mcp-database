# U.S. Census Income — Median Income, Poverty & Economy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-census-income-median-income-poverty-economy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Explore economic indicators across America using Census and CBP data. Get median household income, poverty rates, educational attainment, business establishments, employees, and payroll for any state or county.

## Description
U.S. Census economic data.

### 4 Tools
- **Income by State** — Median income & poverty rates
- **Income by County** — Drill down into local economies
- **Education by State** — Bachelor's degree attainment
- **Business Patterns** — County-level business activity

### Authentication
Requires a free API key from the Census Bureau.


## Available Tools (4)
- **get_income_by_state**: Median income is the single most-used economic indicator from the Census — it determines federal funding, cost-of-living adjustments, and market opportunity analysis.

Get median household income and poverty rates for all states
- **get_income_by_county**: Critical for real estate analysis, business site selection, and understanding economic disparity within a state.

Get median household income and poverty for all counties in a state
- **get_education_by_state**: Education level is a key predictor of income, employment, and economic development.

Get educational attainment for all states — bachelor's degree or higher
- **get_business_patterns**: From County Business Patterns (CBP) — the definitive dataset for understanding local economic activity and business concentration.

Get County Business Patterns — establishments, employees, and payroll by county


## 💬 Prompt Examples

Here are some examples of how you can interact with the **U.S. Census Income — Median Income, Poverty & Economy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the median household income in New York state?"

**🤖 AI Agent:**
> 📊 **U.S. Census Bureau: Income & Poverty by State**

**New York (36):**
- Median Household Income: $79,557
- Total Population in Poverty: 2,750,917
- Poverty Rate: 13.9%

---

**👤 You:**
> "Compare poverty levels down the counties of Illinois"

**🤖 AI Agent:**
> 📊 **Income & Poverty — State 17**

- Cook County (17-031): Median Income $78,304 | Poverty Rate 14.2%
- DuPage County (17-043): Median Income $107,035 | Poverty Rate 6.5%
- Lake County (17-097): Median Income $104,553 | Poverty Rate 7.2%

---

**👤 You:**
> "Show the business patterns for restaurants in Texas"

**🤖 AI Agent:**
> 📊 **Business Patterns — State 48**

Data for Texas (48) Counties:
- Harris County: 110,482 establishments, 2,510,954 employees
- Dallas County: 72,111 establishments, 1,732,490 employees
- Travis County: 41,832 establishments, 856,120 employees


## ❓ FAQ

**Q: What is County Business Patterns (CBP)?**
CBP is an annual series that provides subnational economic data by industry. This server uses it to return total business establishments, employees, and annual payroll by county.

**Q: Does income include taxes?**
Median household income reported by the Census represents pre-tax (gross) income from all sources.

**Q: Can it separate individual vs household income?**
The primary metrics fetched here are Household metrics as they give the highest fidelity snapshot of local living conditions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-census-income-median-income-poverty-economy](https://vinkius.com/mcp/us-census-income-median-income-poverty-economy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **U.S. Census Income — Median Income, Poverty & Economy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-census-income-median-income-poverty-economy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **U.S. Census Income — Median Income, Poverty & Economy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-census-income-median-income-poverty-economy": {
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

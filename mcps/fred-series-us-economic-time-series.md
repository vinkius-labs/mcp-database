# FRED Series — U.S. Economic Time Series MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fred-series-us-economic-time-series)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Search and retrieve data from 816,000+ official U.S. economic time series: GDP, inflation, unemployment, interest rates, money supply — with built-in transformations, frequency aggregation, and vintage analysis.

## Description
Connect your AI agent to the **most powerful economic data engine in the world**. FRED Series gives you direct access to the Federal Reserve's complete time series database.

### What you can do
- **Search 816,000+ Series** — Find any economic indicator by keyword. GDP, CPI, unemployment rate, federal funds rate, housing starts, and hundreds of thousands more
- **Retrieve Observations** — Get actual date/value pairs with built-in unit transformations (percent change, log, year-over-year) and frequency aggregation (daily → monthly → quarterly → annual)
- **Series Metadata** — Full details: title, units, frequency, seasonal adjustment, observation range, source, and notes
- **Recent Updates** — Monitor which series were just updated — essential for tracking economic releases
- **Vintage Analysis** — Access ALFRED-style historical revisions to understand how data was revised over time

### Popular Series IDs
`GDP` · `UNRATE` · `CPIAUCSL` · `FEDFUNDS` · `DGS10` · `SP500` · `M2SL` · `MORTGAGE30US` · `DEXUSEU` · `T10YIE`

### Who is this for?
Quantitative analysts, economists, financial advisors, portfolio managers, data journalists, academic researchers, and anyone building AI agents that need authoritative U.S. economic data.


## Available Tools
- **search_series**: Returns matching series with title, frequency, units, popularity. Use order_by=popularity to find the most-used series. Examples: "GDP", "unemployment rate", "inflation CPI".

Search 816,000+ economic time series by keyword
- **get_series**: Use well-known IDs like GDP, UNRATE, CPIAUCSL, FEDFUNDS, DGS10, SP500, M2SL.

Get metadata for a specific FRED series
- **get_observations**: Supports date filtering, unit transformations (percent change, log, etc.), and frequency aggregation. This is the primary tool for retrieving economic data.

Get actual data values for a FRED time series
- **get_series_updates**: Useful for monitoring new data releases. Filter by macro (large/popular series) or regional.

Get recently updated FRED series
- **get_vintage_dates**: Essential for ALFRED-style vintage analysis and understanding data revisions.

Get historical revision dates for a series


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FRED Series — U.S. Economic Time Series** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current U.S. unemployment rate?"

**🤖 AI Agent:**
> 📊 **U.S. Unemployment Rate (UNRATE)**

Latest: 3.7% (January 2025)
Previous: 3.7% (December 2024)
Frequency: Monthly, seasonally adjusted

12-month trend: Stable around 3.5-3.9%
Historical low: 2.5% (May 1953)
Pandemic peak: 14.7% (April 2020)

The labor market remains tight by historical standards.

---

**👤 You:**
> "Show me U.S. GDP growth rate over the last 5 years"

**🤖 AI Agent:**
> 📈 **U.S. GDP — Percent Change from Previous Quarter (Annualized)**

| Year | Q1 | Q2 | Q3 | Q4 |
|------|-----|-----|-----|-----|
| 2024 | 1.4% | 3.0% | 2.8% | 2.3% |
| 2023 | 2.0% | 2.1% | 4.9% | 3.4% |
| 2022 | -1.6% | -0.6% | 3.2% | 2.6% |

Using series GDP with units=pch (percent change) and frequency=q (quarterly).

---

**👤 You:**
> "Compare the federal funds rate with 10-year Treasury yield"

**🤖 AI Agent:**
> 🏦 **FEDFUNDS vs DGS10 — Rate Comparison**

Federal Funds Rate (FEDFUNDS): 5.33%
10-Year Treasury (DGS10): 4.15%

Yield curve inversion: -118 bps
This inversion has persisted for 18+ months, historically signaling recession risk.

Both series retrieved from FRED with daily frequency.


## ❓ FAQ

**Q: How do I get a FRED API key?**
Free and instant! Go to fredaccount.stlouisfed.org/apikeys, create a free account (no credit card), click 'Request API Key', and copy the 32-character key. Takes under 60 seconds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fred-series-us-economic-time-series](https://vinkius.com/mcp/fred-series-us-economic-time-series)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FRED Series — U.S. Economic Time Series** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `fred-series-us-economic-time-series` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FRED Series — U.S. Economic Time Series** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fred-series-us-economic-time-series": {
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

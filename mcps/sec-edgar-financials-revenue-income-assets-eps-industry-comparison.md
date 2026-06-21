# SEC EDGAR Financials — Revenue, Income, Assets, EPS & Industry Comparison MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sec-edgar-financials-revenue-income-assets-eps-industry-comparison)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sec-edgar-financials-revenue-income-assets-eps-industry-comparison-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sec-edgar-financials-revenue-income-assets-eps-industry-comparison-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-intelligence](../categories/data-intelligence.md)

Extract XBRL financial data from SEC filings: revenue, net income, total assets, liabilities, stockholders' equity, EPS, and cash for any U.S. public company. Compare financial metrics across all companies industry-wide using XBRL frames. Like a free mini-Bloomberg terminal.

## Description
SEC XBRL financial data.

### 4 Tools
- **Key Financials** — Revenue, income, assets, EPS, cash
- **Financial Metric** — Any US-GAAP concept
- **All Facts** — Complete XBRL data dump
- **Industry Comparison** — Cross-company metric frames

### Zero Auth
### Like a free Bloomberg terminal


## Available Tools
- **get_key_financials**: Returns the most recent 5 reported values across 10-K and 10-Q filings. This is like a mini Bloomberg terminal — for free.

Get key financial data for a company — revenue, net income, assets, equity, EPS, cash
- **get_financial_metric**: Common concepts: Revenues, NetIncomeLoss, Assets, Liabilities, StockholdersEquity, EarningsPerShareBasic, LongTermDebt, ResearchAndDevelopmentExpense, CashAndCashEquivalentsAtCarryingValue, CommonStockSharesOutstanding. If the concept is not found, returns available concepts.

Get a specific US-GAAP financial concept for a company (e.g., Revenue, Debt, R&D)
- **get_all_company_facts**: This is the raw, comprehensive dataset — hundreds of concepts across multiple years. Use get_key_financials for a curated summary, or this for deep analysis.

Get ALL XBRL financial facts for a company — complete financial data dump
- **get_industry_comparison**: Useful for industry comparison and screening. Example: get all companies' Revenue for CY2024. Period format: CY2024 (annual), CY2024Q1 (quarterly), CY2024Q1I (instant).

Compare a financial metric across ALL companies — industry-wide XBRL frame data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SEC EDGAR Financials — Revenue, Income, Assets, EPS & Industry Comparison** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get Apple's key financial data — revenue, income, assets, and EPS"

**🤖 AI Agent:**
> 📊 **SEC EDGAR Financials: AAPL**

Apple Inc. (CIK: 0000320193)

💰 Revenue (last 5 periods):
  Q4 2025: $124.3B
  Q3 2025: $85.8B

💵 Net Income (last 5 periods):
  Q4 2025: $36.3B
  Q3 2025: $21.4B

📈 Earnings Per Share (EPS):
  Q4 2025: $2.41

---

**👤 You:**
> "What is Meta's exact Research and Development Expense?"

**🤖 AI Agent:**
> 📊 **US-GAAP Concept: ResearchAndDevelopmentExpense (Meta)**

Meta Platforms, Inc. (CIK: 0001326801)

Reported Values:
FY 2025: $52,130,000,000
FY 2024: $38,485,000,000
FY 2023: $35,338,000,000

---

**👤 You:**
> "Show me a comparison of Revenue across all companies for CY2024"

**🤖 AI Agent:**
> 🏛️ **Industry Frame: Revenues (CY2024)**

Top reporting entities for CY2024 by US-GAAP Revenues:
1. Walmart Inc: $648,125,000,000
2. Amazon.com Inc: $574,785,000,000
3. Apple Inc: $383,285,000,000


## Installation & Usage

To install and use the **SEC EDGAR Financials — Revenue, Income, Assets, EPS & Industry Comparison** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sec-edgar-financials-revenue-income-assets-eps-industry-comparison](https://vinkius.com/mcp/sec-edgar-financials-revenue-income-assets-eps-industry-comparison)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# SEC EDGAR Financials — Revenue, Income, Assets, EPS & Industry Comparison MCP Server

Extract XBRL financial data from SEC filings: revenue, net income, total assets, liabilities, stockholders' equity, EPS, and cash for any U.S. public company. Compare financial metrics across all companies industry-wide using XBRL frames. Like a free mini-Bloomberg terminal.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sec-edgar-financials-revenue-income-assets-eps-industry-comparison)

## Overview
**Category:** data-intelligence
**Tools Count:** 4

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


## Installation & Usage

To install and use the **SEC EDGAR Financials — Revenue, Income, Assets, EPS & Industry Comparison** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sec-edgar-financials-revenue-income-assets-eps-industry-comparison](https://vinkius.com/mcp/sec-edgar-financials-revenue-income-assets-eps-industry-comparison)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

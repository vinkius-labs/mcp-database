# SEC EDGAR Full — The Ultimate Free Bloomberg Alternative for AI Agents MCP Server

The definitive SEC EDGAR Mega-Server: 13 tools spanning company lookup (8,000+ tickers), all filing types (10-K, 10-Q, 8-K), insider trading (Form 4), XBRL financial data extraction (revenue, income, assets, EPS), industry-wide comparison frames, and full-text search across every document ...

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/sec-edgar-full-the-ultimate-free-bloomberg-alternative-for-ai-agents)

## Overview
**Category:** brain-trust
**Tools Count:** 13

## Description
The **ultimate SEC EDGAR Mega-Server** — 13 tools.

### 13 Tools
- 🏢 Companies (3) — Ticker lookup, search, company info
- 📄 Filings (6) — Recent, 10-K, 10-Q, 8-K, insider trades, full-text search
- 📊 Financials (4) — Key metrics, any US-GAAP concept, all facts, industry comparison

### Zero Authentication Required
### Free alternative to Bloomberg Terminal


## Available Tools
- **lookup_ticker**: g., AAPL, MSFT, TSLA) to the SEC CIK number needed for all EDGAR queries. Returns company name, CIK, and ticker. The CIK is the unique identifier SEC uses for all public companies.

Look up a company by stock ticker — get CIK, name, and ID
- **search_companies**: Returns matching companies with CIK numbers. Use this when you don't know the exact ticker.

Search SEC-registered companies by name or ticker
- **get_company_info**: Provide either a CIK number or ticker.

Get full company profile from SEC — SIC code, exchanges, filings history
- **get_recent_filings**: Includes form type, filing date, accession number, and primary document link. Results include all form types (10-K annual reports, 10-Q quarterlies, 8-K events, proxy statements, etc.).

Get the most recent SEC filings for a company — 10-K, 10-Q, 8-K, and more
- **get_annual_reports**: The 10-K is the most detailed financial disclosure — includes audited financial statements, MD&A (Management Discussion), risk factors, and business description. Required by SEC for all public companies.

Get 10-K annual reports for a company — the most comprehensive financial disclosure
- **get_quarterly_reports**: Filed 3 times per year (Q1, Q2, Q3 — Q4 is covered by the 10-K). Includes unaudited financial statements and interim MD&A.

Get 10-Q quarterly reports for a company — unaudited financial updates
- **get_8k_events**: Companies must file an 8-K within 4 business days of material events: earnings announcements, M&A, executive departures, bankruptcy, delisting, etc.

Get 8-K current reports — material events like earnings, mergers, CEO changes
- **get_insider_trades**: Shows insider buys and sells. Insider buying is often considered a bullish signal.

Get insider trading filings (Form 4) — officer and director stock transactions
- **search_filings**: Find specific topics, companies, products, or risks mentioned in any SEC document. Filter by form type (10-K, 10-Q, 8-K) and date range.

Full-text search across all SEC filings — find any keyword in any document
- **get_key_financials**: Returns the most recent 5 reported values across 10-K and 10-Q filings. This is like a mini Bloomberg terminal — for free.

Get key financial data for a company — revenue, net income, assets, equity, EPS, cash
- **get_financial_metric**: Common concepts: Revenues, NetIncomeLoss, Assets, Liabilities, StockholdersEquity, EarningsPerShareBasic, LongTermDebt, ResearchAndDevelopmentExpense, CashAndCashEquivalentsAtCarryingValue, CommonStockSharesOutstanding. If the concept is not found, returns available concepts.

Get a specific US-GAAP financial concept for a company (e.g., Revenue, Debt, R&D)
- **get_all_company_facts**: This is the raw, comprehensive dataset — hundreds of concepts across multiple years. Use get_key_financials for a curated summary, or this for deep analysis.

Get ALL XBRL financial facts for a company — complete financial data dump
- **get_industry_comparison**: Useful for industry comparison and screening. Example: get all companies' Revenue for CY2024. Period format: CY2024 (annual), CY2024Q1 (quarterly), CY2024Q1I (instant).

Compare a financial metric across ALL companies — industry-wide XBRL frame data


## Installation & Usage

To install and use the **SEC EDGAR Full — The Ultimate Free Bloomberg Alternative for AI Agents** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sec-edgar-full-the-ultimate-free-bloomberg-alternative-for-ai-agents](https://vinkius.com/mcp/sec-edgar-full-the-ultimate-free-bloomberg-alternative-for-ai-agents)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

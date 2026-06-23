# SEC EDGAR Full — The Ultimate Free Bloomberg Alternative for AI Agents MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sec-edgar-full-the-ultimate-free-bloomberg-alternative-for-ai-agents)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

The definitive SEC EDGAR Mega-Server: 13 tools spanning company lookup (8,000+ tickers), all filing types (10-K, 10-Q, 8-K), insider trading (Form 4), XBRL financial data extraction (revenue, income, assets, EPS), industry-wide comparison frames, and full-text search across every document ...

## Description
The **ultimate SEC EDGAR Mega-Server** — 13 tools.

### 13 Tools
- 🏢 Companies (3) — Ticker lookup, search, company info
- 📄 Filings (6) — Recent, 10-K, 10-Q, 8-K, insider trades, full-text search
- 📊 Financials (4) — Key metrics, any US-GAAP concept, all facts, industry comparison

### Zero Authentication Required
### Free alternative to Bloomberg Terminal


## Available Tools (13)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SEC EDGAR Full — The Ultimate Free Bloomberg Alternative for AI Agents** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Full financial analysis of NVIDIA: company info, latest 10-K, key financials, and insider trades"

**🤖 AI Agent:**
> 📊 **SEC EDGAR Full Analysis: NVDA**

🏢 NVIDIA Corp (CIK: 0001045810)
SIC: 3674 — Semiconductors

📄 Latest 10-K: Filed 2026-02-26 (FY2025)

💰 Key Financials:
  Revenue (FY2025): $130.5B
  Net Income (FY2025): $72.9B
  EPS: $2.95

👤 Recent Form 4 Trades: Colette Kress (CFO) sold 100,000 shares on 2026-03-05.

---

**👤 You:**
> "Search the entire EDGAR database for 'robotics' and provide a summary of trends"

**🤖 AI Agent:**
> 🔍 **EDGAR Full-Text Search Summary: 'robotics'**

Found 45,210 mentions in recent filings, primarily across the Manufacturing and Healthcare sectors. Companies like Intuitive Surgical (ISRG) and Amazon (AMZN) frequently cite 'robotics' in their Risk Factors and Business Strategy sections. There is a noticeable 15% increase in mentions in 2026 compared to 2025, suggesting accelerated adoption in supply chain logistics.

---

**👤 You:**
> "Compare the historical assets of Microsoft vs Apple, and check if any insiders recently sold stock."

**🤖 AI Agent:**
> 📊 **Comparative Analysis: MSFT vs AAPL**

💰 **Historical Total Assets:**
- Microsoft (CY2025): $475.2B
- Apple (CY2025): $352.5B

👤 **Recent Insider Trades (Form 4):**
- Microsoft: Satya Nadella sold 50,000 shares on 2026-03-01.
- Apple: Tim Cook sold 80,000 shares on 2026-02-15.


## ❓ FAQ

**Q: How does this compare to Bloomberg Terminal?**
Bloomberg Terminal costs $24,000/year. This MCP server provides free, direct access to the same SEC EDGAR data that Bloomberg uses as a primary source. While Bloomberg offers real-time market data, charting, and news, this server covers the fundamental financial data: company filings (10-K, 10-Q, 8-K), XBRL financial statements, insider trading, and full-text search — all for free through the SEC's official APIs.

**Q: Is this server rate-limited?**
The SEC limits API traffic to 10 requests per second. The MCP server honors these requirements by acting transparently and using a respectful User-Agent.

**Q: Is all data strictly accurate?**
Yes, the data is pulled unaltered straight from the SEC's government endpoints. Be mindful that company financial reporting itself may occasionally be updated or reclassified by the companies themselves.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sec-edgar-full-the-ultimate-free-bloomberg-alternative-for-ai-agents](https://vinkius.com/mcp/sec-edgar-full-the-ultimate-free-bloomberg-alternative-for-ai-agents)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SEC EDGAR Full — The Ultimate Free Bloomberg Alternative for AI Agents** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sec-edgar-full-the-ultimate-free-bloomberg-alternative-for-ai-agents` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SEC EDGAR Full — The Ultimate Free Bloomberg Alternative for AI Agents** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sec-edgar-full-the-ultimate-free-bloomberg-alternative-for-ai-agents": {
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

# SEC EDGAR Filings — 10-K, 10-Q, 8-K, Insider Trades & Full-Text Search MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sec-edgar-filings-10-k-10-q-8-k-insider-trades-full-text-search)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Access all SEC filings: 10-K annual reports, 10-Q quarterly reports, 8-K material event disclosures, Form 4 insider trading data, and full-text search across every document ever filed on EDGAR. Filter by company, form type, and date range.

## Description
SEC filings access.

### 6 Tools
- **Recent Filings** — All types
- **10-K** — Annual reports
- **10-Q** — Quarterly reports
- **8-K** — Material events
- **Form 4** — Insider trades
- **Full-Text Search** — Keyword search across EDGAR

### Zero Auth


## Available Tools (6)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SEC EDGAR Filings — 10-K, 10-Q, 8-K, Insider Trades & Full-Text Search** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me Tesla's latest 10-K annual report"

**🤖 AI Agent:**
> 📄 **SEC EDGAR: 10-K Annual Reports — TSLA**

Tesla, Inc. (CIK: 0001318605)

1. 10-K — Filed: 2026-01-29, Period: 2025-12-31, Document URL: https://www.sec.gov/Archives/edgar/data/1318605/...
2. 10-K — Filed: 2025-01-27, Period: 2024-12-31
...

---

**👤 You:**
> "Search SEC filings mentioning 'artificial intelligence' in 10-K reports"

**🤖 AI Agent:**
> 🔍 **EDGAR Full-Text Search: 'artificial intelligence'**

Found 12,847 results in 10-K filings

Top results:
1. NVIDIA Corp — 10-K (2026-02-26)
2. Microsoft Corp — 10-K (2025-08-02)
3. Alphabet Inc — 10-K (2026-01-30)

---

**👤 You:**
> "Get recent insider trades (Form 4) for Microsoft"

**🤖 AI Agent:**
> 👤 **Insider Trades (Form 4): MSFT**

Recent Form 4 filings for Microsoft:
1. Form 4 - Satya Nadella (2026-03-01) - Document URL: ...
2. Form 4 - Brad Smith (2026-02-15) - Document URL: ...


## ❓ FAQ

**Q: What is the difference between 10-K, 10-Q, and 8-K?**
10-K is the comprehensive annual report with audited financials (filed once/year). 10-Q is the quarterly update with unaudited financials (filed 3x/year). 8-K is a current report filed within 4 business days of material events — earnings, M&A, CEO changes, bankruptcy, etc.

**Q: What does Form 4 report?**
Form 4 must be filed by corporate insiders (officers, directors, or 10%+ shareholders) when they buy or sell their own company's stock. It reveals executive sentiment.

**Q: How far back does the full-text search go?**
The SEC EDGAR Full-Text Search generally indexes documents back to 2001, covering over two decades of corporate filings.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sec-edgar-filings-10-k-10-q-8-k-insider-trades-full-text-search](https://vinkius.com/mcp/sec-edgar-filings-10-k-10-q-8-k-insider-trades-full-text-search)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SEC EDGAR Filings — 10-K, 10-Q, 8-K, Insider Trades & Full-Text Search** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sec-edgar-filings-10-k-10-q-8-k-insider-trades-full-text-search` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SEC EDGAR Filings — 10-K, 10-Q, 8-K, Insider Trades & Full-Text Search** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sec-edgar-filings-10-k-10-q-8-k-insider-trades-full-text-search": {
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

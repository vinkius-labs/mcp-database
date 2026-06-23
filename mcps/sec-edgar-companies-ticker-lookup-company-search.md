# SEC EDGAR Companies — Ticker Lookup & Company Search MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sec-edgar-companies-ticker-lookup-company-search)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Look up any U.S. public company on SEC EDGAR: resolve stock tickers (AAPL, TSLA, MSFT) to CIK numbers, search 8,000+ registered companies by name, and retrieve full SEC registration profiles including SIC industry codes, exchanges, and fiscal year details.

## Description
SEC company lookup.

### 3 Tools
- **Ticker Lookup** — Convert ticker to CIK
- **Search** — Find companies by name/ticker
- **Company Info** — Full SEC profile

### Zero Auth


## Available Tools (3)
- **lookup_ticker**: g., AAPL, MSFT, TSLA) to the SEC CIK number needed for all EDGAR queries. Returns company name, CIK, and ticker. The CIK is the unique identifier SEC uses for all public companies.

Look up a company by stock ticker — get CIK, name, and ID
- **search_companies**: Returns matching companies with CIK numbers. Use this when you don't know the exact ticker.

Search SEC-registered companies by name or ticker
- **get_company_info**: Provide either a CIK number or ticker.

Get full company profile from SEC — SIC code, exchanges, filings history


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SEC EDGAR Companies — Ticker Lookup & Company Search** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Look up Apple on SEC EDGAR"

**🤖 AI Agent:**
> 🏢 **SEC EDGAR: AAPL**

Company: Apple Inc.
CIK: 0000320193
Ticker: AAPL
Exchange: NASDAQ
SIC: 3571 — Electronic Computers
State: CA

---

**👤 You:**
> "Search SEC registered companies containing 'micro'"

**🤖 AI Agent:**
> 🔍 **Search: micro**

- Microsoft Corp (CIK: 0000789019, Ticker: MSFT)
- MicroStrategy Inc (CIK: 0001050446, Ticker: MSTR)
- Micron Technology Inc (CIK: 0000723125, Ticker: MU)

---

**👤 You:**
> "Get the full SEC profile for Tesla using its CIK"

**🤖 AI Agent:**
> 🏢 **SEC EDGAR: Tesla, Inc.**

CIK: 0001318605
SIC: 3711 — Motor Vehicles & Passenger Car Bodies
State: TX
Fiscal Year End: 1231


## ❓ FAQ

**Q: What is a CIK number?**
CIK (Central Index Key) is the SEC's unique identifier for every entity that files with the commission. It's a 10-digit number (zero-padded) used to access all filings, financial data, and company information on EDGAR.

**Q: Are foreign companies included?**
Yes, any company that issues securities to the U.S. public and is required to report to the SEC (including Foreign Private Issuers) will be listed in EDGAR and have a CIK.

**Q: Do I need an API key for SEC lookup?**
No, all data is accessed openly via SEC EDGAR endpoints. We only use a custom User-Agent to comply with their fairness policies.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sec-edgar-companies-ticker-lookup-company-search](https://vinkius.com/mcp/sec-edgar-companies-ticker-lookup-company-search)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SEC EDGAR Companies — Ticker Lookup & Company Search** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sec-edgar-companies-ticker-lookup-company-search` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SEC EDGAR Companies — Ticker Lookup & Company Search** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sec-edgar-companies-ticker-lookup-company-search": {
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

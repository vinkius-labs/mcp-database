# SEC EDGAR MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sec-edgar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Official US corporate filings database — access 10-K, 10-Q, and financial data via AI.

## Description
Empower your AI agent with the primary source for US corporate intelligence through the **SEC EDGAR** MCP server. This integration provides real-time access to the Securities and Exchange Commission's database of public company filings. Your agent can retrieve recent submissions (like annual 10-K and quarterly 10-Q reports), extract specific XBRL financial facts, and audit disclosures for any public entity using its Central Index Key (CIK). Whether you are conducting fundamental analysis, auditing regulatory compliance, or researching corporate history, your agent acts as a dedicated financial analyst through natural conversation.

### What you can do

- **Submission Tracking** — Retrieve the most recent filings for any public company.
- **Financial Fact Extraction** — Access structured XBRL data for balance sheets, income statements, and more.
- **Concept Lookup** — Fetch company disclosures for specific financial concepts across multiple years.
- **Entity Identification** — Use CIKs to precisely target data for specific public entities.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access with User-Agent)
3. Start querying corporate filings from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Financial Analysts** — quickly pull data for valuation models and trend analysis.
- **Investors** — monitor recent filings and earnings reports for their portfolio companies.
- **Legal & Compliance Officers** — verify public disclosures and regulatory adherence.
- **Academic Researchers** — access raw financial data for corporate governance and economic studies.


## Available Tools
- **get_company_concept**: g., Assets, Liabilities).

Get a specific financial concept for a company
- **get_company_facts**: Get financial facts for a company
- **get_submissions**: ) for a company using its Central Index Key (CIK).

Get recent submissions for a company


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SEC EDGAR** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get recent submissions for Apple Inc (CIK 0000320193)."

**🤖 AI Agent:**
> Retrieving recent filings for Apple... I found the latest submissions including their most recent 10-Q and several 8-K reports. Would you like to see the details of a specific form?

---

**👤 You:**
> "Extract the 'NetIncomeLoss' for Microsoft (CIK 0000789019) for the last 3 years."

**🤖 AI Agent:**
> Fetching financial facts for Microsoft... I've retrieved the Net Income figures from their official XBRL filings for the last 3 fiscal years. Microsoft reported $72.3B in 2023, $61.2B in 2022, and $61.3B in 2021.

---

**👤 You:**
> "Find all filings for Tesla (CIK 0001318605) related to '8-K' forms this year."

**🤖 AI Agent:**
> Filtering Tesla submissions... I've identified 5 '8-K' (current report) filings for Tesla so far this year. These usually cover major corporate events. Would you like to see the items disclosed in the most recent one?


## ❓ FAQ

**Q: How do I find the CIK for a company like Apple?**
You can search for a company's CIK on the official SEC website or ask your agent to find it. For Apple, the CIK is '0000320193'. Remember to use the leading zeros if necessary.

**Q: Can I see the latest 10-K filing for a specific entity?**
Yes! Use the `get_submissions` tool with the company's CIK. The response will list the most recent filings, and you can identify the 10-K report among them.

**Q: What is XBRL data?**
XBRL (eXtensible Business Reporting Language) is a standardized format for business reporting. It allows the SEC and analysts to extract specific financial facts (like Net Income) from filings programmatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sec-edgar](https://vinkius.com/mcp/sec-edgar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SEC EDGAR** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sec-edgar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SEC EDGAR** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sec-edgar": {
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

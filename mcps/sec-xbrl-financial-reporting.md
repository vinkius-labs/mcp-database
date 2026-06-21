# SEC XBRL (Financial Reporting) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sec-xbrl-financial-reporting)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access real-time SEC EDGAR financial data — query filing histories, company facts, and XBRL disclosures directly from any AI agent.

## Description
Connect your AI agent to the **SEC EDGAR** database and perform deep financial analysis using standardized XBRL data. This server provides programmatic access to the U.S. Securities and Exchange Commission's public filing infrastructure.

### What you can do

- **Filing History** — Retrieve the complete submission history for any entity using its Central Index Key (CIK)
- **Company Facts** — Fetch the entire dictionary of XBRL facts reported by a company, covering all taxonomies (US-GAAP, IFRS, etc.)
- **Concept Analysis** — Drill down into specific financial concepts (e.g., Net Income, Assets) for a single company over time
- **Market-Wide Frames** — Aggregate specific financial data points across all reporting entities for a particular period and unit

### How it works

1. Subscribe to this server
2. Enter your SEC User-Agent string (required by SEC Fair Access policy)
3. Start querying financial statements from Claude, Cursor, or any MCP client

### Who is this for?

- **Financial Analysts** — instantly pull raw XBRL data for modeling without manual spreadsheet entry
- **Investors** — monitor recent filings and compare metrics across industries using standardized frames
- **Compliance Officers** — verify submission histories and disclosure accuracy for specific CIKs


## Available Tools
- **get_company_concept**: Get all XBRL disclosures for a single company concept
- **get_company_facts**: Get all company concepts data for a specific company
- **get_submissions**: Includes metadata and recent filings.

Get filing history for a specific entity
- **get_xbrl_frames**: Get aggregated facts for a specific concept and period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SEC XBRL (Financial Reporting)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the filing history for Microsoft using CIK 789019."

**🤖 AI Agent:**
> I've retrieved the submissions for Microsoft Corp. Recent filings include their latest 10-K and several 8-K reports. Would you like to see the details of the most recent annual report?

---

**👤 You:**
> "Show me all XBRL facts reported by Apple (CIK 320193)."

**🤖 AI Agent:**
> Fetching company facts for Apple Inc... I have access to all reported concepts across US-GAAP and DEI taxonomies. This includes assets, liabilities, and revenue data points. Which specific metric should we analyze?

---

**👤 You:**
> "Compare the 'AccountsPayableCurrent' for all companies in USD for the period CY2023Q3."

**🤖 AI Agent:**
> Aggregating XBRL frames for Accounts Payable (Current) in Q3 2023... I've compiled the data for all reporting entities. For example, Entity A reported $5.2B while Entity B reported $1.1B. Would you like a summary of the top 10 entities by this metric?


## ❓ FAQ

**Q: How do I find the filing history for a specific company?**
Use the `get_submissions` tool with the company's Central Index Key (CIK). For example, Apple is 320193. The tool automatically handles leading zeros.

**Q: Can I retrieve specific financial metrics like 'Net Income' for a company?**
Yes. Use `get_company_concept` by providing the CIK, the taxonomy (usually 'us-gaap'), and the XBRL tag (like 'NetIncomeLoss').

**Q: How can I compare a single metric across all companies for a specific year?**
Use the `get_xbrl_frames` tool. You can specify a concept, unit, and period (e.g., 'CY2023') to get data for every reporting entity in that timeframe.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sec-xbrl-financial-reporting](https://vinkius.com/mcp/sec-xbrl-financial-reporting)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SEC XBRL (Financial Reporting)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sec-xbrl-financial-reporting` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SEC XBRL (Financial Reporting)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sec-xbrl-financial-reporting": {
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

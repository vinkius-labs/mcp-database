# Salesforce Analytics & SOQL MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/salesforce-analytics-soql)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Run SOQL queries, execute reports, view dashboards, and analyze CRM data in real-time through natural conversation.

## Description
The most powerful Salesforce integration — **raw SOQL access** to any data in your org.

### What you can do
- **SOQL** — Run any query against standard or custom objects
- **Reports** — List and execute Salesforce reports
- **Dashboards** — View dashboard components and data
- **Counts** — Get record counts for any object

### Who is this for?
- **Executives** — "What was our win rate last quarter?"
- **RevOps** — Instant data without waiting for BI
- **Analysts** — Ad-hoc queries through conversation


## Available Tools
- **sf_get_dashboard**: Each component includes its type, header, data values, and the source report. Dashboards provide pre-built visual summaries. Get the dashboard ID from sf_list_dashboards. Use when the user asks "show me the sales dashboard" or wants a visual summary of specific metrics.

Get all component data from a specific Salesforce dashboard — charts, metrics, and tables with their underlying data
- **sf_record_count**: Returns the total number of records. Use for quick data volume checks: "how many leads do we have?", "total number of accounts", or capacity planning. Accepts any standard or custom object API name.

Get the total record count for any Salesforce object — Account, Contact, Lead, Opportunity, Case, or any custom object
- **sf_list_dashboards**: Returns dashboard title, folder, last referenced date, and dashboard ID. Dashboards contain visual components (charts, tables, metrics) built from reports. Use to find dashboard IDs before fetching their component data with sf_get_dashboard.

List available Salesforce dashboards with title, folder, and last referenced date to discover visualization assets
- **sf_list_reports**: Returns report name, folder path, report format (Tabular/Summary/Matrix), last run date, and report ID. Use when the user asks about available reports, wants to find a specific one, or needs report IDs before running them with sf_run_report.

List available Salesforce reports with name, folder, format, and last run date to discover reporting assets
- **sf_run_report**: Get the report ID from sf_list_reports first. This is the read-only equivalent of clicking "Run Report" in the Salesforce UI. Returns up to 2000 rows. Use when the user asks for specific report data or wants to extract insights from a saved report.

Execute a specific Salesforce report by ID and return its full data — all rows, columns, and groupings
- **sf_run_soql**: This is the most powerful and flexible tool — you can query any standard or custom object, apply filters, use aggregate functions, and join related objects. Example: SELECT Id, Name, Amount, StageName FROM Opportunity WHERE StageName = 'Closed Won' AND Amount > 10000 LIMIT 10. Use when no other tool covers the specific data need, or when the user requests a custom query.

Execute a raw SOQL query against your Salesforce org to retrieve any data from standard or custom objects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Salesforce Analytics & SOQL** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was our total revenue closed this quarter?"

**🤖 AI Agent:**
> 💰 SELECT SUM(Amount) FROM Opportunity WHERE StageName = 'Closed Won' AND CloseDate = THIS_QUARTER

**$2,340,000** closed this quarter across 47 deals

---

**👤 You:**
> "Show me all reports in the Sales folder"

**🤖 AI Agent:**
> 📊 Found 8 reports in Sales:
1. Pipeline by Stage
2. Won Deals MTD
3. Lead Conversion Rate
...

---

**👤 You:**
> "How many accounts do we have by industry?"

**🤖 AI Agent:**
> 🏢 SELECT Industry, COUNT(Id) FROM Account GROUP BY Industry

| Industry | Count |
|---|---|
| Technology | 234 |
| Financial Services | 189 |
| Healthcare | 156 |


## ❓ FAQ

**Q: Can I run any SOQL query?**
Yes! Any valid SOQL query against standard or custom objects, respecting your field-level security.

**Q: Can I run existing Salesforce reports?**
Yes — list all reports, then run any by ID. Returns full row data.

**Q: Is this safe to use?**
All queries are read-only and respect your Salesforce permissions. The SOQL tool only reads data — it cannot modify records.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salesforce-analytics-soql](https://vinkius.com/mcp/salesforce-analytics-soql)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Salesforce Analytics & SOQL** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `salesforce-analytics-soql` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Salesforce Analytics & SOQL** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "salesforce-analytics-soql": {
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

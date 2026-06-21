# UniCourt MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unicourt)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Access real-time legal data and court records — search cases, track updates, and analyze normalized attorney and judge data directly from your AI agent.

## Description
Connect your **UniCourt** account to any AI agent to streamline legal research and litigation tracking through natural language.

### What you can do

- **Case Search** — Search across millions of court cases using keyword expressions and filters
- **Automated Tracking** — Use `track_case` to monitor specific litigation and receive updates on a schedule
- **Normalized Data** — Access structured profiles for attorneys, law firms, judges, and parties to perform deep background checks
- **Document Management** — Order court documents and export case data directly into your workflow
- **Legal Analytics** — Retrieve case counts and analytics to understand litigation trends

### How it works

1. Subscribe to this server
2. Enter your UniCourt Access Token
3. Start querying legal records from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Legal Professionals** — automate case monitoring and perform quick conflict checks
- **Researchers** — gather large-scale litigation data for market analysis
- **Insurance & Finance** — assess legal risks by inspecting party histories and active court cases


## Available Tools
- **delete_pacer_credential**: Delete PACER account credentials
- **generate_token**: Generate a new UniCourt access token
- **get_case_count_analytics**: Get case count analytics by case type
- **get_case_export_callback**: Get the file URL for a completed case export
- **get_case**: Get details for a specific case
- **get_case_update_status**: Check the status of a requested case update
- **get_document_order_callback**: Get the file URL for a completed document order
- **get_norm_attorney**: Get analytics and details for a normalized attorney
- **get_norm_judge**: Get analytics and details for a normalized judge
- **get_norm_law_firm**: Get analytics and details for a normalized law firm
- **get_norm_party**: Get analytics and details for a normalized party
- **get_pacer_credential**: Retrieve current PACER account credentials status
- **import_case**: High-priority case import
- **import_pacer_case**: Import a case not in UniCourt via PACER
- **order_case_document**: Order a court document
- **request_case_export**: Request an export of case data as a ZIP file
- **request_case_update**: Request an asynchronous update for a case
- **search_cases**: g., caseName:pfizer).

Search for court cases
- **search_norm_attorney**: Search for normalized attorneys
- **search_norm_judge**: Search for normalized judges
- **search_norm_law_firm**: Search for normalized law firms
- **search_norm_party**: Search for normalized parties
- **search_pacer_case_locator**: Search PACER directly via Case Locator
- **track_case**: Automatically update cases on a schedule
- **track_norm_attorney**: Schedule recurring bar source refreshes for an attorney
- **track_norm_law_firm**: Schedule recurring source refreshes for a law firm
- **update_pacer_credential**: Manage PACER account credentials


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UniCourt** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for court cases with the keyword 'Apple Inc' and sort by filing date."

**🤖 AI Agent:**
> I've found several cases for 'Apple Inc'. The most recent ones include 'Apple Inc. vs. Epic Games' (ID: 12345) and 'State of California vs. Apple' (ID: 67890). Would you like the full details for any of these?

---

**👤 You:**
> "Set up automated tracking for case ID 1205934 with a daily refresh."

**🤖 AI Agent:**
> Case 1205934 is now being tracked. I've set the refresh window to 1 day. You will be notified of any changes in the court record for this case.

---

**👤 You:**
> "Get the professional analytics for attorney ID ATTY-98765."

**🤖 AI Agent:**
> Retrieving analytics for attorney ATTY-98765... This attorney has handled 150+ cases, primarily in Intellectual Property. Their win rate in federal courts is approximately 65%. Would you like a breakdown of their most recent cases?


## ❓ FAQ

**Q: How can I search for court cases involving a specific company?**
Use the `search_cases` tool with a query like `caseName:"Company Name"`. The agent will return a list of matching cases with their UniCourt IDs and basic details.

**Q: Can the AI automatically track a case for new updates?**
Yes! By using the `track_case` tool with a specific `caseId`, you can set up automated monitoring. You can even specify a `refreshWindow` like '1d' for daily updates.

**Q: Is it possible to get professional background data for an attorney?**
Absolutely. Use `search_norm_attorney` to find the attorney and then `get_norm_attorney` with their ID to retrieve detailed analytics and professional history.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unicourt](https://vinkius.com/mcp/unicourt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UniCourt** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `unicourt` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UniCourt** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "unicourt": {
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

# Pitchly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pitchly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Turn your firm experience data into competitive deal sheets, credentials, and pitch materials with automated content generation.

## Description
Connect your **Pitchly** account to any AI agent and take full control of your organizational experience and content orchestration through natural conversation. Pitchly is the data management platform of choice for professional services firms, and this integration allows you to retrieve workspace metadata, manage custom data tables, and update critical records (deals, bios, tombstones) directly from your chat interface.

### What you can do

- **Workspace & Table Orchestration** — List all managed workspaces and retrieve detailed table structures programmatically to ensure your data foundation is always synchronized.
- **Record Lifecycle Management** — Query, create, and update records across custom tables with detailed profile metadata directly from the AI interface to maintain high-fidelity business intelligence.
- **Content Discovery Intelligence** — Search through complex data sets for specific deals, professional bios, or tombstone data via natural language to drive better research efficiency.
- **Data Ingestion Control** — Automate the creation of new records and manage organizational metadata using simple AI commands.
- **Operational Monitoring** — Track system responses and manage workspace health to ensure your experience management is always optimized.

### How it works

1. Subscribe to this server
2. Enter your Pitchly API Key (Bearer Token) from your developer settings
3. Start managing your professional experience data from Claude, Cursor, or any MCP-compatible client

No more manual spreadsheet updates or searching through disparate databases. Your AI acts as a dedicated experience manager or data coordinator.

### Who is this for?

- **Professional Services Firms** — quickly retrieve deal summaries and monitor team experience without switching apps.
- **Marketing & BD Teams** — automate the retrieval of tombstone data and track professional bios via natural conversation.
- **Knowledge Managers** — streamline the retrieval of organizational metadata and monitor data health directly within the chat.


## Available Tools (11)
- **create_record**: Add a new record to a table
- **delete_record**: Delete a record from a table
- **get_record_details**: Get details of a specific record
- **get_table_details**: Get details of a specific table
- **get_workspace_details**: Get details of a specific workspace
- **list_fields**: List all fields in a table
- **list_table_records**: List records in a Pitchly table
- **list_tables**: List tables in a workspace
- **list_workspaces**: List all Pitchly workspaces
- **search_records**: Search records within a table
- **update_record**: Update an existing record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pitchly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all tables in my 'Corporate' workspace in Pitchly."

**🤖 AI Agent:**
> I've retrieved your tables. You have 3 active collections: 'Tombstones', 'Professional Bios', and 'Client Projects'. Which one would you like to see records for?

---

**👤 You:**
> "Show me all records in the Client Engagements table that were updated this week."

**🤖 AI Agent:**
> 14 records updated this week in "Client Engagements". Notable changes: "Acme Corp Advisory" moved from Active to Completed (partner: James Park). "TechFlow Due Diligence" updated with new financial data (3 fields modified). "Meridian M&A" added 2 new team members. 4 records had status changes, 6 had field updates, and 4 had new attachments. Most active editor: Sarah Chen with 8 modifications.

---

**👤 You:**
> "Create a new record in the Deal Pipeline table for the ScaleUp Technologies opportunity."

**🤖 AI Agent:**
> Record created in "Deal Pipeline" (ID: rec_8472). Client: ScaleUp Technologies. Stage: Qualification. Estimated Value: $340,000. Lead Partner: assigned to your team. Industry: Enterprise Software. The record has been linked to 2 existing contact records and the associated workspace "Technology Sector". Next step field set to "Initial Assessment" due in 5 business days.


## ❓ FAQ

**Q: Can my AI automatically find a specific deal record by its ID?**
Yes! Use the `get_record` tool with the Table ID and Record ID. Your agent will respond with the complete metadata for the entry, including all custom field values in seconds.

**Q: How do I find my Pitchly API Key?**
Log in to your Pitchly account, navigate to **Settings** or your **Developer Dashboard**, and you will find your unique secret API key there. You may need organization admin privileges to see it.

**Q: Does this work with custom tables?**
Absolutely. This integration dynamically lists all tables available in your workspaces, allowing the AI to interact with any custom schema you've created for deals, bios, or projects.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pitchly](https://vinkius.com/mcp/pitchly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pitchly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pitchly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pitchly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pitchly": {
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

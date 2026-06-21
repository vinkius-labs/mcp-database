# Airtable MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/airtable-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Query databases, manage records, and orchestrate workflows across your connected Airtable bases with full flexibility.

## Description
Connect your **Airtable** account to any AI agent and take full control of your low-code databases and automated data management workflows through natural conversation.

### What you can do

- **Record & Row Orchestration** — List and manage database records programmatically across any table, retrieving detailed high-fidelity metadata in real-time
- **Schema Discovery Intelligence** — Programmatically query base schemas (tables, fields, views) to ensure your agent understands your high-fidelity data structure perfectly
- **Lifecycle Data Management** — Create, update, and delete records dynamically, including handling complex field types and attachments directly through your agent
- **Communication Architecture** — Access and monitor record-level comments and threads to maintain perfectly coordinated team context within your data
- **Operational Monitoring** — Apply advanced filtering formulas and manage account-level metadata directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Personal Access Token (PAT)** from the Airtable Developer Hub
3. Start orchestrating your low-code operations from Claude, Cursor, or any MCP client

No more manual data entry or toggling between browser tabs to find specific records. Your AI acts as your dedicated database engineer and data architect.

### Who is this for?

- **Operations Teams** — instantly retrieve lead records and update statuses using natural language commands
- **Project Managers** — track project milestones and coordinate team comments without leaving your workspace
- **Developers** — integrate high-speed low-code data structures into custom AI workflows through simple AI queries


## Available Tools
- **create_airtable_records**: Must pass a JSON array of objects with a "fields" key.

Create new records
- **delete_airtable_record**: Delete a record
- **get_airtable_base_schema**: Get base schema
- **get_airtable_record**: Get a specific record
- **list_airtable_comments**: List comments on a record
- **list_airtable_records**: List records in a table
- **update_airtable_record**: Update a record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Airtable** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all records in the 'Leads' table for base 'app123XYZ'."

**🤖 AI Agent:**
> I've retrieved your leads. You currently have 15 records in table 'Leads', including 'Acme Corp' (Status: Qualified) and 'Global Tech'. Would you like the detailed high-fidelity metadata for any of these?

---

**👤 You:**
> "Create a new record in table 'app123/tbl456' with fields Name='John' and Email='john@test.com'."

**🤖 AI Agent:**
> Record created! I've successfully registered John (ID: rec1024) in specified table. The high-fidelity data is now live in your Airtable base. Shall I check for any existing comments on this lead?

---

**👤 You:**
> "Show the schema for base ID 'app123XYZ'."

**🤖 AI Agent:**
> Accessing base architecture... Base app123XYZ contains 3 tables: 'Leads', 'Interactions', and 'Revenue'. I've retrieved the high-fidelity field definitions and view IDs to help with automated data entry. Need a summary of the field types?


## ❓ FAQ

**Q: How do I find my Airtable Personal Access Token?**
Log in to your account, navigate to the [**Developer Hub**](https://airtable.com/create/tokens), and click **Create token**. Ensure you grant `data.records:read`, `data.records:write`, and `schema.bases:read` scopes.

**Q: Can I filter records using formulas via AI?**
Yes! The `list_airtable_records` tool accepts a `filter_by_formula` parameter where you can provide native Airtable query logic programmatically.

**Q: How do I find my Base and Table IDs?**
Base IDs are found in the URL (starts with 'app'). You can use the `get_airtable_base_schema` tool to retrieve Table IDs and field names programmatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/airtable-alternative](https://vinkius.com/mcp/airtable-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Airtable** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `airtable-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Airtable** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "airtable-alternative": {
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

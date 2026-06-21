# Airtable MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/airtable)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Connect your Airtable bases to your AI agent — query records, edit spreadsheets, and build automated workflows naturally via chat.

## Description
Connect your **Airtable** account to your AI agent to transform static data into intelligent, conversational spreadsheet workflows.

### What you can do

- **Bases & Tables** — Browse your entire Airtable workspace, list all available bases, and retrieve the schema of any specific table.
- **Read & Query Records** — Fetch specific rows, run complex filters natively, and have the agent summarize data from hundreds of cells into concise insights.
- **Create & Update Data** — Ask the agent to bulk-add new leads, update project statuses, or fix formatting across multiple columns instantly.
- **Delete Records** — Safely remove outdated or duplicate entries through a secure, conversational command.

### How it works

1. Add this integration to your workspace.
2. Provide an Airtable Personal Access Token.
3. Chat with your bases using Claude, Cursor, or any compatible AI agent.

### Who is this for?

- **Project Managers** — ask the agent to identify all overdue tasks in a massive grid and automatically change their status to 'At Risk'.
- **Content Teams** — have the agent review your editorial calendar base and draft new social media copy directly into empty records.
- **Sales & Ops** — instantly query your CRM base for all leads generated last month and update their tracking stages in bulk.


## Available Tools (10)
- **list_bases**: List Airtable bases
- **list_tables**: List tables in a base
- **list_records**: List records from a table
- **get_record**: Get a single record
- **create_records**: Create records in bulk
- **update_records**: Update records in bulk
- **delete_records**: Delete records in bulk
- **search_records**: g. {Status}="Done").

Search records with formulas
- **list_fields**: Get table columns
- **get_base_metadata**: Get base schema


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Airtable** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all tables available inside my 'Product Roadmap' base."

**🤖 AI Agent:**
> In the base 'Product Roadmap', I found 4 tables:
1. Features (ID: tblXy01)
2. Epics (ID: tblXy02)
3. Team Members (ID: tblXy03)
4. Sprint Schedule (ID: tblXy04)
Would you like me to query recent records from any of them?

---

**👤 You:**
> "Find all records in the 'Leads' table where the 'Status' is 'In Progress'."

**🤖 AI Agent:**
> I've fetched 3 leads that match your criteria:
1. Acme Corp - Value: $10,000 - Last Contact: Yesterday
2. Hooli Tech - Value: $4,500 - Last Contact: 3 days ago
3. Initech - Value: $1,200 - Last Contact: Today
Should I compose a follow-up email draft for them?

---

**👤 You:**
> "Create a new record in the 'Tasks' table assigned to Mark with the title 'Review design assets' and mark it 'Urgent'."

**🤖 AI Agent:**
> Done. Created record `rec9A8B7` in the Tasks table. The title is 'Review design assets', Assignee is set to 'Mark', and Priority is mapped to the 'Urgent' single-select parameter successfully.


## ❓ FAQ

**Q: Can the agent query and filter records using Airtable native formulas?**
Yes! The AI agent understands Airtable's native `filterByFormula` parameter. You can ask it to "Find all records where Status is 'Done' and Priority is 'High'", and it will translate your request into the exact Airatble formula required to fetch only that data.

**Q: How do I ensure the agent adds data to the correct columns?**
Before writing, the agent will typically fetch the schema of the Table to understand the exact column spelling, ID, and data type (like Checkbox, Formula, or Single Select). You just need to say "Add a new row for John Doe with Status Lead", and it will align the values to the existing column structure.

**Q: If my base has tens of thousands of records, will it hallucinate?**
No. The integration paginates large queries to ensure accurate results. If you ask a broad open question on a 50,000-row base, the agent will gracefully fetch the data in chunks and summarize the response using the actual API output.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/airtable](https://vinkius.com/mcp/airtable)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `airtable` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Airtable** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "airtable": {
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

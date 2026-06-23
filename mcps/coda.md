# Coda MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coda)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Enable your AI agent to manage docs, tables, formulas, and rows via the Coda API.

## Description
Connect your AI to **Coda**, the collaborative document platform that brings together words, data, and teams.

### What you can do

- **Document Browsing** — List your recent docs and navigate their sections, tables, and pages.
- **Table Data** — Read rows from any Coda table, filter by column values, and update records.
- **Formula Values** — Retrieve the live value of any named formula in a doc for real-time reporting.

### How it works

1. Add the Coda integration to your AI toolset.
2. Provide your API Token (from Account Settings in Coda).
3. Manage your docs and data via natural language.

### Who is this for?

- **Product Managers** — Pull table data and formula results without opening the doc.
- **Operations Teams** — Update tracker tables and check statuses from chat.
- **Developers** — Automate data sync between Coda docs and other systems.


## Available Tools (10)
- **delete_rows**: Delete one or more rows from a Coda table
- **get_doc_details**: Retrieve detailed information about a specific Coda document
- **get_formula_value**: Retrieve the current calculated value of a named formula
- **insert_rows**: Insert new rows into a Coda table
- **list_columns**: Retrieve a list of columns in a Coda table
- **list_docs**: Retrieve a list of Coda documents available to you
- **list_formulas**: Retrieve a list of named formulas in a Coda document
- **list_rows**: Retrieve rows from a specific table in a Coda document
- **list_tables**: Retrieve a list of tables within a specific Coda document
- **update_row**: Update an existing row in a Coda table


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coda** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my recent documents in Coda."

**🤖 AI Agent:**
> You have 8 docs:
1. 'Project Tracker' — last edited 1h ago, 3 tables
2. 'Q1 OKRs' — last edited yesterday, 2 tables
3. 'Sprint Board' — last edited 3 days ago, 5 tables
Would you like to read data from any of these?

---

**👤 You:**
> "Get the current value of formula 'TotalBudget' in doc 'doc-yyyy'."

**🤖 AI Agent:**
> Formula 'TotalBudget' in doc 'doc-yyyy': **$142,500.00**. Last recalculated: 3 minutes ago.

---

**👤 You:**
> "Check the status of task 'Q3 Launch' in our Sprint Board table."

**🤖 AI Agent:**
> Scanning the 'Sprint Board' table. Task 'Q3 Launch' is currently marked as 'In Progress'. It is assigned to Sarah and has a targeted delivery of this coming Friday.


## ❓ FAQ

**Q: How do I find my doc and table IDs?**
You can find IDs in the document's URL, or use the 'list_docs' and 'list_tables' tools to discover them.

**Q: What does 'HTTP 202 Accepted' mean?**
Coda processes many changes asynchronously. This status means your request was queued and will be applied shortly.

**Q: Can I trigger buttons in Coda?**
Many Coda buttons are column actions that can be triggered by updating a row value. So yes, indirectly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coda](https://vinkius.com/mcp/coda)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coda** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coda` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coda** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coda": {
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

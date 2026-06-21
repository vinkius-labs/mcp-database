# Coda MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coda-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Combine docs, spreadsheets, and apps into powerful all-in-one documents that grow with your team and automate routine work.

## Description
Connect your **Coda** account to any AI agent and take full control of your collaborative workspace and structured data workflows through natural conversation.

### What you can do

- **Document Orchestration** — List and manage your Coda documents programmatically, retrieving detailed metadata and ownership information
- **Table & View Intelligence** — Access and monitor table structures (columns) and row data in real-time to maintain a high-fidelity database directly through your agent
- **Data Manipulation** — Programmatically insert, update, or delete rows in any table to coordinate your relational data and project trackers
- **Formula Automation** — Retrieve named formula values and workspace insights to leverage Coda's computational power within your AI workflows
- **Account Visibility** — Access your Coda profile and workspace metadata directly through your agent for instant operational reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** from Coda (Account Settings > API Settings)
3. Start managing your collaborative docs from Claude, Cursor, or any MCP client

No more manual toggling between browser tabs to check row statuses. Your AI acts as your dedicated document operations coordinator and data architect.

### Who is this for?

- **Project Managers** — instantly retrieve task lists and update row statuses using natural language commands
- **Operations Teams** — automate lead tracking and high-volume relational data management without leaving your workspace
- **Product Leads** — monitor project hub activity and retrieve formula-driven metrics through simple AI queries


## Available Tools (11)
- **delete_rows**: Remove rows from a table
- **get_doc_details**: Get metadata for a doc
- **get_table_details**: Get details for a table
- **insert_rows**: Add new rows to a table
- **list_columns**: List columns for a table
- **list_docs**: List your Coda documents
- **list_formulas**: List formulas in a document
- **list_rows**: Supports filtering.

List rows from a table
- **list_tables**: List tables in a document
- **update_row**: Update fields in a row
- **get_user_profile**: Get your Coda profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coda** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all tables in Coda document ID 'doc_123'."

**🤖 AI Agent:**
> I've retrieved the tables for your doc. You have 3 active tables: 'Task_List' (ID: grid-abc), 'Project_Timeline', and 'Team_Resources'. Which one should we inspect for rows?

---

**👤 You:**
> "Add a row to 'Tasks' with Title 'Design API' and Priority 'High'."

**🤖 AI Agent:**
> Action complete! I've inserted the new row into the 'Tasks' table. The record is now visible in your Coda doc with the specified title and priority metadata.

---

**👤 You:**
> "Retrieve the value of the named formula 'Total_Project_Budget'."

**🤖 AI Agent:**
> Fetching formula... The current value of 'Total_Project_Budget' in your document is $15,420.00. Shall I list all other named formulas in this workspace for you?


## ❓ FAQ

**Q: How do I find my Coda API Token?**
Log in to Coda, navigate to **Account Settings** > **API Settings**, and generate a new token for your integration.

**Q: Where do I find my Doc ID?**
The Doc ID is the string of characters in your Coda document's URL after the '/d/'.

**Q: Can I filter rows using natural language?**
Yes! The `list_rows` tool supports a `query` parameter where the agent can apply filters like `Status:"Done"` to find specific data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coda-alternative](https://vinkius.com/mcp/coda-alternative)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `coda-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coda** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coda-alternative": {
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

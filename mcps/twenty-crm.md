# Twenty CRM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/twenty-crm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Manage your CRM data directly from AI — list people, companies, and opportunities, and create or update records in Twenty CRM.

## Description
Connect your **Twenty CRM** account to any AI agent and take full control of your sales pipeline and contact database through natural conversation.

### What you can do

- **People Management** — List all contacts, fetch specific details, and create or update person records directly in the CRM.
- **Company Tracking** — Manage organizational accounts, list companies, and inspect company metadata using unique IDs.
- **Opportunity Pipeline** — Query all sales opportunities (deals), track progress, and create new entries to keep your pipeline updated.
- **Full Data Control** — Perform CRUD operations (Create, Read, Update, Delete) on people and companies to maintain data hygiene.
- **Seamless Integration** — Access your CRM data from Claude, Cursor, or any MCP-compatible client without leaving your workflow.

### How it works

1. Subscribe to this server
2. Enter your Twenty API Key and Base URL (e.g., https://api.twenty.com)
3. Start managing your CRM records using natural language

### Who is this for?

- **Sales Teams** — quickly update opportunity statuses and add new leads without switching tabs
- **Account Managers** — retrieve company details and contact information instantly during client calls
- **Developers** — manage CRM data directly from the code editor to test integrations or verify record states


## Available Tools (25)
- **update_person**: Update an existing person
- **update_task**: Update an existing task
- **get_company**: Get a specific company by ID
- **get_note**: Get a specific note by ID
- **get_opportunity**: Get a specific opportunity by ID
- **get_person**: Get a specific person by ID
- **get_task**: Get a specific task by ID
- **list_companies**: List companies in Twenty CRM
- **list_notes**: List notes in Twenty CRM
- **list_opportunities**: List opportunities in Twenty CRM
- **list_people**: List people in Twenty CRM
- **list_tasks**: List tasks in Twenty CRM
- **update_company**: Update an existing company
- **update_note**: Update an existing note
- **update_opportunity**: Update an existing opportunity
- **create_opportunity**: Create a new opportunity
- **create_person**: Create a new person
- **create_task**: Create a new task
- **delete_company**: Delete a company
- **delete_note**: Delete a note
- **delete_opportunity**: Delete an opportunity
- **delete_person**: Delete a person
- **delete_task**: Delete a task
- **create_company**: Create a new company
- **create_note**: Create a new note


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Twenty CRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all people in my Twenty CRM."

**🤖 AI Agent:**
> I've retrieved the list of people. You have 15 contacts, including 'John Doe' (ID: 1) and 'Jane Smith' (ID: 2). Would you like to see details for a specific person?

---

**👤 You:**
> "Create a new company named 'Global Tech Solutions'."

**🤖 AI Agent:**
> Success! I've created 'Global Tech Solutions' in your CRM with ID 582. You can now associate people or opportunities with this company.

---

**👤 You:**
> "Get the details for opportunity ID 101."

**🤖 AI Agent:**
> I found opportunity 101: 'Enterprise License Expansion'. It is currently in the 'Negotiation' stage with an estimated value of $50,000.


## ❓ FAQ

**Q: Can I create a new contact person directly through the AI?**
Yes! Use the `create_person` tool by providing at least a first name. You can also include a last name to create a complete record in your Twenty CRM database.

**Q: How do I see all the companies currently registered in my CRM?**
Simply ask the agent to run the `list_companies` tool. It will retrieve a list of all company records (accounts) stored in your Twenty environment.

**Q: Is it possible to update the details of an existing sales opportunity?**
Yes, you can use the `update_opportunity` tool. You will need the specific Opportunity ID and the new fields (like name) you wish to modify.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/twenty-crm](https://vinkius.com/mcp/twenty-crm)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Twenty CRM** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `twenty-crm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Twenty CRM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "twenty-crm": {
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

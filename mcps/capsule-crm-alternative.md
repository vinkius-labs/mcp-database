# Capsule CRM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/capsule-crm-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Manage contacts, sales opportunities, and projects via Capsule CRM — search parties, track pipelines, and manage tasks directly from any AI agent.

## Description
Connect your **Capsule CRM** account to any AI agent to streamline your sales and relationship management workflows through natural conversation.

### What you can do

- **Contact Management** — List, search, and retrieve detailed profiles for people and organizations (Parties) using `search_parties` and `get_party`.
- **Sales Pipeline** — Track opportunities, update milestones, and manage your sales funnel with `list_opportunities` and `update_opportunity`.
- **Project Tracking** — Oversee projects from inception to completion with `list_projects` and `get_project`.
- **Task & Activity Logging** — Create and manage tasks, and view history entries with `list_tasks` and `list_entity_entries` to keep track of every interaction.
- **Customization** — Access tags and custom fields via `list_tags` and `list_custom_fields` to maintain your specific business data structure.

### How it works

1. Subscribe to this server
2. Enter your Capsule CRM Personal Access Token
3. Start managing your CRM data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — quickly update opportunity status and add notes after calls without leaving the chat interface.
- **Account Managers** — retrieve full contact history and background info before meetings.
- **Project Leads** — monitor project progress and task completion across the organization.


## Available Tools (31)
- **create_entry**: Create a new note entry
- **create_opportunity**: Create a new opportunity
- **create_party**: Create a new party (person or organisation)
- **create_project**: Create a new project (kase)
- **create_task**: Create a new task
- **delete_party**: Delete a party
- **delete_project**: Delete a project (kase)
- **delete_task**: Delete a task
- **get_current_user**: Show the authenticated user
- **get_opportunity**: Get details for a specific opportunity
- **get_party**: Get details for a specific party
- **get_project**: Get details for a specific project (kase)
- **get_task**: Get details for a specific task
- **list_custom_fields**: List custom field definitions for parties, opportunities, or kases
- **list_deleted_parties**: List deleted parties since a specific date
- **list_entity_entries**: List entries for a specific party, project, or opportunity
- **list_entries**: List recent entries (notes & emails)
- **list_opportunities**: List all opportunities
- **list_parties**: List all parties (people and organisations)
- **list_projects**: List all projects (kases)
- **list_tags**: List tag definitions for parties, opportunities, or kases
- **list_tasks**: List tasks (default: open)
- **list_teams**: List all teams
- **list_users**: List all users
- **search_opportunities**: Search for opportunities
- **search_parties**: Search for parties
- **update_opportunity**: Update an existing opportunity
- **update_party**: Update an existing party
- **update_project**: Update an existing project (kase)
- **update_task**: Update an existing task
- **delete_opportunity**: Delete an opportunity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Capsule CRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for a contact named 'Alice Smith' in Capsule."

**🤖 AI Agent:**
> I found a contact: Alice Smith (ID: 54321) at 'Tech Solutions'. Would you like me to fetch her full profile or recent interaction history?

---

**👤 You:**
> "List all my open sales opportunities."

**🤖 AI Agent:**
> You have 3 open opportunities: 'Enterprise License' ($5,000), 'Consulting Services' ($2,500), and 'API Integration' ($1,200). Which one would you like to update?

---

**👤 You:**
> "Show me the tasks for project ID 12345."

**🤖 AI Agent:**
> I've retrieved the tasks for project 12345. There are 2 pending tasks: 'Review contract' (Due tomorrow) and 'Send welcome email' (Overdue).


## ❓ FAQ

**Q: How can I find a specific contact or company in my CRM?**
You can use the `search_parties` tool by providing a search query. The AI will return matching people and organizations, including their IDs for further inspection via `get_party`.

**Q: Can I see the history of interactions for a specific person?**
Yes! Use the `list_entity_entries` tool with the Party ID. This will retrieve all history entries, notes, and activities associated with that specific contact.

**Q: Is it possible to manage my sales opportunities and pipeline?**
Absolutely. You can use `list_opportunities` to see your current deals, `get_opportunity` for details, and `update_opportunity` to change milestones or probabilities as deals progress.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/capsule-crm-alternative](https://vinkius.com/mcp/capsule-crm-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Capsule CRM** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `capsule-crm-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Capsule CRM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "capsule-crm-alternative": {
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

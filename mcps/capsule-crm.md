# Capsule CRM MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/capsule-crm)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your CRM via Capsule — track contacts, opportunities, and tasks directly from any AI agent.

## Description
Connect your **Capsule CRM** account to any AI agent and orchestrate your sales pipelines, contact management, and task automation through natural conversation.

### What you can do

- **Contact Oversight** — List all your parties (people and organizations) and retrieve detailed profiles, including emails and tags.
- **Opportunity Coordination** — List all sales opportunities and retrieve detailed metadata, including milestones and values.
- **Task Management** — Create, update, and monitor tasks and reminders to ensure your sales process stays on track.
- **Project Tracking** — Access and list your projects managed within the platform to maintain visibility across your team.
- **CRM Automation** — Create new person profiles and tasks directly from your workspace using natural language.
- **Deep Dives** — Get detailed data for specific party, opportunity, or task IDs straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Capsule CRM Personal Access Token (Bearer)
3. Start managing your sales pipeline from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales & SDR Teams** — quickly check for upcoming tasks or retrieve contact details without manual CRM logins.
- **Account Managers** — monitor opportunity statuses and project progress straight from their workflow tools.
- **Business Admins** — retrieve daily CRM summaries and account info using natural language.


## Available Tools (11)
- **create_person**: Add a new person to Capsule CRM
- **create_task**: Create a new task
- **get_account_info**: Retrieve core account/user information
- **get_opportunity_details**: Get details of a specific opportunity
- **get_contact_details**: Get details of a specific contact or organization
- **get_project_details**: Get details of a specific project
- **get_task_details**: Get details of a specific task
- **list_opportunities**: List all sales opportunities
- **list_contacts**: List all contacts and organizations (parties)
- **list_projects**: List all projects
- **list_tasks**: List all tasks and reminders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Capsule CRM** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 contacts in Capsule CRM."

**🤖 AI Agent:**
> I've retrieved your contacts. You have 5 recent parties, including 'John Doe' (Person) and 'Vinkius North' (Organization). Would you like full details for any of them?

---

**👤 You:**
> "Show my open sales opportunities."

**🤖 AI Agent:**
> Retrieving opportunities... You have 3 open deals: 'New Software License' (Value: $5,000) and 'Cloud Migration Services' (Value: $12,000). Which one would you like to inspect?

---

**👤 You:**
> "Create a task 'Follow up with John Doe' due tomorrow."

**🤖 AI Agent:**
> Task 'Follow up with John Doe' has been successfully created in your Capsule account with a due date of tomorrow.


## ❓ FAQ

**Q: Can I check the value of a sales opportunity using the agent?**
Yes! Use the `get_opportunity_details` tool with the Opportunity ID. Your agent will fetch the detailed metadata, which includes the value amount and currency from Capsule CRM.

**Q: How do I list all the people in my CRM?**
Simply ask the agent to `list_contacts`. It will retrieve the list of all parties (people and organizations) from your Capsule account, including their names and primary details.

**Q: Does the integration allow creating a new task?**
Yes. Use the `create_task` action and provide the description. You can also optionally specify a due date. The task will be added to your Capsule account instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/capsule-crm](https://vinkius.com/mcp/capsule-crm)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `capsule-crm` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Capsule CRM** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "capsule-crm": {
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

# Karbon MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/karbon)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Manage your accounting firm's workflow, contacts, and work items directly via AI agents.

## Description
Connect your **Karbon** account to any AI agent to streamline your accounting firm's operations. This MCP server allows your agent to interact with Karbon's powerful workflow and practice management features.

### What you can do

- **Contact Management** — List, retrieve, and create contacts (both People and Organizations) to maintain a clean CRM
- **Workflow Automation** — List and create work items, projects, and tasks to keep track of every engagement
- **Staff Visibility** — Query users and firm members to identify assignees and team availability
- **Note Inspection** — Access historical notes and comments recorded against any contact profile
- **Work Progress** — Get detailed status updates and metadata for specific work items and associated tasks

### How it works

1. Subscribe to this server
2. Enter your Karbon Access Key and Bearer Token
3. Start managing your firm's practice from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Accounting Firm Owners** — Get instant visibility into work progress and team performance
- **Project Managers** — Automate the creation of work items and tracking of task completion
- **Client Managers** — Quickly retrieve contact details and historical notes before meetings


## Available Tools (12)
- **list_contacts**: Useful for a broad overview of clients and associates.

List all contacts (Organizations and People)
- **create_contact**: Requires a name and contact type (Person or Organization).

Create a new contact in Karbon
- **create_work_item**: Requires a title and a work type.

Create a new work item (project)
- **get_contact**: Get detailed information for a specific contact
- **get_work_item**: Get details for a specific work item
- **list_contact_notes**: List notes for a specific contact
- **list_organizations**: ).

List only organizational contacts
- **list_people**: ).

List only individual people contacts
- **list_work_tasks**: List tasks for a specific work item
- **update_work_item**: Update an existing work item
- **list_users**: Use this to identify assignees or firm members.

List all users in the Karbon firm
- **list_work_items**: Use this to track firm workflows and engagements.

List all work items (workflows)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Karbon** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my organizational contacts in Karbon."

**🤖 AI Agent:**
> I've retrieved 12 organizational contacts from your Karbon account, including 'Acme Corp', 'Global Logistics', and 'Innovate Tech'. Would you like to see more details for any of them?

---

**👤 You:**
> "Show me the tasks for the work item with key 'WORK_123'."

**🤖 AI Agent:**
> I found 8 tasks for work item 'WORK_123'. Current pending items include 'Review Tax Documents' and 'Client Interview'. 5 tasks are already completed.

---

**👤 You:**
> "Create a new organization contact named 'Tech Pioneers'."

**🤖 AI Agent:**
> Successfully created the organization 'Tech Pioneers' in your Karbon contacts. The unique key assigned is 'CONTACT_987'.


## ❓ FAQ

**Q: Can the agent create new work items using templates?**
Yes, the `create_work_item` tool allows specifying a work type, which corresponds to your templates in Karbon. This helps in quickly starting new client engagements.

**Q: Can I filter contacts to see only organizations?**
Absolutely. Use the `list_organizations` tool to retrieve only organizational entities, or `list_people` to see individual contacts.

**Q: Is it possible to view the tasks inside a specific project?**
Yes! Use the `list_work_tasks` tool with the unique work item key to see all associated checklist items and tasks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/karbon](https://vinkius.com/mcp/karbon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Karbon** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `karbon` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Karbon** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "karbon": {
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

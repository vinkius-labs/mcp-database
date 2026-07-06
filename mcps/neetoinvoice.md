# NeetoInvoice MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/neetoinvoice)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [project-management](../categories/project-management.md)

Automate billing and project management via NeetoInvoice — manage clients, track time, and generate invoices directly from any AI agent.

## Description
Connect your **NeetoInvoice** account to any AI agent to streamline your billing and project management workflows through natural conversation.

### What you can do

- **Client Management** — Create, retrieve, and update client profiles and recipients with ease using `create_client` and `get_client`.
- **Project & Team Tracking** — Set up projects with specific billing methods (hourly or fixed) and manage team assignments using `create_project` and `add_project_user`.
- **Time Tracking** — Log time entries and monitor work logs across projects to ensure accurate billing with `create_time_entry`.
- **Invoice Generation** — Automatically generate professional invoices based on project data and time entries using `generate_invoice`.
- **Team Collaboration** — List and manage team members and project users to keep your workforce organized.

### How it works

1. Subscribe to this server
2. Enter your NeetoInvoice API Key and Subdomain
3. Start managing your clients and invoices from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Freelancers & Agencies** — track billable hours and generate invoices without leaving your workspace
- **Finance Teams** — quickly query client details and project statuses for reporting
- **Project Managers** — manage team assignments and project billing methods through simple chat commands


## Available Tools (20)
- **create_client**: Requires name, currency, and status.

Create a new client in NeetoInvoice
- **create_project**: Create a new project
- **create_recipient**: Create a recipient for a client
- **create_time_entry**: Create a new time entry
- **delete_recipient**: Delete a client recipient
- **generate_invoice**: Generate a new invoice for a client
- **get_client**: Get client details by ID
- **get_project**: Get project details by ID
- **list_project_users**: List users assigned to a project
- **list_team_members**: List all team members in the workspace
- **list_time_entries**: List time entries with optional filters
- **remove_project_user**: Remove a user from a project
- **remove_team_members**: Remove team members from the workspace
- **update_client**: Update an existing client
- **update_project**: Update an existing project
- **update_project_user**: Update a project user role
- **update_recipient**: Update a client recipient
- **update_team_member**: Update a team member
- **add_project_user**: Add a user to a project
- **add_team_members**: Add team members to the workspace


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NeetoInvoice** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a new client named 'Acme Corp' with USD currency and active status."

**🤖 AI Agent:**
> I've created the client 'Acme Corp' (ID: client_123) with USD currency. They are currently set as active.

---

**👤 You:**
> "List all users assigned to project 98765."

**🤖 AI Agent:**
> Fetching users for project 98765... I found 3 users: John Doe (Manager), Jane Smith (Regular), and Bob Wilson (Regular).

---

**👤 You:**
> "Generate an invoice for project ID 555."

**🤖 AI Agent:**
> Processing... I have successfully generated the invoice for project 555. You can now review it in your NeetoInvoice dashboard.


## ❓ FAQ

**Q: How do I log hours for a specific project?**
You can use the `create_time_entry` tool. Just provide the project ID and the duration of work to record it in NeetoInvoice immediately.

**Q: Can I add a new team member to a project via AI?**
Yes! Use the `add_project_user` tool by specifying the Project ID, User ID, and their role (e.g., 'project_manager' or 'regular_user').

**Q: How can I check the billing details of a project?**
Use the `get_project` tool with the Project ID. It will return the billing method, tasks, and other metadata associated with that project.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/neetoinvoice](https://vinkius.com/mcp/neetoinvoice)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NeetoInvoice** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `neetoinvoice` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NeetoInvoice** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "neetoinvoice": {
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

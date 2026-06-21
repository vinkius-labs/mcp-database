# Moxie MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/moxie)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your freelance or agency business with client portals, project tracking, time logging, and invoicing in one clean tool.

## Description
Connect your **Moxie** workspace to any AI agent and manage your freelance or agency business through natural conversation.

### What you can do

- **Clients & Contacts** — List clients, create new ones, search contacts
- **Projects & Tasks** — Search/create projects, create tasks
- **Invoices** — Search payable invoices, create new ones
- **Time & Expenses** — Log time entries, record expenses
- **Tickets** — Create support tickets
- **Users** — List workspace team members

### Who is this for?

- **Freelancers** — track time and invoice clients
- **Agencies** — manage projects and team workloads


## Available Tools
- **create_client**: Create a new client
- **create_expense**: Log an expense
- **create_invoice**: Create a new invoice
- **create_project**: Create a new project
- **create_task**: Create a new task
- **create_ticket**: Create a support ticket
- **create_time_entry**: Log time
- **list_clients**: List all clients in Moxie
- **list_users**: List workspace users
- **search_contacts**: Search for contacts
- **search_invoices**: Search for payable invoices
- **search_projects**: Search for projects


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Moxie** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all clients and their projects."

**🤖 AI Agent:**
> Clients: 4. 1) Acme Corp (3 projects). 2) Beta Design (1). 3) Gamma Studios (2). 4) Delta Marketing (0). Total: 6 active projects.

---

**👤 You:**
> "Log 2 hours of consulting on the Acme Corp project."

**🤖 AI Agent:**
> Time logged ✅. 120 min, Project: Acme Corp Website. Billable.

---

**👤 You:**
> "Create an invoice for Beta Design."

**🤖 AI Agent:**
> Invoice created ✅. Client: Beta Design. ID: INV-078. Status: Draft.


## ❓ FAQ

**Q: Can I track time and create invoices?**
Yes. Log time entries with descriptions and durations, then create invoices linked to specific clients.

**Q: How does Moxie authentication work?**
Moxie uses an **X-API-KEY** header with your API key, plus your workspace **Base URL**.

**Q: Can I manage projects and tasks?**
Yes. Search projects, create new ones with client associations, and add tasks within projects.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/moxie](https://vinkius.com/mcp/moxie)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Moxie** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `moxie` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Moxie** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "moxie": {
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

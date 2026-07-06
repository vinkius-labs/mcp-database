# GitScrum ClientFlow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gitscrum-clientflow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [project-management](../categories/project-management.md)

Streamline client operations via GitScrum ClientFlow — manage clients, create invoices, draft proposals, and monitor project budgets directly from any AI agent.

## Description
### What you can do

- **Client management** — list, inspect, and create client records with contact details and project history
- **Invoice generation** — create and review invoices linked to client accounts with line items and totals
- **Proposal drafting** — browse existing proposals and their approval statuses for any client
- **Budget monitoring** — check project budget consumption and remaining allocations in real-time
- **Dashboard insights** — access the ClientFlow dashboard for a consolidated view of revenue and client activity
- **Time billing** — list and log time entries on tasks for accurate client billing

### How it works

1. Subscribe to the GitScrum ClientFlow integration from the marketplace
2. Enter your GitScrum API token and company slug
3. Ask your agent to review client portfolios, draft invoices, or check budget health — works in Claude, Cursor, and any MCP client

Your agent becomes your client operations assistant, eliminating context-switching between billing and project tools.

### Who is this for?

- **Agency owners** — monitor all client budgets and revenue from a single conversational interface
- **Project managers** — track billable hours and generate invoices without leaving the workflow
- **Finance teams** — review proposals, invoices, and budget consumption in natural language


## Available Tools (12)
- **clientflow_dashboard**: Get ClientFlow dashboard overview
- **create_invoice**: Pass additional fields as JSON in the body parameter.

Create an invoice for a client
- **get_invoice**: Get invoice details
- **list_invoices**: List all invoices
- **get_proposal**: Get proposal details
- **list_proposals**: List all proposals
- **log_time**: Log time on a task
- **list_time_entries**: List time tracking entries
- **project_budget**: Get project budget
- **create_client**: Create a new client
- **get_client**: Get client details
- **list_clients**: List all clients


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GitScrum ClientFlow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our clients on GitScrum."

**🤖 AI Agent:**
> You have 6 active clients: 1) 'TechCorp Inc.' (3 active projects, $24,500 invoiced), 2) 'Design Studio LLC' (1 project, $8,200 invoiced), 3) 'StartupXYZ' (2 projects, $15,300 invoiced)... Would you like to see invoices for any specific client?

---

**👤 You:**
> "Show me the ClientFlow dashboard overview."

**🤖 AI Agent:**
> ClientFlow Dashboard: Total revenue this month: $47,800 (+12% vs last month). 4 pending invoices worth $12,400. 2 proposals awaiting approval ($18,000 combined). 3 projects at >80% budget consumption. Shall I drill into any of these areas?

---

**👤 You:**
> "Create a new client 'Acme Corp' with email billing@acme.com."

**🤖 AI Agent:**
> Client 'Acme Corp' created successfully with billing contact billing@acme.com. The client UUID is c8d9e0f1-2345-6789-abcd-ef0123456789. Ready to create a proposal or invoice for this client?


## ❓ FAQ

**Q: Can the agent create an invoice for a specific client?**
Yes! Use `create_invoice` with the client UUID and line item details. The agent creates the invoice linked to the client account, including amounts, descriptions, and due dates. Use `list_clients` first to find the correct client UUID.

**Q: Can I monitor project budget health conversationally?**
Absolutely. Use `project_budget` to get real-time budget consumption data, including remaining allocation and burn rate. Combine with `clientflow_dashboard` for the full revenue picture across all clients and projects.

**Q: What billing data can the agent access?**
The agent can list and create clients, manage invoices (list and create), browse proposals, track time entries on tasks, and access the consolidated ClientFlow dashboard. All operations respect your GitScrum account permissions and organizational role.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gitscrum-clientflow](https://vinkius.com/mcp/gitscrum-clientflow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GitScrum ClientFlow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gitscrum-clientflow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GitScrum ClientFlow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gitscrum-clientflow": {
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

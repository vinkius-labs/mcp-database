# TaskForce MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/taskforce)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Manage leads, customers, cases, and invoices programmatically using AI.

## Description
Connect your AI agent to **TaskForce** to natively manage your CRM workflow, customer interactions, and invoicing through natural language commands.

### What you can do

- **Lead & Customer Management** — Query lists of active leads, fetch detailed customer profiles, and instantly create new lead records on the fly.
- **Case Tracking** — Read and track support or business cases, and generate new cases directly from your chat interface.
- **Financial Overview** — Pull real-time lists of pending invoices and active quotes to monitor business performance without opening a dashboard.

### How it works

1. Retrieve your API Key from the TaskForce Admin dashboard.
2. Provide the key to this integration.
3. Instruct your agent to pull your recent leads or check the status of an invoice.

### Who is this for?

- **Sales & Support Teams** — Update leads and track customer cases seamlessly.
- **Accountants** — Monitor invoices and quotes dynamically.
- **Developers** — Connect your TaskForce database with external custom tools.


## Available Tools
- **create_taskforce_case**: Create a new case
- **create_taskforce_lead**: Create a new lead
- **get_taskforce_customer**: Get customer details
- **get_taskforce_lead**: Get lead details
- **list_taskforce_cases**: List all cases
- **list_taskforce_customers**: List all customers
- **list_taskforce_invoices**: List all invoices
- **list_taskforce_leads**: List all leads
- **list_taskforce_quotes**: List all quotes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TaskForce** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active leads in my TaskForce account."

**🤖 AI Agent:**
> Here is the information you requested based on the execution of the tools.

---

**👤 You:**
> "Create a new lead for John Doe (john@example.com)."

**🤖 AI Agent:**
> Here is the information you requested based on the execution of the tools.

---

**👤 You:**
> "Fetch the latest invoices and quotes."

**🤖 AI Agent:**
> Here is the information you requested based on the execution of the tools.


## ❓ FAQ

**Q: Can I add a new lead directly from the chat?**
Yes. By invoking the 'create_taskforce_lead' tool and providing the lead's information in JSON format, the AI will register it instantly.

**Q: How do I check my pending invoices?**
You can use the 'list_taskforce_invoices' tool. The agent will fetch all your invoices and present their statuses.

**Q: Is it possible to view the details of a specific customer case?**
Yes, using the 'list_taskforce_cases' tool you can query all active support or business cases assigned in your CRM.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/taskforce](https://vinkius.com/mcp/taskforce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TaskForce** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `taskforce` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TaskForce** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "taskforce": {
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

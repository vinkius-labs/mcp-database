# Harvest MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/harvest)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate time tracking and invoicing via Harvest — manage clients, invoices, and time entries directly from any AI agent.

## Description
Connect your **Harvest** account to any AI agent and take full control of your time tracking, client management, and invoicing through natural conversation.

### What you can do

- **Time Tracking Oversight** — List and inspect tracked time entries to monitor team productivity.
- **Client Management** — List all clients, create new ones, and update company details effortlessly.
- **Invoicing Automation** — Access your invoice history, create new drafts, and manage billing statuses.
- **Project Monitoring** — List all active projects and retrieve detailed information for each.
- **User Profile** — Get information about the current authenticated user and account status.
- **Operational Efficiency** — Use AI to identify unbilled time or upcoming invoice deadlines across your organization.

### How it works

1. Subscribe to this server
2. Enter your Harvest Access Token and Account ID
3. Start managing your time and billing from Claude, Cursor, or any MCP-compatible client

No more manual exporting of time reports. Your AI assistant acts as a dedicated Billing Coordinator or Operations Manager.

### Who is this for?

- **Project Managers** — instantly retrieve project time summaries and client details during status calls.
- **Operations Leaders** — automate the oversight of invoicing and time entry compliance.
- **Freelancers & Small Agencies** — manage your entire billing cycle and time tracking without leaving your communication flow.


## Available Tools
- **delete_client**: Permanently delete a client
- **create_client**: Create a new client in Harvest
- **create_invoice**: Create a new invoice for a client
- **get_client**: Get detailed information for a specific client
- **get_invoice**: Get details for a specific invoice
- **get_my_profile**: Get information about the current authenticated user
- **list_clients**: List all clients in your Harvest account
- **list_invoices**: List all invoices, including drafts and sent ones
- **list_projects**: List all projects in the account
- **list_time_entries**: List tracked time entries
- **update_client**: Update an existing client name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Harvest** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all time entries from last week."

**🤖 AI Agent:**
> I've retrieved your time entries. Last week, your team logged a total of 120 hours across 5 projects. The most active project was 'Cloud Migration' with 45 hours. Would you like a detailed breakdown by user?

---

**👤 You:**
> "Create a new client named 'Acme Corp'."

**🤖 AI Agent:**
> Client created! I've successfully added 'Acme Corp' (ID: 8821) to your Harvest account. Should I associate a new project with this client now?

---

**👤 You:**
> "Show me all active projects."

**🤖 AI Agent:**
> Accessing projects... You have 4 active projects: 'Website Redesign', 'Mobile App Support', 'Internal Ops', and 'Q2 Marketing'. Which one would you like to see time summaries for?


## ❓ FAQ

**Q: How do I find my Harvest Access Token and Account ID?**
Go to the **Harvest Developers** site (id.getharvest.com), navigate to **Personal Access Tokens**, and create a new token. You will find both the **token** and the **Account ID** listed there.

**Q: Can I see time entries for a specific period?**
Yes! Use the `list_time_entries` tool and provide the `from` and `to` dates in YYYY-MM-DD format to retrieve records for that timeframe.

**Q: Is it possible to create invoices through this integration?**
Yes, you can use the `create_invoice` tool by providing a `client_id` and an optional `subject` to generate a new invoice draft in your Harvest account.

**Q: Is the integration secure for managing financial data?**
Absolutely. The integration uses official Harvest API tokens over HTTPS. Your credentials are encrypted and stored securely within the Vinkius Cloud infrastructure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/harvest](https://vinkius.com/mcp/harvest)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Harvest** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `harvest` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Harvest** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "harvest": {
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

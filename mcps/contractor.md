# Contractor+ MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/contractor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Run your contracting business with job estimates, invoicing, client management, and field crew tracking in one mobile platform.

## Description
Connect your **Contractor+** account to any AI agent and take full control of your field service management and business operations through natural conversation.

### What you can do

- **Client & Lead Orchestration** — List and manage your entire CRM programmatically, including creating new leads and retrieving detailed historical profiles
- **Estimate & Invoice Architecture** — Programmatically generate professional quotes and invoices, monitoring payment statuses and project totals in real-time
- **Field Operations Intelligence** — Access active jobs and scheduled work orders for your crews to maintain high-fidelity coordination between office and field
- **Property Management** — Access detailed records of service properties and tenant data to ensure perfectly coordinated site visits
- **Operational Monitoring** — Check API health status, monitor active webhooks, and retrieve account-level metadata directly through your agent for instant reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Contractor+ dashboard (Settings > API)
3. Start managing your field service operations from Claude, Cursor, or any MCP client

No more manual status checking or digging through fragmented job logs. Your AI acts as your dedicated field operations strategist and business coordinator.

### Who is this for?

- **Contractors & Service Providers** — instantly retrieve project estimates and update job statuses using natural language commands
- **Operations Leads** — track crew assignments and dispatch work orders without leaving your communication tools
- **Business Owners** — monitor invoice pipelines and manage client relationships through simple AI queries


## Available Tools (12)
- **create_client**: Create a new client or lead
- **create_estimate**: Create a new estimate
- **get_account_info**: Get account settings
- **get_client**: Get client details
- **list_clients**: List all clients and leads
- **list_estimates**: List project estimates
- **list_invoices**: List billing invoices
- **list_jobs**: List active jobs
- **list_properties**: List service properties
- **list_service_requests**: List incoming requests
- **list_webhooks**: List configured webhooks
- **list_work_orders**: List work orders


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Contractor+** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active jobs and their current statuses in Contractor+."

**🤖 AI Agent:**
> I've retrieved your ongoing jobs. You have 3 active projects: 'Roof Replacement' (In Progress), 'HVAC Repair' (Scheduled), and 'Kitchen Remodel'. Would you like the crew assignments for any of these?

---

**👤 You:**
> "Create a new lead for 'John Doe' at 'john@example.com'."

**🤖 AI Agent:**
> Lead created! John Doe has been successfully added to your Contractor+ CRM with ID 'cl_1024'. I've initialized his profile. Shall I create an initial estimate for a site visit?

---

**👤 You:**
> "Show me the last 5 invoices and their payment status."

**🤖 AI Agent:**
> Fetching invoices... Out of the last 5, three are 'Paid' and two are 'Overdue' (Invoice #402 and #405). Total outstanding balance is $2,450.00. Would you like me to send reminders for the overdue bills?


## ❓ FAQ

**Q: How do I find my Contractor+ API Key?**
Log in to your account, navigate to **Settings** > **API**, and copy your unique access token.

**Q: Does it support real-time work order tracking?**
Yes! The `list_work_orders` tool retrieves the most current assignments for your field crews directly from the platform.

**Q: Can I create new project estimates via AI?**
Absolutely. Use the `create_estimate` tool to specify a client ID, title, and total amount to generate a quote immediately.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/contractor](https://vinkius.com/mcp/contractor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Contractor+** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `contractor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Contractor+** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "contractor": {
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

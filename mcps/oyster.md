# Oyster MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/oyster)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [human-resources](../categories/human-resources.md)

Manage global HR, payroll, and compliance via Oyster — list engagements, track expenses, and manage time-off requests directly from any AI agent.

## Description
Connect your **Oyster** account to any AI agent to streamline your global team management and HR operations through natural conversation.

### What you can do

- **Engagement Management** — List all active engagements and fetch detailed metadata for specific team members globally.
- **Expense Tracking** — Query existing expenses, filter by review states, and create new expense requests with receipt metadata.
- **Time Off Requests** — Monitor, retrieve, and create time-off requests (vacation, sick leave) for your entire distributed workforce.
- **Financial Insights** — Access and filter company invoices by payroll periods, statuses, or specific engagement IDs.
- **Global Expansion** — Retrieve lists of supported hiring countries and subdivisions to plan your next global hire.
- **Operation Monitoring** — Track the status of asynchronous operations and manage webhooks for real-time updates.

### How it works

1. Subscribe to this server
2. Enter your Oyster Personal Access Token
3. Start managing your global workforce from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **HR Managers** — quickly check time-off balances and engagement details without navigating the Oyster dashboard.
- **Finance Teams** — audit expenses and invoices directly through conversational queries.
- **Operations Leads** — streamline the hiring process by checking country availability and creating draft employments.


## Available Tools
- **create_draft_employment**: This is an async operation.

Create a draft employment (Beta, Async)
- **create_expense**: This is an async operation, returns an operationKey.

Create a new expense (Async)
- **create_time_off_request**: Create a new time off request
- **create_webhook**: Create a new webhook endpoint
- **get_company**: Get company details
- **get_engagement**: Get details for a specific engagement
- **get_expense**: Get details for a specific expense
- **get_operation_status**: Get async operation status
- **get_time_off_request**: Get details for a specific time off request
- **list_engagements**: List Oyster engagements
- **list_expenses**: List expenses
- **list_hiring_countries**: List hiring countries (Beta)
- **list_invoices**: List invoices
- **list_subdivisions**: List subdivisions for a country (Beta)
- **list_time_off_requests**: List time off requests


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Oyster** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active engagements in my Oyster account."

**🤖 AI Agent:**
> I've retrieved your engagements. You have 12 active team members across 5 countries. Would you like to see the details for a specific engagement ID?

---

**👤 You:**
> "Show me the details for time off request ID 'tor_98765'."

**🤖 AI Agent:**
> Fetching request details... Request 'tor_98765' is for a 'VACATION' from 2023-12-20 to 2024-01-05. The current status is 'APPROVED'.

---

**👤 You:**
> "Create a sick leave request for engagement 'eng_123' for tomorrow."

**🤖 AI Agent:**
> I've initiated the sick leave request for engagement 'eng_123' for 2023-10-27. The request has been submitted successfully.


## ❓ FAQ

**Q: Can I submit a new expense for a team member through the AI?**
Yes! Use the `create_expense` tool. You will need to provide the engagement ID, expense details (name, description, category, date), and the receipt information including the amount and currency.

**Q: How do I check which countries Oyster supports for hiring?**
Simply ask the agent to run the `list_hiring_countries` tool. It will return a list of all countries where Oyster currently facilitates global employment.

**Q: Is it possible to track the status of a request I just created?**
Yes. For asynchronous operations like creating expenses, you can use the `get_operation_status` tool with the operation key provided during creation to check its progress.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oyster](https://vinkius.com/mcp/oyster)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Oyster** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `oyster` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Oyster** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "oyster": {
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

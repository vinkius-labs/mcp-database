# Cashboard MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cashboard)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage time tracking, invoicing, and projects via Cashboard — track expenses, send estimates, and monitor client billing directly from any AI agent.

## Description
Connect your **Cashboard** account to any AI agent and take full control of your freelance or small business operations through natural conversation. Streamline time tracking and client invoicing.

### What you can do

- **Invoicing Oversight** — List and retrieve details for all client invoices and estimates natively
- **Time Tracking** — Access recent time tracking entries to monitor project progress and billable hours
- **Expense Management** — List business expenses and associate them with specific projects securely
- **Project Control** — Monitor active projects and tasks to ensure delivery timelines are met flawlessly
- **Contact Management** — List client and staff contacts to maintain seamless communication
- **Account Visibility** — Retrieve core account and subscription information directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Cashboard API Key and account Subdomain
3. Start managing your business finances from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Freelancers** — track billable hours and send invoices using natural language
- **Small Business Owners** — monitor expenses and project profitability without opening the dashboard
- **Project Managers** — audit project tasks and time entries straight from their chat interface
- **Accountants** — quickly verify invoice statuses and client billing records


## Available Tools (8)
- **get_cashboard_account**: Retrieve core account and subscription information
- **list_cashboard_contacts**: List client and staff contacts
- **list_estimates**: List all project estimates
- **list_business_expenses**: List tracked business expenses
- **list_invoices**: List all invoices
- **list_active_projects**: List active projects
- **list_project_tasks**: List all project tasks
- **list_time_entries**: List recent time tracking entries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cashboard** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my last 5 invoices in Cashboard."

**🤖 AI Agent:**
> Retrieving your recent invoices... I found 5 including Invoice #1001 ($500.00 - Paid) and #1002 ($1,250.00 - Outstanding). Would you like to see the line items for any of these?

---

**👤 You:**
> "What are my active projects right now?"

**🤖 AI Agent:**
> Checking your active projects... You currently have 3 active projects: 'Website Redesign', 'Mobile App Development', and 'Marketing Consultation'.

---

**👤 You:**
> "List my business expenses from the last 30 days."

**🤖 AI Agent:**
> Retrieving your expenses... I found 12 entries in the last 30 days totaling $845.50. The largest expense was 'AWS Hosting' ($120.00).


## ❓ FAQ

**Q: Can I list my billable time entries for this week?**
Yes! Use the `list_time_entries` tool. The agent will return recent time tracking records, allowing you to audit hours worked across your projects.

**Q: How do I check if an invoice has been paid?**
Use the `list_invoices` tool. Your agent will fetch the list of invoices along with their current status (e.g., Paid, Outstanding, Overdue).

**Q: Where do I find my Cashboard API Key?**
Log in to your Cashboard account and look for the 'API' or 'Developer' section in your account settings. If you can't find it, contact Cashboard support.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cashboard](https://vinkius.com/mcp/cashboard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cashboard** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cashboard` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cashboard** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cashboard": {
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

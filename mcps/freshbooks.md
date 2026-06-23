# FreshBooks MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freshbooks)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage small business accounting via FreshBooks — track clients and invoices, handle payments and billing via AI agents.

## Description
Connect your **FreshBooks** account to any AI agent to automate your small business accounting, invoicing, and client management through the Model Context Protocol (MCP). FreshBooks is the leading cloud-based accounting software designed for small businesses and self-employed professionals. This MCP server enables you to manage your clients, track invoice statuses, and retrieve financial summaries directly through natural conversation.

### Key Features

- **Client Management** — List and search for clients, fetch detailed profiles, and maintain full context of your customer relationships.
- **Invoice Lifecycle** — Track sales invoices across all states (Sent, Paid, Overdue) and retrieve detailed line-item metadata.
- **Expense Oversight** — Monitor recorded business expenses and categorize them for better financial tracking.
- **Payment History** — Retrieve a list of all payments received to ensure your cash flow is accurately monitored.
- **Project & Task Tracking** — Access projects, tasks, and time entries to see how they impact your billing and productivity.
- **User Identity** — Fetch global user profile and identity details to ensure you are working in the correct account context.
- **Financial Insights** — Access high-level metadata for your specific FreshBooks business account instantly.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your FreshBooks Account ID and Access Token (found in your Dashboard and App settings)
3. Start managing your business finances from Claude, Cursor, or any MCP client

### Who is this for?

- **Small Business Owners** — quickly check invoice statuses or client data without manual dashboard navigation.
- **Accountants & Bookkeepers** — automate the retrieval of billing histories and payment records via simple AI commands.
- **Freelancers** — track projects, tasks, and time entries while focused on delivery in your primary workspace.


## Available Tools (12)
- **get_account_info**: Get business info
- **get_client_details**: Get client metadata
- **get_invoice_details**: Get invoice metadata
- **get_my_identity**: Get user identity
- **list_expense_categories**: List categories
- **list_clients**: List clients
- **list_expenses**: List tracked expenses
- **list_invoices**: List sales invoices
- **list_payments**: List invoice payments
- **list_active_projects**: List projects
- **list_project_tasks**: List tasks
- **list_time_entries**: List time logs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FreshBooks** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my 5 most recent clients in FreshBooks."

**🤖 AI Agent:**
> Retrieving clients... I found your 5 most recent entries, including 'Acme Corp' and 'Globex Inc'. Would you like the contact details for any of them?

---

**👤 You:**
> "Show me the status of my last 3 invoices."

**🤖 AI Agent:**
> Fetching invoices... Your last 3 invoices are: INV-001 (Paid), INV-002 (Sent), and INV-003 (Overdue). Would you like to see the details for the overdue one?

---

**👤 You:**
> "Get my time tracking entries for this week."

**🤖 AI Agent:**
> Retrieving time entries... I've fetched your logs for this week. You've recorded a total of 32 hours across projects 'Web Design' and 'Consulting'.


## ❓ FAQ

**Q: How do I get an Access Token for FreshBooks?**
You can find your Access Token in your FreshBooks application settings or by creating a Personal Access Token in the FreshBooks Developer Portal.

**Q: Where do I find my FreshBooks Account ID?**
Your Account ID is the unique number visible in your browser's URL bar immediately after '/portal/' when you are logged into FreshBooks.

**Q: Can I see if a specific invoice has been paid?**
Yes! Use the 'get_invoice_details' tool and provide the Invoice ID. The agent will return the current status, including whether it is 'Sent', 'Paid', or 'Overdue'.

**Q: Is time tracking data accessible via the agent?**
Yes, the 'list_time_entries' tool allows you to retrieve all time tracking logs for your business, keeping your project productivity in view.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freshbooks](https://vinkius.com/mcp/freshbooks)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FreshBooks** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `freshbooks` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FreshBooks** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "freshbooks": {
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

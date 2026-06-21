# TurfHop MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/turfhop)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage your lawn care and landscaping business with route planning, job scheduling, and customer billing in one app.

## Description
Connect your **TurfHop** account to any AI agent and simplify how you coordinate your field service operations, scheduling, and billing through natural conversation.

### What you can do

- **Customer Management** — List and search customer records, create new profiles, and retrieve complete service histories.
- **Job Scheduling** — List all service jobs, create new assignments, and update job details or statuses programmatically.
- **Billing & Invoicing** — Monitor your cash flow by listing invoices, quotes, and payment statuses for your services.
- **Service Catalog** — Browse your offered products and services to identify pricing and availability.
- **Operational tracking** — Fetch detailed metadata for specific jobs or customers to stay on top of your mobile workforce.

### How it works

1. Subscribe to this server
2. Enter your TurfHop API Key (found in your account settings)
3. Start managing your field services from Claude, Cursor, or any MCP client

### Who is this for?

- **Field Service Business Owners** — quickly check job statuses and manage client records via simple AI commands.
- **Operations Managers** — schedule new assignments and track team progress directly from the workspace.
- **Administrative Staff** — monitor invoices and quotes to maintain an organized billing cycle via the AI assistant.


## Available Tools
- **create_customer**: Pass customer data as a JSON string.

Create a new customer
- **create_job**: Pass job data as a JSON string.

Create a new service job
- **get_customer**: Get customer details by ID
- **get_invoice**: Get invoice details
- **get_job**: Get job details
- **list_customers**: List all customers
- **list_invoices**: List all invoices
- **list_jobs**: List all service jobs
- **list_products**: List all products and services
- **list_quotes**: List all quotes
- **update_customer**: Update an existing customer
- **update_job**: Update an existing job


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TurfHop** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active service jobs in my TurfHop account."

**🤖 AI Agent:**
> I've retrieved your jobs. You have 3 active assignments: 'Weekly Mowing' for John Doe, 'Gutter Cleaning' for Smith Residence, and 'Fertilization' for Tech Campus. Which one would you like details on?

---

**👤 You:**
> "Search for a customer named 'Michael Scott'."

**🤖 AI Agent:**
> I've found the record. Michael Scott (ID: cust_10293) is a registered customer. He has an outstanding balance of $120 and his last service was completed last Tuesday. Shall I retrieve his full history?

---

**👤 You:**
> "Show me all unpaid invoices from this month."

**🤖 AI Agent:**
> Fetching invoices... I found 2 unpaid invoices: #INV-8823 ($250.00) and #INV-8824 ($45.50). Both are marked as 'Sent' but not yet paid. Would you like to check the associated customer details?


## ❓ FAQ

**Q: Can I search for a customer by their name?**
Yes! Use the `list_customers` tool. While it returns the full list, you can ask the AI agent to find a specific person or retrieve details for a specific ID using `get_customer`.

**Q: How do I schedule a new service job via AI?**
Use the `create_job` action. You'll need to provide a JSON string containing the job details like `customer_id`, `title`, and `start_date` to register the new assignment.

**Q: Is it possible to see the payment status of an invoice?**
Absolutely. Use the `get_invoice` tool and provide the Invoice ID. The agent will retrieve the complete metadata, including whether the invoice is paid, pending, or overdue.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/turfhop](https://vinkius.com/mcp/turfhop)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TurfHop** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `turfhop` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TurfHop** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "turfhop": {
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

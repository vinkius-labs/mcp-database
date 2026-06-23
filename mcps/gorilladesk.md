# GorillaDesk MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gorilladesk)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage field service operations — schedule jobs, invoice customers, and update notes via AI.

## Description
Connect your **GorillaDesk** account to your AI agent and streamline your field service management. Use natural language to query customer records, check job statuses, and manage invoices without manually navigating the software interface.

### What you can do

- **Customer Management** — Search for customers, view their details, and create or update customer profiles instantly
- **Job Tracking** — List upcoming or past jobs (work orders) and retrieve specific details to keep your team aligned
- **Invoicing** — Check the status of unpaid invoices and review billing details for specific customers
- **Note Taking** — Read and add notes to customer profiles directly from the chat to ensure your technicians have all the context they need

### How it works

1. Subscribe to this server
2. Enter your GorillaDesk API Key (generated in the Addons page)
3. Start managing your field service operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Dispatchers & Office Managers** — quickly look up a customer's address and upcoming job schedule while on a call
- **Field Technicians** — add notes to a customer's file via voice-to-text chat immediately after completing a job
- **Business Owners** — check the total number of open invoices or review customer details without logging into the main dashboard


## Available Tools (12)
- **create_customer**: Create a new customer profile
- **create_note**: Add a note to a customer profile
- **get_company**: Get details for the current GorillaDesk company account
- **get_customer**: Get details for a specific customer
- **get_invoice**: Get details of a specific invoice
- **get_job**: Get details of a specific job
- **list_customers**: List or search for customers
- **list_invoices**: List invoices
- **list_jobs**: List upcoming or past jobs (work orders)
- **list_notes**: List notes for a specific customer
- **list_users**: List all users/technicians in the account
- **update_customer**: Update an existing customer


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GorillaDesk** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find the customer record for john@example.com."

**🤖 AI Agent:**
> Searching customers... I found one match: John Doe (ID: 93021). His primary address is 123 Main St, and his current account status is 'Active'. Would you like to see his recent jobs?

---

**👤 You:**
> "Show me the details for job ID 88392."

**🤖 AI Agent:**
> Fetching job details... Job #88392 is for 'Quarterly Pest Control' at John Doe's residence. It is scheduled for tomorrow at 2:00 PM, assigned to technician Mike R. The status is currently 'Confirmed'.

---

**👤 You:**
> "Check the schedule logic for Mike R. tomorrow and list all his confirmed routes."

**🤖 AI Agent:**
> Analyzing tomorrow's manifest... Mike R. has 4 confirmed pest control jobs logically spaced out. First stop is at 8:00 AM, finishing his primary route efficiently by 3:00 PM solidly.


## ❓ FAQ

**Q: Can I add notes to a customer's profile using this integration?**
Yes! Use the `create_note` tool. You just need to provide the Customer ID and the text of the note. It will be instantly added to their profile for your technicians to see.

**Q: How do I filter unpaid invoices?**
You can use the `list_invoices` tool and pass 'unpaid' (or the equivalent status parameter specified in GorillaDesk) to quickly retrieve a list of outstanding balances.

**Q: Can I check the schedules for specific field technicians?**
Absolutely. By utilizing the schedule-checking tool with a technician's name or ID, the agent retrieves their complete run-sheet for the requested day.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gorilladesk](https://vinkius.com/mcp/gorilladesk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GorillaDesk** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gorilladesk` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GorillaDesk** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gorilladesk": {
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

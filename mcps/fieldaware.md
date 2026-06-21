# FieldAware MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fieldaware)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [field-service-management](../categories/field-service-management.md)

Connect FieldAware to automate field service management — manage jobs, customers, and invoices directly from your AI agent.

## Description
FieldAware is a comprehensive field service management platform. This MCP server allows your AI agent to interact with your FieldAware account flawlessly.

### Key Features
- **Job Orchestration** — List all active jobs and fetch detailed metadata for specific work orders natively.
- **Customer Intelligence** — Access customer profiles and contact details to personalize service interactions flawlessly.
- **Invoice Management** — Retrieve and inspect invoices to stay updated on billing and payments synchronously.
- **Asset Tracking** — List managed assets and equipment to ensure your field team has the right context natively.
- **Quote & Item Access** — Query active quotes and your product/service catalog flawlessly through the agent.
- **Identity Verification** — Verify the authorized user and permissions for the current API key flawlessly.

### How it works
1. Subscribe to this server
2. Enter your FieldAware API Key (found in your developer settings)
3. Start managing your field operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Service Managers** — monitor job progress and customer status without manual portal navigation
- **Operations Teams** — sync work orders and equipment data directly from your chat workflow
- **Field Dispatchers** — quickly look up customer history and asset details through simple natural language queries


## Available Tools
- **create_job**: Create a new job
- **get_customer**: Get details for a specific customer
- **get_invoice**: Get details for a specific invoice
- **get_job**: Get details for a specific job
- **get_whoami**: Identify the user associated with the current API key
- **list_assets**: List all assets
- **list_contacts**: List all contacts
- **list_customers**: List all customers
- **list_invoices**: List all invoices
- **list_items**: List all items (products/services)
- **list_jobs**: List all jobs
- **list_quotes**: List all quotes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FieldAware** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active jobs in FieldAware."

**🤖 AI Agent:**
> I've retrieved your jobs. You have 8 active assignments including 'AC Repair' (Job ID: 5501) and 'Annual Inspection' (Job ID: 5502). Which one would you like to see the details for?

---

**👤 You:**
> "Show me the contact info for customer ID 12345."

**🤖 AI Agent:**
> Inspecting customer... ID 12345 is 'Global Tech Corp'. The primary contact is 'Sarah Miller' at sarah@globaltech.com. Shall I also check their active service locations?

---

**👤 You:**
> "Check if there are any unpaid invoices."

**🤖 AI Agent:**
> Retrieving invoices... I found 3 unpaid invoices: INV-901 ($450), INV-902 ($1,200), and INV-905 ($350). Would you like to see the associated job details for these?


## ❓ FAQ

**Q: How do I obtain my FieldAware API Key?**
You can request or generate your API Key from your FieldAware account administrator or within the **Developer/API Settings** section of your FieldAware portal.

**Q: What is the format for the API Key in the settings?**
The agent automatically handles the 'Token' prefix. You only need to paste the literal API key provided by FieldAware.

**Q: Can I create new jobs through this agent?**
Yes! The `create_job` tool allows you to programmatically generate new work orders by providing a customer ID and description.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fieldaware](https://vinkius.com/mcp/fieldaware)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FieldAware** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `fieldaware` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FieldAware** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fieldaware": {
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

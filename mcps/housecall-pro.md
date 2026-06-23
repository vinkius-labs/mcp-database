# Housecall Pro MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/housecall-pro)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage home service jobs, customers, and invoices via Housecall Pro API.

## Description
Connect your AI agents to Housecall Pro to streamline your home service business. This MCP server allows you to list and manage jobs, track customer details, view estimates, monitor invoices, and see your team of technicians directly through the Housecall Pro API. Ideal for automating scheduling and billing workflows.


## Available Tools (10)
- **get_company**: Gets your company information
- **get_customer**: Retrieves details for a specific customer
- **get_job**: Retrieves details for a specific job
- **list_customers**: Lists customers
- **list_estimates**: Lists estimates sent to customers
- **list_invoices**: Lists invoices
- **list_jobs**: Lists service jobs
- **list_price_list_items**: Lists items in your price list
- **list_technicians**: Lists technicians/employees
- **list_webhooks**: Lists configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Housecall Pro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active jobs for today in Housecall Pro."

**🤖 AI Agent:**
> I'll retrieve today's job list for you.

---

**👤 You:**
> "Show me details for customer ID 789."

**🤖 AI Agent:**
> I'll fetch that customer's information.

---

**👤 You:**
> "Check for unpaid invoices."

**🤖 AI Agent:**
> I'll look up your pending invoices.


## ❓ FAQ

**Q: Where do I find my Housecall Pro API Key?**
Log in to Housecall Pro, go to the App Store, and find the API integration to generate your key.

**Q: Is this for Pros or Partners?**
This MCP is designed for Pros using their own API keys for custom integrations.

**Q: Can I see technician schedules?**
Yes, the list_technicians and list_jobs tools help you track team activity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/housecall-pro](https://vinkius.com/mcp/housecall-pro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Housecall Pro** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `housecall-pro` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Housecall Pro** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "housecall-pro": {
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

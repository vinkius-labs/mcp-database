# Belong Australia MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/belong-australia)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Manage your Belong mobile and broadband services — track usage, list invoices, and check account balance directly from any AI agent.

## Description
Connect your **Belong Australia** account to any AI agent and manage your telecommunications services through natural conversation.

### What you can do

- **Service Oversight** — List and inspect all active mobile and broadband services linked to your account.
- **Usage Tracking** — Retrieve real-time data usage statistics to avoid overages and stay informed.
- **Billing Management** — List recent invoices and retrieve direct PDF links for auditing and payment.
- **Order Monitoring** — Check the status of recent orders and service modifications.
- **Account Health** — View your current account balance and saved payment methods instantly.

### How it works

1. Subscribe to this server
2. Enter your Belong OAuth Access Token
3. Start managing your services from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Belong Customers** — quickly check data balances and recent bills without logging into the mobile app.
- **Household Managers** — monitor multiple services and broadband usage through simple questions.
- **Business Users** — retrieve invoice summaries for expense reporting directly from their workflow.


## Available Tools
- **get_account_balance**: Check current account balance
- **get_invoice_pdf**: Retrieve a specific invoice PDF link
- **get_order_details**: Get details of a specific order
- **get_service_details**: Get details of a specific service
- **get_usage_data**: Retrieve data usage for a service
- **get_user_profile**: Get Belong user profile
- **list_invoices**: List recent invoices
- **list_orders**: List recent orders
- **list_payment_methods**: List saved payment methods
- **list_services**: List active mobile and broadband services


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Belong Australia** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active services in my Belong account."

**🤖 AI Agent:**
> I've retrieved your services. You have 2 active plans: 'Mobile 20GB' (ID: svc_123) and 'Broadband Unlimited' (ID: svc_456). Which one would you like to check usage for?

---

**👤 You:**
> "Check data usage for my mobile plan svc_123."

**🤖 AI Agent:**
> You have used 12.5GB of your 20GB monthly allowance. You still have 7.5GB remaining for the current billing cycle.

---

**👤 You:**
> "Show my recent account balance and payment methods."

**🤖 AI Agent:**
> Your current account balance is $0.00. I found 1 saved payment method: 'Visa ending in 1234'. Your next bill is scheduled for April 15th.


## ❓ FAQ

**Q: Can I check how much data I have left on my mobile plan?**
Yes! Use the `get_usage_data` tool with your Service ID. Your agent will fetch the latest data consumption statistics directly from Belong.

**Q: How do I see my last 3 invoices?**
Simply ask the agent to `list_invoices`. It will retrieve the history of recent bills linked to your account, showing dates and amounts.

**Q: Does the integration allow me to change my internet plan?**
Currently, the toolset focuses on querying and monitoring (Read-Only). You can list and inspect services, usage, and invoices, but plan changes must be performed via the official Belong website or mobile app for security.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/belong-australia](https://vinkius.com/mcp/belong-australia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Belong Australia** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `belong-australia` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Belong Australia** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "belong-australia": {
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

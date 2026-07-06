# Cheddar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cheddar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage usage-based billing and subscriptions via Cheddar — track usage, monitor invoices, and manage customers directly from any AI agent.

## Description
Connect your **Cheddar (formerly CheddarGetter)** account to any AI agent and take full control of your recurring and usage-based billing through natural conversation. Streamline how you manage subscriptions and tracked items.

### What you can do

- **Customer Oversight** — List and retrieve details for all active and inactive customers natively
- **Plan Management** — Access and monitor available pricing plans and their configurations flawlessly
- **Usage Tracking** — Add one-time or quantity-based charges to customer accounts securely
- **Invoice Intelligence** — List and retrieve details for recent customer invoices and billing history flawlessly
- **Transaction Auditing** — Access and monitor all billing transactions and payment statuses securely
- **Product Analytics** — Retrieve core product information, configuration metadata, and active promotions flawlessly

### How it works

1. Subscribe to this server
2. Enter your Cheddar Email, Product Secret, and Product Code
3. Start managing your usage-based billing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SaaS Founders** — monitor subscription revenue and customer growth using natural language
- **Billing Administrators** — audit invoices and track usage without opening the dashboard
- **Support Teams** — quickly look up customer billing history and apply charges straight from their chat interface
- **Financial Analysts** — verify transaction volumes and promotion effectiveness


## Available Tools (8)
- **get_cheddar_customer_details**: Get detailed information for a specific customer
- **add_cheddar_charge**: Add a one-time or quantity-based charge to a customer
- **get_cheddar_product_info**: Retrieve core product and configuration information
- **list_cheddar_customers**: List all customers for the product
- **list_cheddar_invoices**: List recent customer invoices
- **list_cheddar_plans**: List all available pricing plans
- **list_cheddar_promotions**: List active promotions and coupons
- **list_cheddar_transactions**: List recent billing transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cheddar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the last 5 invoices in Cheddar."

**🤖 AI Agent:**
> Retrieving your recent invoices... I found 5 items totaling $1,850.00. 3 are 'Settled' and 2 are 'Pending'. Would you like to see the customer associated with each?

---

**👤 You:**
> "Add 10 units of usage for customer 'ACME-123' under charge code 'API_CALLS'."

**🤖 AI Agent:**
> Adding usage... 10 units of 'API_CALLS' have been successfully recorded for ACME-123. This will be reflected in their next billing cycle.

---

**👤 You:**
> "List all my available pricing plans in Cheddar."

**🤖 AI Agent:**
> Checking plans... You have 3 active plans: 'Basic' ($29/mo), 'Pro' ($99/mo), and 'Enterprise' (Usage-based). I can show you the specific tracked items for each.


## ❓ FAQ

**Q: Can I record a new usage event for a customer?**
Yes! Use the `add_cheddar_charge` tool with the customer code, charge code (tracked item), and quantity. The agent will record the usage in Cheddar immediately.

**Q: How do I see the billing history for a specific person?**
Use the `get_cheddar_customer_details` tool with the unique customer code. Your agent will fetch the full record, including active plans, status, and associated invoices.

**Q: Where do I find my Product Secret and Product Code?**
Log in to your Cheddar dashboard and look for 'Product Settings'. You can view and copy your unique Product Code and generate a Secret Key from there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cheddar](https://vinkius.com/mcp/cheddar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cheddar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cheddar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cheddar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cheddar": {
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

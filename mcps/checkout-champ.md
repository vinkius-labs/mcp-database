# Checkout Champ MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/checkout-champ)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage CRM and order workflows via Checkout Champ — track leads, monitor orders, and analyze transactions directly from any AI agent.

## Description
Connect your **Checkout Champ** account to any AI agent and take full control of your e-commerce CRM and order management through natural conversation. Streamline your sales funnel and customer logistics.

### What you can do

- **Order Oversight** — List and retrieve details for all customer orders and fulfillment statuses natively
- **Lead Intelligence** — Access and monitor captured leads to understand your sales pipeline flawlessly
- **Transaction Auditing** — List and review financial transactions and payment gateway responses securely
- **Customer Management** — Access detailed customer profiles and their complete interaction history flawlessly
- **Campaign Tracking** — List configured marketing campaigns and retrieve their performance metadata flawlessly
- **Product Logistics** — Access your product catalog and retrieve master data directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Checkout Champ API Login ID and Password
3. Start managing your CRM from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Store Owners** — monitor order volumes and lead generation using natural language
- **Sales Operations** — audit transaction success rates and customer data without opening the CRM
- **Marketing Teams** — quickly look up campaign details and lead profiles straight from their chat interface
- **Support Staff** — verify customer order history and transaction details for resolving inquiries


## Available Tools
- **get_champ_customer_details**: Get detailed information for a specific customer
- **get_champ_order_details**: Get detailed information for a specific order
- **list_champ_campaigns**: List configured marketing campaigns
- **list_champ_customers**: List customers in the CRM
- **list_champ_leads**: List captured leads
- **list_champ_orders**: List orders from Checkout Champ
- **list_champ_products**: List products in the catalog
- **list_champ_transactions**: List recent financial transactions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Checkout Champ** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the last 5 orders in Checkout Champ."

**🤖 AI Agent:**
> Retrieving recent orders... I found 5 items: Order #12345 (John Doe - $99.00), #12346 (Jane Smith - $45.00), and 3 others. Would you like to check the shipping status for any of these?

---

**👤 You:**
> "What is my total sales volume for today?"

**🤖 AI Agent:**
> Checking today's transactions... You have 15 successful orders totaling $1,250.00 and 2 declined transactions. Would you like to see the decline reasons?

---

**👤 You:**
> "List all active campaigns."

**🤖 AI Agent:**
> Retrieving active campaigns... I found 3: 'Summer Sale 2024', 'Retargeting Blitz', and 'New Product Launch'. I can provide performance data for each if you'd like.


## ❓ FAQ

**Q: Can I see the reason why a transaction failed?**
Yes! Use the `list_champ_transactions` tool. The agent will retrieve recent transactions including the decline reason and response from the payment gateway.

**Q: How do I list my latest leads from a specific campaign?**
Use the `list_champ_leads` tool. You can then ask the agent to filter the results by campaign name or ID to see who signed up recently.

**Q: Where do I find my API Login ID and Password?**
Log in to Checkout Champ and go to the 'Settings' or 'Admin' section to manage API Users. You can create a dedicated API user and get the credentials there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/checkout-champ](https://vinkius.com/mcp/checkout-champ)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Checkout Champ** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `checkout-champ` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Checkout Champ** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "checkout-champ": {
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

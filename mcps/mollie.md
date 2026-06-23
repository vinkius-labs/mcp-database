# Mollie MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mollie)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [money-moves](../categories/money-moves.md)

Manage payments, orders, and customers via Mollie — track transactions and manage your e-commerce finances directly from your AI agent.

## Description
Connect your **Mollie** merchant account to your AI agent and take control of your payment workflows and e-commerce operations through natural conversation.

### What you can do

- **Payment Tracking** — List all transactions and get real-time status updates, amounts, and metadata.
- **Order Management** — View e-commerce orders, including line items and fulfillment status.
- **Customer Insights** — Access customer profiles, payment history, and saved details.
- **Refunds & Chargebacks** — Monitor your refund history and stay informed about disputed payments (chargebacks).
- **Create Payments** — Generate new payment links with custom amounts, currencies, and descriptions.
- **Deep Inspection** — Fetch complete details for specific payments, orders, or customers using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your Mollie API Key (Live or Test)
3. Start managing your finances from Claude, Cursor, or any MCP client

### Who is this for?

- **E-commerce Owners** — quickly check if a customer's payment has been received without opening the Mollie dashboard.
- **Support Teams** — verify order statuses and transaction details while assisting customers.
- **Finance Teams** — automate the retrieval of payment and refund lists for reconciliation and reporting.


## Available Tools (10)
- **create_payment**: Create a new Mollie payment
- **get_customer**: g., cst_8wmqcHMN4U).

Get specific customer details
- **get_order**: g., ord_st9n7), including line items and shipping info.

Get details for a specific order
- **get_payment**: g., tr_7UhVrS0eba).

Get details for a specific payment
- **get_refund**: Get specific refund details
- **list_chargebacks**: List payment chargebacks
- **list_customers**: List Mollie customers
- **list_orders**: List all e-commerce orders
- **list_payments**: List all Mollie payments
- **list_refunds**: List all payment refunds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mollie** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my 5 most recent payments and their current status."

**🤖 AI Agent:**
> I've retrieved your recent transactions. You have 5 recent payments: three are 'paid' (totaling €150.00), one is 'open' (waiting for payment), and one is 'expired'. Would you like more details on the open payment?

---

**👤 You:**
> "Create a new payment link for €45.00 for 'Service Invoice #123'."

**🤖 AI Agent:**
> I've generated the payment link for 'Service Invoice #123'. The amount is €45.00 and you can send this URL to your customer: https://www.mollie.com/checkout/select-method/7PrMmS. The payment is currently in 'open' status.

---

**👤 You:**
> "Show me my refund history."

**🤖 AI Agent:**
> Retrieving your refunds... You have processed 3 refunds recently: two for 'Service Refund' (€20.00 each) and one for 'Returned Product' (€55.00). All are marked as 'succeeded'.


## ❓ FAQ

**Q: Does this server support Mollie's Test Mode?**
Yes! Simply provide your Test API Key instead of your Live API Key during authentication. The agent will then interact with your test environment.

**Q: Can I see exactly what items were in a specific order?**
Yes. Use the `get_order` tool with an Order ID (starting with `ord_`). Your agent will return the full breakdown of products, prices, and shipping details.

**Q: How do I check for disputed payments?**
Use the `list_chargebacks` tool to see a list of all transactions that have been disputed by customers through their banks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mollie](https://vinkius.com/mcp/mollie)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mollie** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mollie` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mollie** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mollie": {
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

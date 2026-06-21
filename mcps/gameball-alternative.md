# Gameball MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gameball-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Automate loyalty programs and gamification via Gameball — manage customer profiles, track points, and handle order rewards directly from any AI agent.

## Description
Connect your **Gameball** account to any AI agent to orchestrate your loyalty and retention strategies through natural conversation.

### What you can do

- **Customer Management** — Create or update customer profiles with custom attributes and contact details instantly.
- **Points & Balances** — Retrieve real-time points balances, monetary values, and upcoming expiration dates for any customer.
- **Transaction Control** — Hold points for temporary redemption to prevent double-spending during checkout processes.
- **Order Tracking** — Submit order details to automatically award loyalty points and finalize held redemptions.
- **Refund Handling** — Process refunds or cancellations to reverse points earned or restore points redeemed accurately.

### How it works

1. Subscribe to this server
2. Enter your Gameball API Key (and optional Secret Key)
3. Start managing your loyalty ecosystem from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **E-commerce Managers** — quickly check customer loyalty tiers and reward status without leaving your workflow.
- **Growth & Marketing Teams** — automate customer profiling and event tracking to drive retention.
- **Support Teams** — handle point refunds and balance inquiries directly within the chat interface.


## Available Tools
- **create_or_update_customer**: This API is idempotent.

Create or update a Gameball customer profile
- **get_customer_activities**: Get a log of customer activities
- **get_customer_balance**: Get a customer's points balance
- **get_order_transactions**: Get all loyalty transactions for an order
- **hold_points**: Holds typically expire after 10 minutes.

Hold points for temporary redemption
- **refund_transaction**: Refund a transaction
- **send_events**: Send customer events
- **track_order**: Track an order to award points and finalize redemptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gameball** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the points balance for customer ID 'cust_98765'."

**🤖 AI Agent:**
> I've retrieved the balance for customer cust_98765. They currently have 1,250 points (valued at $12.50). Note that 200 points are set to expire on the 30th of next month.

---

**👤 You:**
> "Track a new order of $150 for customer 'cust_123' with order ID 'ORD-999'."

**🤖 AI Agent:**
> Order ORD-999 has been successfully tracked for customer cust_123. Based on the $150 total, the customer has been awarded 150 loyalty points.

---

**👤 You:**
> "Create a customer profile for 'Alice Smith' with email 'alice@example.com' and ID 'alice_001'."

**🤖 AI Agent:**
> I've created the profile for Alice Smith (ID: alice_001). Her details are now synchronized with Gameball for loyalty tracking.


## ❓ FAQ

**Q: How can I check a customer's current points balance?**
Use the `get_customer_balance` tool by providing the unique Customer ID. The agent will return the points balance, their monetary value, and any points nearing expiration.

**Q: Can I reserve points during a checkout process to prevent double-spending?**
Yes! The `hold_points` action allows you to temporarily lock a specific amount of points for a customer, ensuring they aren't used elsewhere while the transaction is being finalized.

**Q: How do I reward points to a customer for a new purchase?**
Use the `track_order` tool. By submitting the order ID and total price, Gameball will automatically calculate and award the appropriate loyalty points based on your configured rules.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gameball-alternative](https://vinkius.com/mcp/gameball-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gameball** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `gameball-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gameball** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gameball-alternative": {
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

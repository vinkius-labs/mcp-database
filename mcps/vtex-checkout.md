# VTEX Checkout MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vtex-checkout)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Simulate carts, calculate shipping, apply coupons, and manage client profiles on your VTEX store — all from any AI agent.

## Description
Connect your **VTEX** e-commerce checkout API to any AI agent and streamline your store's pre-purchase operations through natural conversation.

### What you can do

- **Cart Simulation** — Run complete order simulations with items, quantities, and sellers to instantly preview totals, discounts, and available shipping options for any postal code.
- **Shopping Cart Management** — Retrieve the full state of any active shopping cart (orderform), including items, client profile, payment conditions, and logistics.
- **Coupon Management** — Apply discount coupons to active carts and immediately see the impact on totals.
- **Client Profiles** — Look up registered client profiles by user ID — retrieve name, CPF/CNPJ, email, and contact details.
- **Address Management** — Register new shipping addresses for clients, streamlining the checkout flow.
- **Payment Simulation** — Validate payment tokens and simulate payment conditions before placing an order.

### How it works

1. Subscribe to this server
2. Enter your VTEX Account Name, App Key, and App Token (found in **Account Settings → Application Keys** in your VTEX Admin)
3. Start simulating carts and managing checkout data from Claude, Cursor, or any MCP-compatible agent

### Who is this for?

- **E-Commerce Managers** — Quickly simulate cart scenarios during promotions, flash sales, or seasonal campaigns without navigating the full admin.
- **Support Teams** — Look up client profiles and cart states instantly during live support conversations.
- **Operations Teams** — Validate shipping costs and coupon rules across different regions and postal codes.


## Available Tools (6)
- **create_address**: Add a new address to a client profile
- **get_client_profile**: Get client profile details
- **add_coupon**: Apply a coupon to a shopping cart
- **get_orderform**: Get details of a specific shopping cart
- **simulate_payment**: Simulate a payment validation
- **simulate_order**: Simulate a cart and shipping costs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VTEX Checkout** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Simulate a cart with 2 units of product ID 1234 and shipping to ZIP 01310-100"

**🤖 AI Agent:**
> Cart simulation complete! **Total: R$ 259.80** (2x Widget Pro @ R$ 129.90 each). Shipping options to 01310-100:

🚚 **Standard** — R$ 12.50 (5-7 business days)
⚡ **Express** — R$ 29.90 (1-2 business days)
🆓 **Free Shipping** — eligible (order above R$ 200)

---

**👤 You:**
> "Apply coupon code SUMMER20 to orderform abc123"

**🤖 AI Agent:**
> Coupon **SUMMER20** applied successfully to orderform `abc123`! Discount: **-R$ 51.96 (20% off)**. New total: R$ 207.84. The coupon is now active and will be retained until the order is placed or the cart expires.

---

**👤 You:**
> "Look up the client profile for user ID 98765"

**🤖 AI Agent:**
> Client found: **Maria Silva** (maria@example.com). Document: CPF 123.456.789-00. Phone: +55 11 98765-4321. This client has 3 saved addresses and 12 previous orders.


## ❓ FAQ

**Q: How do I get my VTEX API credentials?**
Log in to your VTEX Admin, go to **Account Settings → Application Keys**, and create a new App Key. You'll receive an App Key and App Token pair. You also need your Account Name (the subdomain you use to access the VTEX Admin, e.g., 'mystore'). No code, no SDK — just connect and go.

**Q: Can my agent simulate a full cart with shipping costs?**
Yes! Use the 'simulate_order' tool with a list of items and a postal code. Your agent will return the full cart breakdown — totals, per-item pricing, available logistics options, estimated delivery dates, and applicable discounts — all without touching the actual store.

**Q: What happens when a customer asks support about their current cart?**
Your support agent can use the 'get_orderform' tool to instantly retrieve the customer's active cart — items, quantities, prices, applied coupons, and shipping address. No need to switch tabs or navigate the admin. The agent can then apply a coupon or check shipping costs, all within the same conversation.

**Q: Can I validate payment conditions before placing bulk orders?**
Absolutely. The 'simulate_payment' tool lets your agent validate payment tokens and check accepted conditions — perfect for operations teams running bulk order validations across multiple sellers and payment methods without processing real transactions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vtex-checkout](https://vinkius.com/mcp/vtex-checkout)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **VTEX Checkout** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vtex-checkout` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **VTEX Checkout** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vtex-checkout": {
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

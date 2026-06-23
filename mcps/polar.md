# Polar MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/polar)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage digital products, subscriptions, orders and customers via Polar — create checkouts, manage discounts and track revenue from any AI agent.

## Description
Connect your **Polar** account to any AI agent and take full control of your digital commerce operations through natural conversation.

### What you can do

- **Product Management** — List, retrieve and audit all products (one-time, subscription, free) with pricing and metadata
- **Subscription Tracking** — Monitor active, canceled and past_due subscriptions with billing periods and customer info
- **Order & Revenue** — List completed orders with amounts, currency, payment status and customer details
- **Customer Discovery** — Browse customers by email, name and purchase history
- **Discount Management** — List, create and audit discount codes with percentage or fixed-amount types
- **Checkout Operations** — Create checkout sessions for products and track open, expired and confirmed checkouts
- **Webhook Audit** — Review configured webhook endpoints and their subscribed events

### How it works

1. Subscribe to this server
2. Enter your Polar Personal Access Token
3. Start managing your commerce from Claude, Cursor, or any MCP-compatible client

No more clicking through the Polar dashboard to check subscriptions or create discount codes. Your AI acts as a dedicated commerce engineer.

### Who is this for?

- **Indie Developers** — quickly check subscription status, review orders and create discount codes without leaving your IDE
- **Commerce Teams** — audit product catalog, track revenue via orders and manage customer data
- **Marketing** — create promotional discounts, track checkout conversion and review webhook integrations


## Available Tools (10)
- **create_checkout**: Requires the product ID. Optionally associate with an existing customer and apply a discount. Returns the checkout session with its URL that you can redirect customers to for payment.

Create a new checkout session in Polar
- **create_discount**: Requires the name, code, type (percentage or fixed_amount), and amount. Optionally set the duration (once, forever, repeating). The discount can be applied during checkout.

Create a new discount code in Polar
- **get_product**: Provide the product ID (UUID format).

Get details for a specific Polar product
- **list_checkouts**: Each checkout shows its status (open, expired, confirmed), associated product, customer, and creation date. Useful for tracking abandoned and completed checkouts.

List checkout sessions in your Polar store
- **list_customers**: Each customer shows their email, name, billing address, and metadata. Optionally filter by email to find a specific customer.

List customers in your Polar store
- **list_discounts**: Each discount shows its code, type (percentage, fixed_amount), amount, duration (once, forever, repeating), and active status. Use this to audit your promotional offers.

List discount codes in your Polar store
- **list_orders**: Each order shows the customer, product, amount, currency, payment status, and creation date. Useful for tracking revenue and verifying successful transactions.

List orders in your Polar store
- **list_products**: Each product includes its name, description, price, type (one-time, subscription, free), and metadata. Use this to audit your product catalog and see what you are selling.

List products in your Polar store
- **list_subscriptions**: Each subscription shows the customer, product, status (active, past_due, canceled, expired, incomplete, trialing), current period start/end dates, and amount. Optionally filter by status and set a limit.

List subscriptions in your Polar store
- **list_webhooks**: Each webhook shows its URL, subscribed events (order.created, subscription.active, etc.), and status. Use this to audit your event integrations.

List webhook endpoints in your Polar store


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Polar** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all active subscriptions and their total monthly revenue."

**🤖 AI Agent:**
> I found 23 active subscriptions. Monthly recurring revenue is $1,847 across 12 products. The top product is 'Pro Plan' at $29/mo (18 subscribers). Would you like a breakdown by product?

---

**👤 You:**
> "Create a 20% discount code called 'LAUNCH20' for the summer sale."

**🤖 AI Agent:**
> Done! I've created the discount code 'LAUNCH20' with 20% off, duration set to 'once'. Customers can now apply this code during checkout. The discount is active immediately.

---

**👤 You:**
> "Show me all orders from the last 30 days."

**🤖 AI Agent:**
> I found 47 orders totaling $3,219.50. The highest-value order was $199.00 for 'Enterprise Plan'. Average order value is $68.50. Would you like details on any specific order?


## ❓ FAQ

**Q: How do I create a Polar Personal Access Token?**
Log in to the [**Polar Dashboard**](https://polar.sh), go to **Settings > Developer > Personal Access Tokens**, click **Create Token**, give it a name and copy the token immediately — it starts with `polar_pat_` and won't be shown again.

**Q: Can I create discount codes via the agent?**
Yes! Use the `create_discount` tool with a name, code, type (percentage or fixed_amount) and amount. Optionally set the duration (once, forever, repeating). The discount will be available during checkout.

**Q: Can I check my subscription revenue?**
Yes! Use `list_subscriptions` with status 'active' to see all active subscriptions, and `list_orders` to see completed orders with their amounts. Combine both to get a full picture of your recurring and one-time revenue.

**Q: Can I create checkout links programmatically?**
Yes! Use `create_checkout` with a product_id and optionally a customer_id and discount_id. This creates a checkout session that returns a URL you can share with customers or embed in your app.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/polar](https://vinkius.com/mcp/polar)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Polar** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `polar` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Polar** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "polar": {
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

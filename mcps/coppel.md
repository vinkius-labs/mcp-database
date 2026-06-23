# Coppel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coppel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate retail operations via Coppel — browse products, manage orders, check customer credit, and find stores across Mexico from any AI agent.

## Description
Connect your **Coppel** B2B account to any AI agent and manage Mexico's largest department store and consumer credit ecosystem through natural conversation.

### What you can do

- **Product Catalog** — Browse, search, and inspect Coppel's massive catalog spanning electronics, furniture, appliances, clothing, and shoes with real-time pricing
- **Order Management** — Create orders, track fulfillment status, and review complete order histories with payment breakdowns
- **Customer Credit Intelligence** — Query any customer's Coppel credit account: approved limits, current balances, weekly payment amounts (abonos semanales), and payment history
- **Store Locator** — Search through 1,700+ Coppel retail stores across all Mexican states with addresses, hours, and available services
- **Promotions & Campaigns** — Access active seasonal promotions (Buen Fin, Hot Sale), category discounts, and interest-free credit offers

### How it works

1. Subscribe to this server
2. Enter your Coppel API Key and Secret
3. Start managing retail operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Store Managers** — check product availability and customer credit without navigating internal systems
- **Sales Representatives** — quickly look up product details and credit options for walk-in customers
- **Financial Analysts** — query credit portfolio data and payment collection performance programmatically


## Available Tools (14)
- **create_order**: Specify the product IDs, quantities, delivery address, and payment method. Credit-eligible customers can select weekly payment plans (abonos semanales).

Place a new order
- **get_customer_credit**: Coppel is famous for its consumer credit program serving Mexico's underbanked population.

Check a customer's Coppel credit status
- **get_customer**: Get full details of a specific customer
- **get_order**: Get full details of a specific order
- **get_product**: Get full details of a specific product
- **get_store**: Get details of a specific store
- **list_categories**: List all product categories
- **list_customers**: List registered customers
- **list_orders**: Filter by status to find pending or delivered orders.

List customer orders
- **list_payments**: Shows payment amounts, dates, methods (weekly installment, cash at store, card), and receipt references.

List payments for an order or account
- **list_products**: Products span electronics, furniture, appliances, clothing, and shoes. Filter by category for targeted browsing.

List products from the Coppel catalog
- **list_promotions**: List active promotions and deals
- **list_stores**: Filter by state to find stores in a specific Mexican state (e.g., "Jalisco", "CDMX").

List Coppel physical store locations
- **search_products**: Returns matching products with pricing and credit plan availability.

Search products by keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Coppel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for Samsung TVs under $15,000 MXN in the Coppel catalog."

**🤖 AI Agent:**
> I found 6 Samsung TVs under $15,000 MXN: 1. Samsung Crystal UHD 43" — $8,999 (weekly: $175 x 60 weeks). 2. Samsung Crystal UHD 50" — $11,499 (weekly: $222 x 60 weeks). 3. Samsung LED 32" — $4,599 (weekly: $89 x 60 weeks). Would you like the full specs on any of these?

---

**👤 You:**
> "Check the credit status for customer account #7890123."

**🤖 AI Agent:**
> Customer #7890123 (María González López): Credit limit: $45,000 MXN. Current balance: $12,350 MXN. Available credit: $32,650 MXN. Weekly payment (abono semanal): $285 MXN. Next payment due: April 15, 2026. Payment streak: 24 consecutive on-time payments. Credit rating: A+ (excellent). She has room for a purchase up to $32,650 MXN.

---

**👤 You:**
> "Show me active Buen Fin promotions."

**🤖 AI Agent:**
> 3 active Buen Fin promotions found: 1. '20% off all Samsung TVs' (Nov 15-18). 2. '18 months interest-free on Whirlpool appliances' (Nov 15-18). 3. 'Buy 2 get 1 free on Nike shoes' (Nov 15-20). All promotions are stackable with the regular weekly credit plans. Want me to search specific products in these categories?


## ❓ FAQ

**Q: Can I check a customer's weekly payment amount and remaining credit balance?**
Yes! Use the `get_customer_credit` tool with the customer's account number. It returns their approved credit limit, current outstanding balance, weekly payment amount (abono semanal), next payment due date, and their on-time payment streak.

**Q: Can I find Coppel stores in a specific Mexican state?**
Absolutely. Use the `list_stores` tool with the state parameter (e.g., 'Jalisco', 'Nuevo León', 'CDMX'). It returns all branches in that state with addresses, phone numbers, operating hours, and available services like BanCoppel banking.

**Q: How do I search for products and see their credit payment plans?**
Use the `search_products` tool with a keyword query. Each result includes the cash price, available weekly payment plan options (abonos), number of installments, and total credit cost. Use `get_product` for the full specification sheet of a specific item.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coppel](https://vinkius.com/mcp/coppel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Coppel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `coppel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Coppel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "coppel": {
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

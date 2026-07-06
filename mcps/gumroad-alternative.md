# Gumroad MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gumroad-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Sell digital products, memberships, and physical goods directly to your audience with a checkout that handles everything.

## Description
Connect your **Gumroad** account to any AI agent and take full control of your digital products and e-commerce workflows through natural conversation.

### What you can do

- **Product Management** — List all your digital products and retrieve detailed metadata, pricing, and shareable URLs programmatically
- **Sales Intelligence** — Monitor transaction history with precise date filters to track revenue and customer acquisition trends
- **Offer Code Automation** — Create and manage discount codes (fixed or percentage-based) to drive marketing campaigns and sales
- **Customer Relationships** — List and manage product-specific subscribers to maintain direct communication with your audience
- **Store Performance** — Retrieve complete transaction details for any sale ID to provide high-fidelity customer support

### How it works

1. Subscribe to this server
2. Retrieve your Application Token from your Gumroad Dashboard (Settings > Advanced > Application tokens)
3. Start managing your creator business from Claude, Cursor, or any MCP client

No more manual status checking or complex store management through different tabs. Your AI acts as your dedicated store manager.

### Who is this for?

- **Digital Creators** — automate discount code generation and monitor sales performance through natural language
- **Customer Success Managers** — quickly retrieve customer transaction data to verify purchases and handle support requests
- **Growth Marketers** — track subscriber lists and campaign performance across multiple products without leaving your workspace


## Available Tools (8)
- **list_offer_codes**: List discount codes for a product
- **list_sales**: Supports date filtering.

List recent sales
- **list_product_subscribers**: List subscribers for a product
- **create_offer_code**: Create a new discount code
- **get_product_details**: Get details for a product
- **get_sale_details**: Get details for a specific sale
- **get_user_profile**: Get your Gumroad account details
- **list_products**: List your Gumroad products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gumroad** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my products on Gumroad."

**🤖 AI Agent:**
> I've retrieved your digital products. You have 5 active items, including 'Advanced AI Guide' ($49.00) and 'MCP Templates' ($19.00). Would you like the shareable URLs for any of these?

---

**👤 You:**
> "Show me the sales from the last 7 days."

**🤖 AI Agent:**
> Scanning transaction history... In the last 7 days, you've had 12 sales totaling $345.00. The best-selling product was 'MCP Templates'. Would you like a breakdown of each transaction?

---

**👤 You:**
> "Create a 20% discount code named 'SUMMER26' for my AI Guide product."

**🤖 AI Agent:**
> Done! I've created the offer code 'SUMMER26' for your 'Advanced AI Guide'. It provides a 20% discount and is ready for use on your checkout page.


## ❓ FAQ

**Q: How do I find my Application Token for Gumroad?**
Log in to your Gumroad account, navigate to **Settings** > **Advanced**, and scroll down to the **Application tokens** section to create a new one.

**Q: Can I create discount codes with my AI agent?**
Yes! The `create_offer_code` tool allows your agent to generate new coupons for any of your products with fixed or percentage discounts.

**Q: Does the integration support checking specific customer info?**
The `get_sale_details` tool provides comprehensive data for any transaction, including the customer's email and purchase metadata.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gumroad-alternative](https://vinkius.com/mcp/gumroad-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gumroad** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gumroad-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gumroad** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gumroad-alternative": {
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

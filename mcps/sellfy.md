# Sellfy MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sellfy)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Open your online store in minutes and sell physical products, digital downloads, subscriptions, and print-on-demand merchandise.

## Description
Connect your **Sellfy** store to any AI agent and take full control of your e-commerce operations through natural conversation. Sellfy is the premier platform for creators to sell digital products, physical goods, and subscriptions, and this integration allows you to orchestrate your entire storefront without leaving your chat interface.

### What you can do

- **Product & Catalog Orchestration** — List all managed products and retrieve detailed pricing metadata, including creating new items programmatically.
- **Order Lifecycle Management** — Access recent store transactions and retrieve detailed fulfillment metadata directly from the AI interface.
- **Customer CRM Control** — Manage your store's customer base and retrieve profile metadata to ensure personalized engagement via natural language.
- **Subscription & Coupon Intelligence** — Monitor recurring billing subscriptions and active discount codes to ensure your revenue streams are always optimized.
- **Operational Monitoring** — Retrieve store metadata and monitor system usage using simple AI commands to ensure your business is always healthy.

### How it works

1. Subscribe to this server
2. Enter your Sellfy API Key from your dashboard settings
3. Start managing your digital storefront from Claude, Cursor, or any MCP-compatible client

No more manual dashboard navigation or spreadsheet order tracking. Your AI acts as a dedicated store manager or operations coordinator.

### Who is this for?

- **Digital Creators** — quickly retrieve sales summaries and monitor subscription growth without switching apps.
- **Store Managers** — automate the management of product metadata and track order fulfillment via natural conversation.
- **Operations Teams** — streamline the retrieval of customer records and monitor organizational health directly within the chat.


## Available Tools
- **create_product**: Requires a title and price.

Create a new product
- **get_customer_details**: Get details for a specific customer
- **get_order_details**: Get details for a specific order
- **get_product_details**: Get details for a specific product
- **get_store_information**: Get high-level store details
- **get_subscription_details**: Get details for a specific subscription
- **list_product_categories**: List product categories
- **list_store_coupons**: List active discount coupons
- **list_customers**: List store customers
- **list_orders**: List recent store orders
- **list_products**: List all store products
- **list_subscriptions**: List recurring subscriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sellfy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all physical products in my Sellfy store."

**🤖 AI Agent:**
> I've retrieved your products. You have 3 physical items including 'Custom T-Shirt' and 'Signed Poster'. Would you like to check the stock levels for any of them?

---

**👤 You:**
> "Show me the sales analytics for all digital products this month with revenue breakdown."

**🤖 AI Agent:**
> Monthly sales analytics. Total revenue: $12,400. Orders: 234. Products sold: 6 categories. "UI Kit Pro" leads with $4,200 (89 sales). "E-book: Design Systems" at $2,800 (140 sales, $19.99 each). "Video Course: React Mastery" at $2,100 (21 sales, $99.99). "Icon Pack Premium" at $1,800 (180 sales, $9.99). "Template Bundle" at $1,100 (22 sales). "Audio Sample Pack" at $400 (40 sales). Average order value: $53. Repeat customers: 34%. Top traffic source: Twitter (42%).

---

**👤 You:**
> "Create a new digital product listing for a premium Figma design template at $49.99."

**🤖 AI Agent:**
> Product created: "Premium Dashboard UI Kit - Figma". Price: $49.99. Category: Digital Download. File uploaded: dashboard_ui_kit_v2.fig (34 MB). Description: 120+ components, dark/light modes, responsive layouts. Product page generated with auto-preview thumbnails. SEO: meta title and description optimized. Payment options: credit card, PayPal. Discount code slot: empty (add anytime). Analytics tracking enabled. Shareable link generated. Estimated based on similar products: 15-20 sales/month.


## ❓ FAQ

**Q: Can my AI automatically find the details and status for a specific order by providing its ID?**
Yes! Use the `get_order` tool with the Order ID. Your agent will respond with complete metadata, including payment status, items purchased, and customer notes in seconds.

**Q: How do I check the current subscription status for a specific customer?**
Simply ask the agent to run the `get_subscription` action with the Subscription ID. It will retrieve the detailed metadata for that recurring billing profile.

**Q: How do I find my Sellfy API Key?**
Log in to your Sellfy dashboard, navigate to **Store Settings** > **Integrations** > **Developer API**, and you will find your unique secret API key there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sellfy](https://vinkius.com/mcp/sellfy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sellfy** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sellfy` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sellfy** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sellfy": {
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

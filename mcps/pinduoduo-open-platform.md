# Pinduoduo Open Platform MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pinduoduo-open-platform)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage Pinduoduo (DDK) affiliate operations — search goods, generate promotion links, and track orders directly from any AI agent.

## Description
Connect your AI agents to the **Pinduoduo Open Platform**, specifically the **Duo Duo Jin Bao (DDK)** affiliate ecosystem. This MCP provides 10 tools to automate product discovery, promotion link generation, and real-time order tracking directly through natural conversation.

### What you can do

- **Product Search** — Search for millions of products on Pinduoduo using keywords, categories, and specific filters
- **Deep Insights** — Retrieve granular product details, including pricing, coupons, and historical sales volume
- **Link Orchestration** — Generate various types of promotion links (short, long, and app-awakening) for affiliate marketing
- **Order Tracking** — Synchronize increment orders and track commission statuses in real-time
- **Market Trends** — Query hot products and top lists to identify trending items across the platform

### How it works

1. Subscribe to this server
2. Log in to the [**Pinduoduo Open Platform**](https://open.pinduoduo.com/)
3. Register as a **DDK Affiliate** and obtain your **Client ID** and **Client Secret**
4. Generate an **Access Token** via the OAuth 2.0 flow
5. Insert your credentials and token into the fields below to start managing your Pinduoduo affiliate backend.

### Who is this for?

- **Affiliate Marketers** — automate the selection of high-commission products and link generation
- **E-commerce Ops** — track real-time order conversions and monitor promotional performance
- **Data Analysts** — retrieve platform-wide top sales data and trending category insights


## Available Tools (10)
- **generate_pid**: Generate unique Promotion IDs (PIDs)
- **generate_promotion_url**: Generate tracking links for a product
- **list_categories**: List product categories
- **get_goods_details**: Get detailed info for a specific product
- **get_order_details**: Get details for a specific promotion order
- **get_recommendations**: Get recommended products from specific channels
- **list_themes**: List marketing themes
- **query_top_goods**: Query real-time ranking of popular products
- **search_goods**: Search for products on Pinduoduo
- **sync_increment_orders**: Retrieve orders based on last update time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pinduoduo Open Platform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search Pinduoduo for 'smart watches' with a minimum commission rate of 20%."

**🤖 AI Agent:**
> I've searched Pinduoduo for smart watches. Here are the top results with at least 20% commission: 1. GT-Pro Smartwatch (Price: 199 CNY, Commission: 25%), 2. Sport Band X (Price: 89 CNY, Commission: 22%)... Would you like me to generate promotion links for these?

---

**👤 You:**
> "Generate a promotion link for product 'p_abc123' using PID 'pid_777'."

**🤖 AI Agent:**
> Generating tracking link... Success! Here is your custom promotion URL for 'Wireless Earbuds': [https://p.pinduoduo.com/abc...]. All sales through this link will be attributed to PID 'pid_777'.

---

**👤 You:**
> "List the top 5 hot products in the 'Electronics' category."

**🤖 AI Agent:**
> Retrieving trending items... I've found the top 5 hot products in Electronics: 1. Tablet Pro Max (ID: t1), 2. Noise Cancelling Headset (ID: t2), 3. Quick Charge Hub (ID: t3)... Would you like the commission details for these?


## ❓ FAQ

**Q: Can my AI automatically generate promotion links for multiple products?**
Yes! Use the `generate_promotion_url` tool with the `goods_sign` of the target product. Your agent can iterate through multiple products to create personalized tracking links in seconds.

**Q: What is a 'goods_sign' and how do I get it?**
The `goods_sign` is a unique identifier for a product on the Pinduoduo platform. You can obtain it by running the `search_goods` or `query_top_goods` tools.

**Q: How do I track commissions for my generated links?**
Use the `sync_increment_orders` tool to retrieve orders associated with your PIDs. It will return the order status and the calculated commission for each successful transaction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pinduoduo-open-platform](https://vinkius.com/mcp/pinduoduo-open-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pinduoduo Open Platform** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pinduoduo-open-platform` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pinduoduo Open Platform** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pinduoduo-open-platform": {
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

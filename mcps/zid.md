# Zid MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zid)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Launch your Arabic e-commerce store with a platform built for Saudi and Gulf markets including local payment and shipping options.

## Description
Connect your **Zid** store to any AI agent and take full control of your e-commerce ecosystem and high-fidelity retail orchestration through natural conversation.

### What you can do

- **Product Portfolio Orchestration** — List all store products, retrieve detailed high-fidelity metadata including variants and attributes, and monitor catalog health programmatically
- **Order Pipeline Intelligence** — Query customer orders, retrieve detailed technical metadata, and stay on top of fulfillment and payment status in real-time
- **Customer Intelligence Architecture** — Access complete high-fidelity customer profiles and purchase history to personalize every interaction directly through your agent
- **Inventory & Stock Monitoring** — Access your complete directory of high-fidelity inventories across multiple locations to optimize stock levels and warehouse operations
- **Shop Profile Discovery** — Access high-fidelity store metadata and operational settings to understand and orchestrate your retail environment programmatically
- **Operational Monitoring** — Verify account-level API connectivity and monitor retail orchestration volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **Manager Token** and **Authorization Token** from your Zid dashboard
3. Start managing your e-commerce growth from Claude, Cursor, or any MCP client

No more manual stock checks or missing order updates. Your AI acts as your dedicated store coordinator and retail architect.

### Who is this for?

- **Store Owners** — instantly retrieve sales analytics and order statuses using natural language commands without leaving your creative workspace
- **Operations Managers** — monitor high-fidelity inventory levels and fulfillment progress to ensure healthy retail operations
- **Customer Support Leads** — verify technical customer profiles and order history to resolve inquiries through simple AI queries


## Available Tools
- **get_zid_customer**: Get customer details
- **get_zid_order**: Get order details
- **get_zid_product**: Get product details
- **list_zid_customers**: List shop customers
- **list_zid_inventories**: List inventories
- **list_zid_orders**: List store orders
- **list_zid_products**: List store products
- **get_zid_shop_profile**: Get shop profile
- **check_zid_status**: Check API Status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zid** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products and show their status."

**🤖 AI Agent:**
> I've retrieved your products. You currently have 12 active high-fidelity profiles, including 'Premium Coffee' (Active) and 'Arabic Dates'. Would you like to see the detailed inventory metadata for any of them?

---

**👤 You:**
> "Show the last 5 orders and their fulfillment status."

**🤖 AI Agent:**
> Retail orchestrated! I've identified 5 recent high-fidelity order profiles, including order #12345 (Ready for Shipping). I've retrieved the technical fulfillment metadata for your review. Shall I summarize the sales progress?

---

**👤 You:**
> "Check the available inventories for the 'Main Warehouse'."

**🤖 AI Agent:**
> Inventory directory orchestrated! Your store currently has 3 high-fidelity inventory locations active. Your API connection is healthy. Shall I retrieve the detailed resource distribution metadata for these sites?


## ❓ FAQ

**Q: How do I find my Zid API Tokens?**
Log in to your Zid Partner dashboard, navigate to your App settings, and locate your unique **X-MANAGER-TOKEN** and **Authorization** Bearer token.

**Q: Can I check product stock levels via AI?**
Yes! The `list_zid_inventories` tool allows your agent to retrieve high-fidelity stock metadata across all defined inventory locations.

**Q: How do I list my shop's orders?**
Use the `list_zid_orders` tool to retrieve the complete high-fidelity directory of customer orders along with their current fulfillment status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zid](https://vinkius.com/mcp/zid)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zid** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `zid` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zid** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zid": {
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

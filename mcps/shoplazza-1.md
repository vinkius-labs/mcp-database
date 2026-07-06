# Shoplazza MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shoplazza-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Launch your cross-border e-commerce store with a platform optimized for global selling, multi-currency, and localized checkout.

## Description
Connect your **Shoplazza** store to any AI agent and take full control of your e-commerce operations and high-fidelity retail orchestration through natural conversation.

### What you can do

- **Product Portfolio Orchestration** — List all store products, retrieve detailed high-fidelity metadata including variants and inventory, and monitor stock levels programmatically
- **Order Pipeline Intelligence** — Query customer orders, retrieve detailed technical metadata, and stay on top of fulfillment status in real-time
- **Customer Intelligence Architecture** — Access complete high-fidelity customer profiles and purchase history to personalize every interaction directly through your agent
- **Collection & Category Monitoring** — Access your complete directory of high-fidelity product collections to understand and orchestrate your store's merchandising structure
- **Store Metadata Discovery** — Access high-fidelity shop profiles and configuration settings to understand and orchestrate your environment programmatically
- **Operational Monitoring** — Verify account-level API connectivity and monitor retail orchestration volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **Access Token** and **Shop Domain** from your Shoplazza dashboard (Settings > API)
3. Start managing your e-commerce growth from Claude, Cursor, or any MCP client

No more manual stock checks or missing order updates. Your AI acts as your dedicated store coordinator and retail architect.

### Who is this for?

- **Store Owners** — instantly retrieve product details and order statuses using natural language commands without leaving your creative workspace
- **Operations Managers** — monitor high-fidelity fulfillment progress and customer trends to ensure healthy retail operations
- **Marketing Teams** — analyze technical customer segments and collection performance to optimize campaigns through simple AI queries


## Available Tools (11)
- **get_shoplazza_order**: Get order details
- **get_shoplazza_product**: Get product details
- **get_shoplazza_shop**: Get shop metadata
- **list_shoplazza_collections**: List product collections
- **list_shoplazza_customers**: List shop customers
- **list_shoplazza_orders**: List store orders
- **list_shoplazza_products**: List store products
- **check_shoplazza_status**: Check API Status
- **create_shoplazza_customer**: Create a new customer
- **create_shoplazza_product**: Create a new product
- **get_shoplazza_customer**: Get customer details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Shoplazza** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all products and show their current price."

**🤖 AI Agent:**
> I've retrieved your products. You currently have 15 active high-fidelity profiles, including 'Classic T-Shirt' ($25) and 'Denim Jacket' ($85). Would you like to see the detailed inventory metadata for any of them?

---

**👤 You:**
> "Show the last 5 orders and their fulfillment status."

**🤖 AI Agent:**
> Retail orchestrated! I've identified 5 recent high-fidelity order profiles, including order #1001 (Fulfilled) and #1002 (Processing). I've retrieved the technical fulfillment metadata for your review. Shall I summarize the sales progress?

---

**👤 You:**
> "Check the available collections for the 'Summer' promotion."

**🤖 AI Agent:**
> Collection directory orchestrated! Your store currently has 5 high-fidelity promotion profiles active, including 'Summer Sale' and 'New Arrivals'. Your API connection is healthy. Shall I retrieve the detailed product orchestration metadata for these collections?


## ❓ FAQ

**Q: How do I find my Shoplazza Access Token?**
Log in to your account, navigate to **Settings** > **API Settings**, and create a new high-fidelity **Private App** to obtain your Access Token.

**Q: Can I check product inventory via AI?**
Yes! The `get_shoplazza_product` tool allows your agent to retrieve high-fidelity inventory metadata for all product variants and stock locations.

**Q: How do I list my shop's customers?**
Use the `list_shoplazza_customers` tool to retrieve the complete high-fidelity directory of customer profiles along with their unique identifiers for precise orchestration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shoplazza-1](https://vinkius.com/mcp/shoplazza-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Shoplazza** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shoplazza-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Shoplazza** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shoplazza-1": {
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

# JVZoo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/jvzoo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage products, sales, and affiliates via JVZoo API.

## Description
Empower your AI agents with JVZoo's digital commerce platform. This MCP server allows you to list and retrieve product details, track sales transactions, manage affiliates, and view account information directly through the JVZoo API. Ideal for automating marketing operations and sales tracking.


## Available Tools (10)
- **get_account**: Use to verify connection status and account identity.

Retrieves details about your JVZoo account
- **get_affiliate**: Essential for partner vetting and relationship management.

Retrieves details for a specific affiliate
- **get_product**: Returns descriptions, sales status, and technical settings. Use this when the user needs to analyze a specific listing.

Retrieves details for a specific product
- **get_sale**: Returns customer details, product purchased, and payment status. Use this for order verification or support.

Retrieves details for a specific sale
- **list_affiliates**: Use this to monitor your affiliate network and identify top partners.

Lists all approved affiliates
- **list_campaigns**: Useful for tracking promotional efforts and campaign IDs.

Lists all active affiliate campaigns
- **list_coupons**: Useful for auditing available incentives.

Lists all active discount coupons
- **list_products**: Returns product names, IDs, and pricing. Use this to identify specific items for sales analysis or affiliate management.

Lists all products in your JVZoo account
- **list_sales**: Includes transaction IDs, amounts, and timestamps. Essential for monitoring revenue and recent customer purchases.

Lists all sales transactions
- **list_webhooks**: Useful for auditing automated integrations.

Lists all configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JVZoo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my products on JVZoo."

**🤖 AI Agent:**
> I'll fetch the list of products you have listed in your JVZoo account.

---

**👤 You:**
> "Show me the last 10 sales transactions."

**🤖 AI Agent:**
> I'll retrieve your recent sales history from JVZoo for you.

---

**👤 You:**
> "Check the performance of affiliate ID '123'."

**🤖 AI Agent:**
> I'll look up the profile and activity for that specific affiliate in JVZoo.


## ❓ FAQ

**Q: How do I get JVZoo API credentials?**
Log in to your JVZoo account, navigate to My Account > Applications, and find your API Key.

**Q: Can I see sales in real-time?**
Yes, the list_sales tool provides access to your recent transaction history recorded in JVZoo.

**Q: Does it support affiliate management?**
Yes, you can list approved affiliates and retrieve details for specific partners using this MCP.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/jvzoo](https://vinkius.com/mcp/jvzoo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JVZoo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `jvzoo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JVZoo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "jvzoo": {
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

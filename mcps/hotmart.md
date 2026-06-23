# Hotmart MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hotmart)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Manage sales, products, and subscriptions via Hotmart API.

## Description
Empower your AI agents to manage your digital products business on Hotmart. This MCP server provides tools to list products, track sales history, manage subscriptions, view commissions, and monitor affiliates directly through the Hotmart API. Perfect for automating creator workflows.


## Available Tools (10)
- **get_me**: Gets current authenticated user info
- **get_sale_by_user**: Finds sales associated with a specific user email
- **get_sales_report**: Retrieves a sales report
- **list_affiliates**: Lists affiliates for your products
- **list_commissions**: Lists commissions for sales
- **list_payments**: Lists payments received
- **list_products**: Lists products in your Hotmart account
- **list_sales_history**: Lists sales history
- **list_subscriptions**: Lists product subscriptions
- **list_webhooks**: Lists configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hotmart** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the last 10 sales in my Hotmart account."

**🤖 AI Agent:**
> I've pulled the recent sales data. Over the last 10 transactions, you've accumulated $425.50 in net commissions. Your top-selling product was 'Advanced AI Prompting Course' with 6 conversions this week alone.

---

**👤 You:**
> "List all my products on Hotmart."

**🤖 AI Agent:**
> You have 3 active digital products registered: 1. 'Masterclass SEO' (ID: 99120), 2. 'Email Templates' (ID: 99144), 3. 'Consulting Calls' (ID: 99201). Let me know if you would like me to list their individual conversion rates.

---

**👤 You:**
> "Check for active subscriptions."

**🤖 AI Agent:**
> Scanning subscriptions... You currently stand at 145 active recurring subscribers, generating approximately $2,900 MRR. There were 2 new signups today and 1 cancellation.


## ❓ FAQ

**Q: How do I get my Hotmart API credentials?**
You can find your Client ID and Client Secret in the Hotmart Developers platform under 'Credentials'.

**Q: Can I track affiliate sales?**
Yes, the list_affiliates and list_sales_history tools allow you to monitor affiliate performance.

**Q: Is the sales report real-time?**
Yes, all data is retrieved directly from Hotmart's servers in real-time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hotmart](https://vinkius.com/mcp/hotmart)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hotmart** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `hotmart` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hotmart** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hotmart": {
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

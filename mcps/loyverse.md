# Loyverse MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/loyverse)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Free POS and inventory management system.

## Description
The Loyverse MCP Server allows you to seamlessly integrate your point-of-sale system with any AI agent. Manage your inventory, track sales data, and create customer profiles programmatically through natural language.

### What you can do

- **Track Sales** — Retrieve aggregated sales metrics, receipts, and performance data dynamically
- **Inventory Management** — Check stock levels and list items across multiple locations
- **Customer Data** — Search and list your registered customers in the system
- **Locations** — Retrieve store location details and coordinate operations across branches

### How it works

1. Subscribe to this server
2. Open your Loyverse Back Office and generate an Access Token
3. Start managing your store operations from any MCP-compatible client or AI agent

### Who is this for?

- **Store Managers** — quickly check inventory levels without opening the dashboard
- **Retail Owners** — pull daily sales numbers via chat
- **Customer Service** — look up customer history automatically


## Available Tools
- **l_list_customers**: List your registered store customers from Loyverse POS
- **l_list_items**: List inventory items in your Loyverse account with optional pagination parameters
- **l_list_locations**: List all store locations in your Loyverse account
- **l_list_receipts**: Can filter by creation date min and max parameters.

List generated receipts from your Loyverse POS system. Can be filtered by date range and pagination limit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Loyverse** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Fetch the total sales numbers for all locations yesterday."

**🤖 AI Agent:**
> Retrieved yesterday's sales figures: A total of $4,532.10 across 3 stores with 120 individual receipts.

---

**👤 You:**
> "Check the current inventory level for the item 'Honduras Dark Roast Coffee' at the Main Street location."

**🤖 AI Agent:**
> The item 'Honduras Dark Roast Coffee' has 45 units in stock at the Main Street location. The low stock alert threshold is 10 units.

---

**👤 You:**
> "Create a new customer profile for John Doe with the email john@example.com."

**🤖 AI Agent:**
> Customer profile for 'John Doe' (john@example.com) has been successfully created and linked to your customer database.


## ❓ FAQ

**Q: How do I get my Loyverse API token?**
Log in to your Loyverse Back Office. Navigate to the Integrations section, specifically 'Access Tokens'. Here, you can generate a new personal access token specifically for this AI integration.

**Q: Can I query daily sales reports?**
Yes, you can use the `l_list_receipts` tool to retrieve sales data and individual receipts over any date range, and the AI agent can aggregate these into daily sales reports for you.

**Q: Does the API support checking inventory?**
Absolutely. You can use the `l_list_items` tool to dynamically track item catalog details and stock presence across your system.

**Q: Can I see all my registered customers?**
Yes. The `l_list_customers` tool lets the agent fetch your entire customer database, including their names, registration dates, and generated identifiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/loyverse](https://vinkius.com/mcp/loyverse)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Loyverse** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `loyverse` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Loyverse** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "loyverse": {
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

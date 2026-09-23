# Menu Item Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/menu-item-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-aggregation](../categories/data-aggregation.md)

Aggregate and count unique menu items across restaurant categories.

## Description
This MCP server provides tools to manage and audit restaurant menus. Use `get_category_list` to discover available categories, `get_item_count_by_category` to check specific counts, `get_total_count_for_selection` to sum items across multiple groups, and `verify_category_integrity` to identify empty or invalid categories.


## Available Tools (4)
- **get_category_list**: Get a list of all available menu categories for a restaurant
- **get_item_count_by_category**: Get the number of items in a specific menu category
- **get_total_count_for_selection**: Get the total number of items across multiple categories
- **verify_category_integrity**: Verify the integrity of menu categories


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Menu Item Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What categories are available for restaurant ID 'rest_123'?"

**🤖 AI Agent:**
> The available categories for restaurant 'rest_123' are Appetizers, Main Courses, Desserts, and Beverages.

---

**👤 You:**
> "How many items are in the 'Desserts' category for restaurant 'rest_123'?"

**🤖 AI Agent:**
> There are 12 items in the Desserts category.

---

**👤 You:**
> "What is the total number of items in 'Appetizers' and 'Main Courses' for restaurant 'rest_123'?"

**🤖 AI Agent:**
> The total number of items across Appetizers and Main Courses is 45.


## ❓ FAQ

**Q: How do I see all available categories?**
You can use the `get_category_list` tool to retrieve a full list of valid category IDs for a specific restaurant.

**Q: Can I sum items from multiple categories at once?**
Yes, the `get_total_count_for_selection` tool allows you to provide a list of category IDs to get an additive total count.

**Q: How can I check for empty categories?**
Use the `verify_category_integrity` tool to generate a report that identifies categories with zero items.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/menu-item-counter](https://vinkius.com/en/ai-agent-connect/menu-item-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Menu Item Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `menu-item-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Menu Item Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "menu-item-counter": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Home Inventory Replacement Value MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/home-inventory-replacement-value)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate replacement costs and insurance coverage adequacy for household assets.

## Description
This MCP server provides specialized tools to assess the financial exposure of a home inventory. It calculates the total replacement value of all household assets and identifies if specific categories exceed their insurance coverage limits. Use `calculate_inventory_totals` to get a full financial summary, `identify_high_value_items` to flag expensive assets, or `validate_category_coverage` to check for under-insured categories.


## Available Tools (4)
- **calculate_inventory_totals**: Calculates overall financial exposure
- **get_inventory_by_category**: Retrieves items in a category
- **identify_high_value_items**: Filters for high value items
- **validate_category_coverage**: Checks if a category is under-insured


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Home Inventory Replacement Value** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total inventory value and check for over-limit categories using these items: [{'itemId': '1', 'quantity': 2, 'unitReplacementPrice': 500, 'categoryId': 'electronics'}] and these limits: [{'categoryId': 'electronics', 'maxCoverageAmount': 800}]"

**🤖 AI Agent:**
> The total inventory value is $1,000. The 'electronics' category is over its limit by $200.

---

**👤 You:**
> "Find all items worth more than $1,000 in this list: [{'itemId': 'A', 'quantity': 1, 'unitReplacementPrice': 1500, 'categoryId': 'jewelry'}, {'itemId': 'B', 'quantity': 1, 'unitReplacementPrice': 200, 'categoryId': 'furniture'}]"

**🤖 AI Agent:**
> The high-value item found is item 'A' with a replacement value of $1,500.

---

**👤 You:**
> "Is the 'furniture' category under-insured if the limit is $500 and the items are [{'itemId': 'F1', 'quantity': 1, 'unitReplacementPrice': 600, 'categoryId': 'furniture'}]?"

**🤖 AI Agent:**
> Yes, the 'furniture' category is under-insured. The current total is $600, which exceeds the $500 limit by $100.


## ❓ FAQ

**Q: How is replacement value calculated?**
Replacement value is calculated as the quantity of an item multiplied by its current market replacement price, ignoring historical purchase costs.

**Q: Can I check if my jewelry is under-insured?**
Yes, you can use `validate_category_coverage` to compare the total value of items in a specific category against a defined limit.

**Q: How do I find my most expensive items?**
You can use the `identify_high_value_items` tool by providing a minimum threshold value.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/home-inventory-replacement-value](https://vinkius.com/en/ai-agent-connect/home-inventory-replacement-value)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Home Inventory Replacement Value** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `home-inventory-replacement-value` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Home Inventory Replacement Value** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "home-inventory-replacement-value": {
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

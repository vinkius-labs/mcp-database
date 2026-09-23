# Cafe Daily Sales Tracker MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cafe-daily-sales-tracker)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Record and analyze daily cafe revenue and sales volume.

## Description
This MCP server connects AI agents to cafe transaction data. Use `record_sale` to log new food and drink transactions, `get_daily_summary` to view total revenue and item counts, `get_top_selling_items` to identify popular products, and `get_category_split` to analyze the revenue ratio between food and drinks.


## Available Tools (4)
- **get_daily_summary**: Retrieves the total revenue and total number of items sold for a specific day
- **get_category_split**: Analyzes the ratio of food sales to drink sales for a given day
- **get_top_selling_items**: You can optionally specify a limit for the number of top items.

Identifies which items were most popular on a specific date
- **record_sale**: Ensure the date is in YYYY-MM-DD format and the category is either "Drink" or "Food".

Records a single successful sale of a food or drink item


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cafe Daily Sales Tracker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Record a sale for a Latte costing 4.50 on 2023-10-01."

**🤖 AI Agent:**
> The sale for the Latte has been recorded successfully.

---

**👤 You:**
> "What was the total revenue for 2023-10-01?"

**🤖 AI Agent:**
> The total revenue for 2023-10-01 was 150.00 with 25 items sold.

---

**👤 You:**
> "Show me the top 3 items sold on 2023-10-01."

**🤖 AI Agent:**
> The top items were: Croissant (10), Latte (8), and Muffin (5).


## ❓ FAQ

**Q: How do I record a new sale?**
Use the `record_sale` tool with the date, category (Drink or Food), item name, and the amount.

**Q: Can I see which items sold the most?**
Yes, you can use `get_top_selling_items` to see a ranked list of products for a specific date.

**Q: How is the revenue split calculated?**
The `get_category_split` tool calculates the percentage of total revenue contributed by food versus drinks.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cafe-daily-sales-tracker](https://vinkius.com/en/ai-agent-connect/cafe-daily-sales-tracker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cafe Daily Sales Tracker** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cafe-daily-sales-tracker` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cafe Daily Sales Tracker** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cafe-daily-sales-tracker": {
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

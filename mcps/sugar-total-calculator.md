# Sugar Total Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sugar-total-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Track and aggregate sugar content from food and drink items.

## Description
This MCP server provides tools to monitor dietary sugar intake. You can use `add_food_item` to log new entries, `list_sugar_items` to view your current list, `remove_food_item` to delete entries, and `calculate_totals` to get the aggregate sugar sum and average per item.


## Available Tools (4)
- **add_food_item**: Adds a new food or drink entry with a specified sugar amount to the session
- **calculate_totals**: Computes the sum of all sugar and the average sugar per item for a given session
- **list_sugar_items**: Retrieves the current list of food and drink items being tracked in the session
- **remove_food_item**: Removes a specific item from the tracking session


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sugar Total Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add an apple with 10 grams of sugar to my session 'session-123'."

**🤖 AI Agent:**
> Added apple with 10 grams of sugar to session session-123.

---

**👤 You:**
> "What is my total sugar for session 'session-123'?"

**🤖 AI Agent:**
> The total sugar for session session-123 is 10 grams, with an average of 10 grams per item.

---

**👤 You:**
> "List all items in session 'session-123'."

**🤖 AI Agent:**
> The items in session session-123 are: apple (10g).


## ❓ FAQ

**Q: How do I add a new item?**
Use the `add_food_item` tool by providing the session ID, the name of the food, and the sugar amount in grams.

**Q: How can I see my total sugar intake?**
You can use the `calculate_totals` tool to retrieve the total sugar and the average sugar per item for your session.

**Q: Can I remove an item I added by mistake?**
Yes, use the `remove_food_item` tool with the exact name of the item to remove it from your session.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sugar-total-calculator](https://vinkius.com/en/ai-agent-connect/sugar-total-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sugar Total Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sugar-total-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sugar Total Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sugar-total-calculator": {
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

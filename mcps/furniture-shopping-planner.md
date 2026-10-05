# Furniture Shopping Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/furniture-shopping-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [shopping](../categories/shopping.md)

Select optimal furniture based on room dimensions, budget, and logistics.

## Description
This MCP server helps users make informed furniture purchases by evaluating spatial constraints, budgetary limits, and logistical needs. It provides tools to check if items fit in a room using `get_room_capacity`, verify affordability with `filter_by_budget`, and assess delivery or assembly requirements via `evaluate_logistics`. It also calculates item value through `calculate_utility_score` and can suggest the best options using `get_recommended_items`.


## Available Tools (5)
- **evaluate_logistics**: Determines if the delivery and assembly requirements align with user preferences
- **filter_by_budget**: Identifies if a furniture item is affordable within a specific spending limit
- **get_recommended_items**: Suggests a list of items that satisfy all constraints (space, budget, and logistics)
- **get_room_capacity**: Evaluates if a specific piece of furniture can physically fit within a designated room
- **calculate_utility_score**: Provides a weighted rating of how much value a piece of furniture adds


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Furniture Shopping Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a room that is 5m x 4m x 3m. Will a bed that is 2m x 2m x 0.5m fit if I need 1m of clearance around it?"

**🤖 AI Agent:**
> Yes, the bed fits within the room dimensions while maintaining the required clearance.

---

**👤 You:**
> "I have $500. Is a $450 dining table affordable?"

**🤖 AI Agent:**
> Yes, the dining table is affordable, leaving you with $50 remaining.

---

**👤 You:**
> "Can you recommend furniture for a 4x4x3 room with a $1000 budget and 7 days max delivery?"

**🤖 AI Agent:**
> Based on your constraints, I recommend the compact armchair and the modular side table.


## ❓ FAQ

**Q: How do I know if a sofa will fit in my living room?**
You can use the `get_room_capacity` tool by providing your room dimensions and the sofa's dimensions to confirm it fits with necessary clearance.

**Q: Can I check if an item is within my budget?**
Yes, the `filter_by_budget` tool allows you to compare an item's price against your available funds.

**Q: Does the tool consider assembly needs?**
Yes, `evaluate_logistics` checks if the delivery timing and assembly requirements match your preferences.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/furniture-shopping-planner](https://vinkius.com/en/ai-agent-connect/furniture-shopping-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Furniture Shopping Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `furniture-shopping-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Furniture Shopping Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "furniture-shopping-planner": {
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

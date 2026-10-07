# Packing List Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/packing-list-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate precise travel packing lists based on trip duration, weather, and activities.

## Description
This MCP server acts as a smart travel assistant that calculates exactly what you need to pack. By synthesizing trip duration, laundry availability, and weather profiles, it determines clothing needs using `calculate_clothing_requirements`. It can also add specialized gear for specific events via `add_activity_gear`, subtract items you already own with `apply_inventory_deductions`, and ensure everything fits in your suitcase using `validate_luggage_capacity`.


## Available Tools (4)
- **add_activity_gear**: Adds specialized equipment required for specific scheduled events
- **apply_inventory_deductions**: Adjusts the required quantities by subtracting items the user already possesses
- **calculate_clothing_requirements**: Determines the number of essential clothing items needed based on trip length and logistics
- **validate_luggage_capacity**: Checks if the final packing list fits within the user's physical luggage constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Packing List Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I'm going on a 7-day trip to a cold climate and I'll have access to laundry every 3 days. How many clothes should I pack?"

**🤖 AI Agent:**
> For a 7-day trip in cold weather with laundry every 3 days, you will need 5 base layers, 3 heavy sweaters, and 2 heavy jackets.

---

**👤 You:**
> "I am planning a trip that includes swimming and hiking. What gear do I need?"

**🤖 AI Agent:**
> You will need to pack swimwear, a towel, hiking boots, and moisture-wicking socks.

---

**👤 You:**
> "My luggage limit is 20kg. Will these items fit: 5 shirts (1kg each) and 2 jackets (3kg each)?"

**🤖 AI Agent:**
> Yes, the total weight is 11kg, which is well within your 20kg limit.


## ❓ FAQ

**Q: How does the tool handle weather changes?**
The `calculate_clothing_requirements` tool adjusts the quantity and type of clothing layers based on the weather profile you provide, such as cold or hot.

**Q: Can I account for items I already own?**
Yes, you can use `apply_inventory_deductions` to subtract items from your required list that you already have in your possession.

**Q: How do I know if my luggage is too heavy?**
You can use `validate_luggage_capacity` to check if your final list of items stays within your specified weight and volume limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/packing-list-builder](https://vinkius.com/en/ai-agent-connect/packing-list-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Packing List Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `packing-list-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Packing List Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "packing-list-builder": {
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

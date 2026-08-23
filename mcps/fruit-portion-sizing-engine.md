# Fruit Portion Sizing Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/fruit-portion-sizing-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate exact fruit portions to hit a 15g carbohydrate target.

## Description
This MCP server provides precise nutritional calculations for diabetic-standard servings. By using the `get_carb_portion_details` tool, you can determine the exact mass and volume of a fruit needed to reach exactly 15g of carbohydrates. It also allows you to use `get_available_fruits` to see supported options and `get_nutritional_profile_comparison` to compare the sugar and fiber ratios between different fruits at the same carbohydrate level.


## Available Tools (3)
- **get_available_fruits**: Lists all fruits supported by the engine
- **get_carb_portion_details**: Calculates the exact mass, volume, sugar, and fiber content required to hit the 15g carbohydrate target for a specific fruit
- **get_nutritional_profile_comparison**: Compares the sugar and fiber ratios of two different fruits when both are scaled to the 15g carbohydrate standard


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fruit Portion Sizing Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many grams of strawberries do I need for 15g of carbs?"

**🤖 AI Agent:**
> You need 150g of strawberries to reach 15g of carbohydrates.

---

**👤 You:**
> "What is the volume equivalent for 80g of banana?"

**🤖 AI Agent:**
> 80g of banana is approximately half a medium banana.

---

**👤 You:**
> "Compare the sugar and fiber in an apple versus a banana for a 15g carb serving."

**🤖 AI Agent:**
> An apple provides more fiber, while a banana provides a different sugar profile, both at the 15g carbohydrate standard.


## ❓ FAQ

**Q: What is a standard diabetic serving?**
A standard diabetic serving is defined as exactly 15 grams of total carbohydrates.

**Q: How do I know which fruits are supported?**
You can use the `get_available_fruits` tool to see a complete list of all fruits currently supported by the engine.

**Q: Can I compare the nutritional value of two fruits?**
Yes, use the `get_nutritional_profile_comparison` tool to compare the sugar and fiber deltas between two fruits, both scaled to 15g of carbohydrates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/fruit-portion-sizing-engine](https://vinkius.com/ai-agent-connect/fruit-portion-sizing-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fruit Portion Sizing Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fruit-portion-sizing-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fruit Portion Sizing Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fruit-portion-sizing-engine": {
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

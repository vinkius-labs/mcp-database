# Capsule Wardrobe Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/capsule-wardrobe-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

A deterministic engine to build optimal capsule wardrobes based on climate, season, and style rules.

## Description
This MCP server provides a suite of tools to optimize wardrobe selection. Use `plan_capsule` to generate a high-utility wardrobe within a specific piece limit, or `validate_outfit` to check if a combination of garments meets temperature and occasion requirements. You can also use `get_garment_versatility` to score individual items or `analyze_wardrobe_coverage` to see how well your selection covers various climate scenarios and occasions.


## Available Tools (4)
- **analyze_wardrobe_coverage**: Provides a detailed report on which occasions and climate scenarios the current capsule satisfies
- **get_garment_versatility**: Calculates a score for a garment indicating how many different types of outfits it can participate in
- **plan_capsule**: Generates the optimal capsule wardrobe based on user constraints and available garments
- **validate_outfit**: Checks if a specific combination of items constitutes a legal outfit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Capsule Wardrobe Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Help me plan a 10-item capsule wardrobe for a summer trip to Italy with a temperature range of 25-35 degrees."

**🤖 AI Agent:**
> I have generated a 10-item capsule wardrobe optimized for summer in Italy. It includes 4 tops, 3 bottoms, 2 pairs of footwear, and 1 accessory, providing 12 unique outfit combinations that cover Casual and Professional occasions.

---

**👤 You:**
> "Is this outfit valid for a formal dinner at 20 degrees Celsius: a black dress and heels?"

**🤖 AI Agent:**
> Yes, the black dress and heels combination is a valid outfit for a formal occasion at 20 degrees Celsius.

---

**👤 You:**
> "Which of these items is the most versatile for my current wardrobe?"

**🤖 AI Agent:**
> The white linen shirt has the highest versatility score, as it can participate in 8 different outfit combinations across various occasions.


## ❓ FAQ

**Q: How does the engine decide which clothes to pick?**
The engine uses a deterministic optimization process to maximize the total number of valid outfit combinations within your specified piece limit.

**Q: Can I check if an outfit is suitable for a specific temperature?**
Yes, you can use the `validate_outfit` tool to verify if a set of garments is appropriate for a given temperature and occasion.

**Q: What happens if two different sets of clothes provide the same number of outfits?**
The engine uses a stable tie-break rule based on the lexicographical sum of item IDs to ensure the selection is always consistent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/capsule-wardrobe-planner](https://vinkius.com/en/ai-agent-connect/capsule-wardrobe-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Capsule Wardrobe Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `capsule-wardrobe-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Capsule Wardrobe Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "capsule-wardrobe-planner": {
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

# Caffeine Total Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/caffeine-total-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Calculate total caffeine intake and the percentage contribution of each drink.

## Description
This MCP server provides tools to aggregate caffeine content from various beverages. Use `calculate_total_intake` to find the cumulative caffeine and volume from multiple servings, `get_caffeine_distribution` to see the percentage contribution of each drink, and `validate_daily_limit` to check safety thresholds for different user profiles.


## Available Tools (4)
- **calculate_total_intake**: 
- **get_caffeine_distribution**: 
- **get_drink_caffeine_info**: 
- **validate_daily_limit**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Caffeine Total Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total caffeine from 2 Espressos and 1 Black Coffee?"

**🤖 AI Agent:**
> The total caffeine intake is 190mg from a total volume of 180ml.

---

**👤 You:**
> "Is 400mg of caffeine safe for an adult?"

**🤖 AI Agent:**
> No, 400mg exceeds the standard limit for an adult. The limit is 400mg, and you have reached it.

---

**👤 You:**
> "What percentage of my caffeine comes from 3 servings of Energy Drink?"

**🤖 AI Agent:**
> The Energy Drink accounts for 75% of your total caffeine intake.


## ❓ FAQ

**Q: How do I calculate my total caffeine intake?**
You can use the `calculate_total_intake` tool by providing a list of drinks and their number of servings.

**Q: Can I check if my caffeine intake is safe?**
Yes, use the `validate_daily_limit` tool with your total caffeine amount and your user profile to check against safety thresholds.

**Q: How can I see which drink contributed most to my caffeine level?**
Use the `get_caffeine_distribution` tool to see the percentage of total caffeine for each beverage.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/caffeine-total-calculator](https://vinkius.com/en/ai-agent-connect/caffeine-total-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Caffeine Total Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `caffeine-total-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Caffeine Total Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "caffeine-total-calculator": {
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

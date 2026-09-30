# Baby Shower Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/baby-shower-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Automated logistics planning for baby showers including food, decor, and timelines.

## Description
This MCP server provides a complete planning engine for baby showers. It uses guest counts to scale catering, decorations, and favors. Use `generate_event_blueprint` to create a master plan, `calculate_catering_requirements` for food quantities, `plan_entertainment_and_games` for activities, `generate_decor_and_favor_list` for aesthetics, and `construct_event_timeline` to schedule the event.


## Available Tools (5)
- **calculate_catering_requirements**: Provides a detailed breakdown of food and drink quantities needed
- **generate_decor_and_favor_list**: Lists the necessary decorations and guest favors
- **construct_event_timeline**: Generates a chronological schedule for the event
- **generate_event_blueprint**: Creates the complete master plan for the baby shower
- **plan_entertainment_and_games**: Suggests a selection of games and activities


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Baby Shower Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Plan a baby shower for 20 guests with a budget of $500 and a Boho theme."

**🤖 AI Agent:**
> I have generated your Boho-themed baby shower blueprint for 20 guests. Your budget is allocated with $250 for food, $100 for decor, $50 for favors, $50 for games, and $50 for gifts. The plan includes a list of finger foods, boho decorations, and a 3-hour timeline.

---

**👤 You:**
> "How much food do I need for a tea party with 15 guests?"

**🤖 AI Agent:**
> For a tea party with 15 guests, you will need approximately 45 finger sandwiches, 30 mini scones, and 15 servings of assorted pastries.

---

**👤 You:**
> "Create a timeline for a 2-hour event with Arrival, Food, and Games."

**🤖 AI Agent:**
> Your 2-hour schedule is: 0:00-0:30 Arrival, 0:30-1:15 Food, and 1:15-2:00 Games.


## ❓ FAQ

**Q: How do I create a full event plan?**
You can use the `generate_event_blueprint` tool to create a comprehensive plan covering budget, food, decor, and a timeline based on your guest count.

**Q: Can I plan specific catering needs?**
Yes, the `calculate_catering_requirements` tool provides detailed food and drink quantities based on your guest count and chosen event style.

**Q: How are decorations and favors handled?**
The `generate_decor_and_favor_list` tool calculates the necessary items and scales favors to match your guest count.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/baby-shower-planner](https://vinkius.com/en/ai-agent-connect/baby-shower-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Baby Shower Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `baby-shower-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Baby Shower Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "baby-shower-planner": {
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

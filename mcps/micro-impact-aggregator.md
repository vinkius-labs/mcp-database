# Micro Impact Aggregator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/micro-impact-aggregator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sustainability](../categories/sustainability.md)

Track daily sustainable actions and convert them into measurable environmental impact and financial savings.

## Description
The Micro Impact Aggregator transforms small, repeatable sustainable habits--like using a reusable cup or choosing meatless meals--into tangible metrics. By utilizing tools like `calculate_period_impact`, users can see the total water saved, plastic avoided, and CO2 reduced over any period. The server also tracks progress through `get_achievement_progress` to identify streaks and milestones, and uses `map_impact_to_analogies` to translate abstract numbers into relatable comparisons like 'enough water to fill 10 bathtubs'.


## Available Tools (3)
- **map_impact_to_analogies**: Converts metrics to relatable analogies
- **calculate_period_impact**: Calculates total environmental and financial savings for a period
- **get_achievement_progress**: Evaluates user engagement via streaks and milestones


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Micro Impact Aggregator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What was my total impact from using reusable bags and cups last week?"

**🤖 AI Agent:**
> Last week, you avoided 50g of plastic and saved 20 liters of water by using reusable items.

---

**👤 You:**
> "Convert 500 liters of water savings into a relatable analogy."

**🤖 AI Agent:**
> You saved enough water to fill approximately 2.5 standard bathtubs.

---

**👤 You:**
> "Check my current sustainability streak for meatless meals."

**🤖 AI Agent:**
> You are currently on a 5-day streak of meatless meals!


## ❓ FAQ

**Q: How can I see my total savings for the last month?**
You can use the `calculate_period_impact` tool by providing your action logs from the past 30 days.

**Q: Does this track financial benefits?**
Yes, it calculates the money saved by choosing sustainable alternatives over single-use options.

**Q: How are milestones calculated?**
The `get_achievement_progress` tool analyzes your cumulative environmental savings against predefined achievement tiers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/micro-impact-aggregator](https://vinkius.com/mcp/micro-impact-aggregator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Micro Impact Aggregator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `micro-impact-aggregator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Micro Impact Aggregator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "micro-impact-aggregator": {
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

# Active Minutes Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/active-minutes-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Convert physical activities into metabolic active minutes and track health progress.

## Description
This MCP server connects AI agents to a metabolic activity engine. It uses MET-based classification to convert any physical activity into active minutes, providing a clear breakdown of moderate and vigorous intensity. Users can use `search_activity_catalog` to find valid activities, `calculate_activity_impact` to determine calories burned and active minutes, `get_weekly_progress` to track health goals, and `get_user_metabolic_profile` to adjust intensity thresholds based on age.


## Available Tools (4)
- **calculate_activity_impact**: Calculates the specific impact of a single activity session on a user's health metrics
- **get_user_metabolic_profile**: Provides context for how activity intensity should be interpreted for a specific age group
- **get_weekly_progress**: Checks how much of the weekly health guideline has been met based on accumulated activity
- **search_activity_catalog**: Allows the user to find valid activity types to ensure they provide correct inputs to other tools


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Active Minutes Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I just did 30 minutes of running. How many calories did I burn and what is my active minute impact?"

**🤖 AI Agent:**
> For 30 minutes of running at your weight, you burned 300 calories and earned 45 active minutes.

---

**👤 You:**
> "What activities are available in the catalog for strength training?"

**🤖 AI Agent:**
> Available strength training activities include weightlifting, resistance bands, and bodyweight exercises.

---

**👤 You:**
> "How much progress have I made this week if I have 150 moderate minutes and 60 vigorous minutes?"

**🤖 AI Agent:**
> You have reached 85% of your weekly health goal.


## ❓ FAQ

**Q: How are active minutes calculated?**
Active minutes are calculated by weighting the duration of an activity based on its MET (Metabolic Equivalent of Task) value, distinguishing between moderate and vigorous intensity.

**Q: Can I find specific exercises in the tool?**
Yes, you can use `search_activity_catalog` to find supported activities and their corresponding MET values.

**Q: Does age affect the results?**
Yes, `get_user_metabolic_profile` provides age-based adjustments to ensure intensity thresholds align with metabolic guidelines for your age group.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/active-minutes-calculator](https://vinkius.com/en/ai-agent-connect/active-minutes-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Active Minutes Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `active-minutes-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Active Minutes Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "active-minutes-calculator": {
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

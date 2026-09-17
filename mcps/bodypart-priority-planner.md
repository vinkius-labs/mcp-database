# Bodypart Priority Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bodypart-priority-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Optimizes training splits and volume to prioritize lagging muscle groups.

## Description
The Bodypart Priority Planner reconfigures your workout schedule to address muscular imbalances. By analyzing the development gap between your current muscle status and your target goals, it uses priority training principles to adjust frequency and volume. Use `plan_training_split` to generate a full weekly schedule, `calculate_volume_distribution` to allocate weekly sets, `suggest_exercise_selection` for movement types, and `optimize_frequency_adjustment` to determine how often to train each group.


## Available Tools (4)
- **calculate_volume_distribution**: Determines how many sets should be assigned to each muscle group per week
- **optimize_frequency_adjustment**: Calculates how many times per week each muscle group should be trained given the user's constraints
- **plan_training_split**: Generates a full training weekly schedule optimized for the user's lagging muscle groups
- **suggest_exercise_selection**: Recommends specific types of exercises based on the priority and needs of a muscle group


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bodypart Priority Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a weekly training plan for 4 days where my Chest is at level 5 but I want it at level 8, and my Back is at level 7 with a target of 8."

**🤖 AI Agent:**
> Your 4-day plan will prioritize Chest with high frequency and volume, while Back will receive maintenance training to close the gap efficiently.

---

**👤 You:**
> "How many sets should I do for my Quads if I have 20 total sets available per week?"

**🤖 AI Agent:**
> Based on your development gap, the planner will allocate a specific portion of your 20 sets to Quads to ensure they reach your target level.

---

**👤 You:**
> "What exercises should I do for high priority Shoulders?"

**🤖 AI Agent:**
> For high priority Shoulders, you should focus on heavy compound movements like overhead presses, supplemented by isolation exercises like lateral raises.


## ❓ FAQ

**Q: How does the planner decide which muscles are high priority?**
Priority is determined by the development gap, which is the difference between your current muscle level and your target goal level.

**Q: Can I use this for a 3-day training split?**
Yes, you can specify any number of available training days between 1 and 7 when using `plan_training_split`.

**Q: What kind of exercises will be recommended?**
The planner recommends a mix of compound movements for mechanical tension and isolation movements for metabolic stress based on the priority of the muscle group.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bodypart-priority-planner](https://vinkius.com/en/ai-agent-connect/bodypart-priority-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bodypart Priority Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bodypart-priority-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bodypart Priority Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bodypart-priority-planner": {
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

# Pull-up Progression Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pull-up-progression-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Generates structured training roadmaps to reach your pull-up repetition goals.

## Description
This MCP server provides a specialized training engine to bridge the gap between your current strength and your target pull-up repetitions. By using tools like `generate_progression_plan`, you can create a complete, structured training roadmap. The engine also allows you to `calculate_weekly_volume` for specific training phases, `get_assistance_requirement` to determine necessary mechanical aid (like bands), and `validate_progression_feasibility` to ensure your strength goals are realistic within your chosen timeline.


## Available Tools (4)
- **calculate_weekly_volume**: Determines the specific repetition targets for a single week within a larger plan
- **generate_progression_plan**: Creates a complete, structured training roadmap from a starting point to a target goal
- **get_assistance_requirement**: Identifies what type of mechanical aid is required for a user at a specific stage or rep count
- **validate_progression_feasibility**: Checks if a user's goal is realistic given their current strength and the requested time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pull-up Progression Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I can do 0 pull-ups. I want to do 5 pull-ups in 8 weeks. Can you make a plan?"

**🤖 AI Agent:**
> To reach 5 unassisted pull-ups in 8 weeks, your plan will focus on Scapular Pulls, Negative Pull-ups, and Banded Pull-ups to build the necessary foundation.

---

**👤 You:**
> "I can do 3 pull-ups. How many reps should I do in week 4 of a 10-week plan?"

**🤖 AI Agent:**
> In week 4 of your 10-week plan, your target is 12 repetitions with a moderate intensity level.

---

**👤 You:**
> "Is it possible to go from 1 pull-up to 10 pull-ups in only 2 weeks?"

**🤖 AI Agent:**
> No, that goal is not feasible. A more realistic timeline for such a significant increase would be approximately 12 to 16 weeks.


## ❓ FAQ

**Q: How do I know if my pull-up goal is realistic?**
You can use the `validate_progression_feasibility` tool. It analyzes your current capability against your target reps and timeline to provide a confidence score and suggested duration.

**Q: Can I plan my weekly workouts with this tool?**
Yes. Once you have a plan, you can use `calculate_weekly_volume` to find the exact repetition targets and intensity levels for any specific week in your progression.

**Q: What if I need help with resistance bands?**
The `get_assistance_requirement` tool identifies the type of mechanical aid, such as resistance bands, and the assistance percentage needed based on your current capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pull-up-progression-planner](https://vinkius.com/en/ai-agent-connect/pull-up-progression-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pull-up Progression Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pull-up-progression-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pull-up Progression Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pull-up-progression-planner": {
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

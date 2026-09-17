# Progressive Overload Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/progressive-overload-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fitness](../categories/fitness.md)

Generates structured strength and hypertrophy training progressions using periodization principles.

## Description
This MCP server provides advanced training programming tools. Use `plan_progression` to generate multi-week schedules, `calculate_deload_schedule` to manage recovery, `evaluate_progression_feasibility` to check if goals are realistic, and `get_exercise_constraints` to ensure physiological soundness. It applies linear and undulating periodization models based on trainee experience levels.


## Available Tools (4)
- **calculate_deload_schedule**: Determines the optimal timing and intensity for recovery periods
- **evaluate_progression_feasibility**: Checks if the user's goal is realistic given their current stats and timeframe
- **get_exercise_constraints**: Provides the standard rep and set ranges allowed for different exercise types
- **plan_progression**: Generates a complete, multi-week training schedule based on specific user goals and constraints


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Progressive Overload Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can I increase my squat from 100kg to 110kg in 8 weeks if I am an intermediate lifter?"

**🤖 AI Agent:**
> Yes, that is a feasible goal for an intermediate lifter within an 8-week timeframe.

---

**👤 You:**
> "Create a 4-week linear progression plan for a beginner doing compound exercises, starting at 50kg and aiming for 60kg."

**🤖 AI Agent:**
> Week 1: 50kg, 5 reps, 3 sets. Week 2: 52.5kg, 5 reps, 3 sets. Week 3: 55kg, 5 reps, 3 sets. Week 4: 57.5kg, 5 reps, 3 sets.

---

**👤 You:**
> "What are the typical rep ranges for isolation exercises?"

**🤖 AI Agent:**
> Isolation exercises typically focus on higher rep ranges for hypertrophy.


## ❓ FAQ

**Q: How does the planner handle different experience levels?**
The tool adjusts the rate of weight increases and deload frequency based on whether the user is a beginner, intermediate, or advanced trainee.

**Q: Can I use undulating periodization?**
Yes, you can specify the `progressionModel` as 'undulating' when calling `plan_progression` to get fluctuating intensity and volume.

**Q: What is a deload?**
A deload is a scheduled period of reduced intensity or volume to allow for recovery from accumulated fatigue.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/progressive-overload-planner](https://vinkius.com/en/ai-agent-connect/progressive-overload-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Progressive Overload Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `progressive-overload-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Progressive Overload Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "progressive-overload-planner": {
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

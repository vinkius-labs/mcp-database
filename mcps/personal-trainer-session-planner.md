# Personal Trainer Session Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/personal-trainer-session-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate personalized, goal-oriented weight training session structures based on objectives and physical constraints.

## Description
This MCP server provides an automated system to generate complete, structured training sessions. By using the `plan_training_session` tool, you can create workouts that include a warm-up, a main metabolic or strength block, and a cooldown. The plan is dynamically calculated based on your training goal (such as Strength, Hypertrophy, Endurance, or Power), available equipment, target muscle groups, and any physical limitations to ensure safety and effectiveness.


## Available Tools (1)
- **plan_training_session**: Generates a personalized training session plan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Personal Trainer Session Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 45-minute hypertrophy session for chest and triceps using dumbbells, with no knee limitations."

**🤖 AI Agent:**
> Your 45-minute Hypertrophy session is ready. It includes a 7-minute warm-up, a main block featuring Dumbbell Chest Press and Tricep Extensions with 3 sets of 10 reps, and a 5-minute cooldown.

---

**👤 You:**
> "Create a 30-minute strength workout for legs using only bodyweight."

**🤖 AI Agent:**
> Your 30-minute Strength session is ready. It includes a 5-minute warm-up, a main block featuring Bodyweight Squats and Lunges with 5 sets of 5 reps, and a 5-minute cooldown.

---

**👤 You:**
> "Plan an endurance session for 60 minutes focusing on full body with any available equipment."

**🤖 AI Agent:**
> Your 60-minute Endurance session is ready. It includes a 10-minute warm-up, a high-intensity main block with short rest intervals, and a 5-minute cooldown.


## ❓ FAQ

**Q: How do I create a workout plan?**
Use the `plan_training_session` tool by providing your training goal, total duration, available equipment, target muscle groups, and any physical limitations.

**Q: Can I specify exercises to avoid?**
Yes, you can include specific movements or body parts in the `physicalLimitations` parameter to ensure they are excluded from your session plan.

**Q: What training goals are supported?**
The system supports STRENGTH, HYPERTROPHY, ENDURANCE, and POWER goals, each with unique repetition ranges and rest intervals.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/personal-trainer-session-planner](https://vinkius.com/mcp/personal-trainer-session-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Personal Trainer Session Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `personal-trainer-session-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Personal Trainer Session Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "personal-trainer-session-planner": {
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

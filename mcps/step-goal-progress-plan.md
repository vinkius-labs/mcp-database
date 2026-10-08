# Step Goal Progress Plan MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/step-goal-progress-plan)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate daily step requirements to reach your weekly activity goals.

## Description
This MCP server provides precise calculations to help users manage their weekly activity targets. By analyzing completed steps, planned activities, and remaining days, it determines exactly how many steps are needed daily to stay on track. Use `get_daily_requirement` to find your daily target, `get_progress_summary` for a high-level overview, `validate_plan_feasibility` to check if your goal is realistic, and `get_weekly_trajectory` to predict your end-of-week total.


## Available Tools (4)
- **get_weekly_trajectory**: Predicts the final end-of-week total based on current pace
- **validate_plan_feasibility**: Checks if the current plan is realistic against the weekly goal
- **get_daily_requirement**: Calculates the specific number of steps needed per day for the remaining days in the week
- **get_progress_summary**: Provides a high-level overview of how much of the weekly goal has been achieved


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Step Goal Progress Plan** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a weekly goal of 50,000 steps. I've done 15,000 steps so far, and I have 10,000 steps planned for tomorrow. There are 4 days left in the week. How many steps do I need per day?"

**🤖 AI Agent:**
> You need to take 6,250 steps per day for the remaining 4 days to reach your goal of 50,000 steps.

---

**👤 You:**
> "What is my current progress? My goal is 30,000 steps, I've completed 12,000, and I have 5,000 steps planned."

**🤖 AI Agent:**
> You have achieved 56.67% of your goal, with 13,000 steps remaining.

---

**👤 You:**
> "Is my goal of 100,000 steps feasible? I've done 20,000 steps, have 10,000 planned, and have 5 days left."

**🤖 AI Agent:**
> Your goal is High difficulty because you would need to take 14,000 steps every day to reach it.


## ❓ FAQ

**Q: How do I know how many steps I need to take today?**
You can use the `get_daily_requirement` tool. Provide your weekly goal, steps already completed, steps already planned for the future, and how many days are left in the week.

**Q: Can I check if my weekly goal is too ambitious?**
Yes, the `validate_plan_feasibility` tool evaluates your current progress and planned steps to determine if your goal is Low, Moderate, or High difficulty.

**Q: How can I predict my total steps at the end of the week?**
Use the `get_weekly_trajectory` tool to project your final total based on your current pace and planned activities.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/step-goal-progress-plan](https://vinkius.com/en/ai-agent-connect/step-goal-progress-plan)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Step Goal Progress Plan** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `step-goal-progress-plan` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Step Goal Progress Plan** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "step-goal-progress-plan": {
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

# Competition Peak Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/competition-peak-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [training](../categories/training.md)

Generate personalized training taper protocols, nutritional strategies, and peak performance windows.

## Description
The Competition Peak Planner helps athletes reach their physiological peak exactly on competition day. By using tools like `generate_tapering_schedules`, you can create a week-by-week reduction in training volume (40-60%) while maintaining intensity. Predict your supercompensation window with `calculate_peak_performance_window`, optimize glycogen stores via `get_carb_loading_nutrition_plan`, and ensure nothing is missed with `generate_pre_competition_checklist`.


## Available Tools (4)
- **get_carb_loading_nutrition_plan**: Provide a 3-day carbohydrate loading strategy
- **generate_pre_competition_checklist**: Generate a pre-competition logistics and physiological checklist
- **calculate_peak_performance_window**: Predict the athlete's peak performance window
- **generate_tapering_schedules**: Generate a week-by-week training taper schedule


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Competition Peak Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a tapering schedule for a marathon on 2024-12-01. My current weekly volume is 80km and intensity is High."

**🤖 AI Agent:**
> Your tapering schedule for the marathon on 2024-12-01 includes: Week 3: 64km (High intensity), Week 2: 52km (High intensity), Week 1: 40km (High intensity).

---

**👤 You:**
> "What should my carb loading plan look like for a competition on 2024-12-01 if I weigh 75kg?"

**🤖 AI Agent:**
> For your 75kg weight, the 3-day plan is: Day -3: Focus on complex carbs like oats; Day -2: Increase intake with pasta and rice; Day -1: High glycemic index foods like white bread and sports drinks.

---

**👤 You:**
> "Generate a checklist for a weightlifting competition in 5 days."

**🤖 AI Agent:**
> Your checklist: Check lifting belt and shoes, Finalize travel logistics, Ensure hydration levels are optimal, Confirm competition start time.


## ❓ FAQ

**Q: How does the tapering schedule work?**
The `generate_tapering_schedules` tool calculates a progressive reduction in your training volume by 40-60% while keeping your intensity levels consistent to prevent detraining.

**Q: Can I get a nutrition plan for carb loading?**
Yes, use the `get_carb_loading_nutrition_plan` tool by providing your weight and competition date to receive a 3-day strategy for maximizing glycogen stores.

**Q: How do I know when my peak performance will be?**
The `calculate_peak_performance_window` tool predicts the specific day and time range for your physiological supercompensation based on your taper duration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/competition-peak-planner](https://vinkius.com/mcp/competition-peak-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Competition Peak Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `competition-peak-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Competition Peak Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "competition-peak-planner": {
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

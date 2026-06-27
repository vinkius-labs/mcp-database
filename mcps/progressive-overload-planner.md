# Progressive Overload Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/progressive-overload-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [training](../categories/training.md)

Generate periodized strength training schedules based on 1RM progression targets.

## Description
The Progressive Overload Planner is a mathematical engine designed to bridge the gap between current strength levels and target performance. By utilizing proven methodologies like Linear Progression, Double Progression, and Undulating Periodization, this MCP server generates precise week-by-week training schedules. Use `generate_overload_plan` to create your roadmap, `assess_load_intensity` to understand the physiological focus of your lifts, and `forecast_plateau_risk` to identify potential stagnation points before they happen.


## Available Tools (3)
- **assess_load_intensity**: Assesses the training intensity zone based on weight and 1RM
- **forecast_plateau_risk**: Forecasts the risk of hitting a plateau in a training plan
- **generate_overload_plan**: Generates a week-by-week progressive overload training plan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Progressive Overload Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 4-week training plan starting from a 100kg squat to reach 105kg using the LINEAR model."

**🤖 AI Agent:**
> Your 4-week plan is ready. Week 1: 100kg, 5 reps; Week 2: 101.25kg, 5 reps; Week 3: 102.5kg, 5 reps; Week 4: 103.75kg, 5 reps.

---

**👤 You:**
> "If I lift 80kg for 10 reps with a 100kg 1RM, what is the intensity zone?"

**🤖 AI Agent:**
> The intensity is 80% of your 1RM, which falls into the HYPERTROPHY zone.

---

**👤 You:**
> "Analyze this plan for plateau risks: {"weeks": [{"weekNumber": 1, "progressionRate": 0.05}, {"weekNumber": 2, "progressionRate": 0.15}]}"

**🤖 AI Agent:**
> High risk detected in week 2 due to an aggressive 15% progression rate jump.


## ❓ FAQ

**Q: How do I generate a new training plan?**
Use the `generate_overload_plan` tool by providing your current 1RM, target 1RM, duration in weeks, and preferred training model.

**Q: What are the different training models available?**
The engine supports `LINEAR` for beginners, `DOUBLE_PROGRESSION` for intermediates, and `UNDULATING_PERIODIZATION` for advanced lifters.

**Q: Can I check if a specific weight is too heavy?**
Yes, you can use the `assess_load_intensity` tool to determine the intensity zone (Strength, Hypertrophy, or Endurance) for any given weight and repetition count.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/progressive-overload-planner](https://vinkius.com/mcp/progressive-overload-planner)
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

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

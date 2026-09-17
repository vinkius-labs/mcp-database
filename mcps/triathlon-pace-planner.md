# Triathlon Pace Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/triathlon-pace-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [planning](../categories/planning.md)

Strategic pacing, nutrition, and physiological planning for triathletes.

## Description
Triathlon Pace Planner connects AI agents to specialized triathlon modeling. It provides precise race duration estimates using `get_race_duration_estimate`, detailed effort breakdowns via `generate_pacing_strategy`, customized nutrition schedules through `calculate_nutrition_plan`, and physiological targets with `get_race_profile_metrics`.


## Available Tools (4)
- **calculate_nutrition_plan**: Determines the timing and volume of nutritional intake required to sustain performance
- **generate_pacing_strategy**: Provides a detailed breakdown of how the athlete should manage their effort throughout the race
- **get_race_duration_estimate**: Calculates the expected time for each individual leg and the total estimated race time
- **get_race_profile_metrics**: Provides physiological metrics and intensity targets for the athlete to monitor


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Triathlon Pace Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Estimate my time for a sprint triathlon where I swim at 50 m/min, bike at 30 km/h, and run at 10 min/km, with 5 minute transitions."

**🤖 AI Agent:**
> Your estimated sprint triathlon time is 55 minutes, including 10 minutes for both transitions.

---

**👤 You:**
> "What should my nutrition plan be for a 70.3 race lasting 5 hours if I weigh 75kg and the intensity is moderate?"

**🤖 AI Agent:**
> For a 5-hour race at moderate intensity, your target is 300g of carbohydrates and 2500ml of fluids.

---

**👤 You:**
> "Give me a pacing strategy for an Olympic distance race with steady swim, threshold bike, and negative-split run."

**🤖 AI Agent:**
> Your strategy involves a steady swim, a high-intensity threshold effort on the bike, and a progressive negative-split run to finish strong.


## ❓ FAQ

**Q: How accurate are the race time estimates?**
Estimates are based on the athlete's provided speeds and the specific race distance. Using `get_race_duration_estimate` provides a calculated baseline including transition times.

**Q: Can I plan my nutrition for an Ironman?**
Yes. By using `calculate_nutrition_plan`, you can determine the required carbohydrate and fluid intake based on your weight and the total race duration.

**Q: How do I manage my effort levels?**
You can use `generate_pacing_strategy` to define specific effort levels like conservative, steady, or aggressive for each leg of the race.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/triathlon-pace-planner](https://vinkius.com/en/ai-agent-connect/triathlon-pace-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Triathlon Pace Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `triathlon-pace-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Triathlon Pace Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "triathlon-pace-planner": {
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

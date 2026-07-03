# Weight Loss Compounder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/weight-loss-compounder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health-fitness](../categories/health-fitness.md)

Model non-linear weight loss trajectories by accounting for metabolic slowdown.

## Description
The Weight Loss Compounder is a physiological simulator that models realistic, decelerating weight loss journeys. Unlike simple linear calculators, this tool accounts for the biological reality that as body mass decreases, Total Daily Energy Expenditure (TDEE) also drops, causing progress to naturally slow down unless caloric intake is adjusted. Using tools like `calculate_projection_summary`, `get_weekly_trajectory`, and `analyze_metabolic_efficiency`, you can project how your weight will change week-by-week based on your starting weight, target weight, and daily caloric intake. It provides a detailed view of the deceleration curve as your body reaches a new equilibrium.


## Available Tools (3)
- **analyze_metabolic_efficiency**: Analyze the deceleration of weight loss efficiency
- **calculate_projection_summary**: Calculate a weight loss projection summary
- **get_weekly_trajectory**: Get a detailed weekly weight loss trajectory


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weight Loss Compounder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I weigh 250 lbs and want to reach 200 lbs. I eat 2000 calories a day. How long will it take?"

**🤖 AI Agent:**
> Based on your starting weight of 250 lbs and a daily intake of 2000 calories, you can expect to reach your target of 200 lbs in approximately 34 weeks.

---

**👤 You:**
> "Show me the weekly progress for someone starting at 220 lbs, targeting 180 lbs, with a 1800 calorie daily intake."

**🤖 AI Agent:**
> Week 1: Start 220.0 lbs, End 217.5 lbs, Deficit 1400 kcal. Week 2: Start 217.5 lbs, End 215.1 lbs, Deficit 1350 kcal. (Simulation continues until target is reached).

---

**👤 You:**
> "How much will my weight loss rate slow down if I go from 280 lbs to 240 lbs eating 2200 calories?"

**🤖 AI Agent:**
> The metabolic deceleration for this journey is approximately 12.5%, meaning your weekly weight loss rate will be significantly lower by the time you reach 240 lbs compared to your first week.


## ❓ FAQ

**Q: How does the simulation account for metabolic slowdown?**
The simulator recalculates your TDEE every week based on your new, lower weight. As you lose mass, your body requires fewer calories to maintain itself, which naturally reduces your caloric deficit and slows the rate of loss.

**Q: Can I see a week-by-week breakdown of my progress?**
Yes, by using the `get_weekly_trajectory` tool, you can generate a detailed chronological log showing your weight at the start and end of each week along with the weekly calorie deficit.

**Q: What does the metabolic efficiency analysis show?**
The `analyze_metabolic_efficiency` tool quantifies the deceleration of your weight loss by comparing your initial weekly loss rate to your final weekly loss rate, providing a percentage decrease in efficiency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/weight-loss-compounder](https://vinkius.com/mcp/weight-loss-compounder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weight Loss Compounder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `weight-loss-compounder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weight Loss Compounder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weight-loss-compounder": {
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

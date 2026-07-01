# Weight Loss Plateau Recalculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/weight-loss-plateau-recalculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Predictive simulation engine to model dietary adjustments for overcoming weight loss stalls.

## Description
The Weight Loss Plateau Recalculator is a specialized simulation tool designed to help users navigate metabolic adaptation. By modeling the relationship between calorie intake and body mass, it predicts how periodic calorie reductions can overcome plateaus. Using tools like `simulate_dietary_adaptation`, you can project month-by/month weight changes and identify when your current plan might lead to a stall based on your specific `stallThresholdKg`.


## Available Tools (3)
- **simulate_dietary_adaptation**: Simulate long-term weight loss progress with potential calorie adjustments
- **calculate_maintenance_burn**: Calculate calories needed to maintain current weight
- **evaluate_plateau_risk**: Evaluate the risk of a weight loss plateau


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Weight Loss Plateau Recalculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much should I reduce my calories if I stop losing weight at 0.3kg per week?"

**🤖 AI Agent:**
> To overcome a stall where progress falls below 0.3kg/week, you can run a simulation using `simulate_dietary_adaptation` with a reduction amount of 100 or 150 calories to see the projected impact on your timeline.

---

**👤 You:**
> "Estimate my maintenance calories if I weigh 95kg."

**🤖 AI Agent:**
> Based on a weight of 95kg, your estimated daily maintenance energy requirement is approximately 2450 kcal.

---

**👤 You:**
> "Simulate my progress from 100kg to 85kg starting at 2200 calories with a 0.3kg threshold."

**🤖 AI Agent:**
> The simulation shows that you will reach 85kg in approximately 24 weeks, with calorie adjustments occurring in month 3 and month 5 to maintain progress above your threshold.


## ❓ FAQ

**Q: How does the simulation handle weight loss plateaus?**
The engine monitors your weekly progress. If the average weight loss over a two-week window falls below your defined threshold, the `simulate_dietary_adaptation` tool automatically applies a calorie reduction to help restart progress.

**Q: Can I estimate my maintenance calories?**
Yes, you can use the `calculate_maintenance_burn` tool by providing your current weight in kilograms to get an estimate of your daily energy requirements.

**Q: What is the 7700 kcal rule used in this tool?**
The simulation uses the principle that a cumulative deficit of approximately 7700 calories is equivalent to 1 kg of weight loss, allowing for mathematically grounded projections.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/weight-loss-plateau-recalculator](https://vinkius.com/mcp/weight-loss-plateau-recalculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Weight Loss Plateau Recalculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `weight-loss-plateau-recalculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Weight Loss Plateau Recalculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "weight-loss-plateau-recalculator": {
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

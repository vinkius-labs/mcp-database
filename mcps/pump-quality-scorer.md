# Pump Quality Scorer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pump-quality-scorer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [analytics](../categories/analytics.md)

Analyzes training sessions to score muscle pump effectiveness.

## Description
This MCP server provides an analytical engine to evaluate how effectively a training session induces muscle hypertrophy-related pumps. By analyzing variables like exercise selection, volume, rest periods, and nutrition, it provides actionable insights. Use `calculate_pump_score` to get a composite score, `analyze_volume_impact` to check work intensity, `evaluate_nutrition_timing` to assess metabolic readiness, and `get_rest_period_efficiency` to optimize metabolic stress accumulation.


## Available Tools (4)
- **calculate_pump_score**: Evaluates the overall effectiveness of a single training session in producing a muscle pump
- **evaluate_nutrition_timing**: Assesses how current nutritional intake supports blood volume and glycogen for the pump
- **get_rest_period_efficiency**: Determines if the rest intervals allowed for enough metabolic stress accumulation
- **analyze_volume_impact**: Determines if the volume performed was sufficient or excessive for optimal pump induction


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pump Quality Scorer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my pump score for a session with 10 sets of bicep curls, 45 seconds rest, and I am in a pre-workout-carb-rich state."

**🤖 AI Agent:**
> Your pump score is 85. The primary drivers were high metabolic stress from short rest periods and optimal glycogen availability.

---

**👤 You:**
> "Was my volume sufficient for an isolation exercise session with 50 total reps?"

**🤖 AI Agent:**
> The volume rating is Optimal. The metabolic stress level is high, and no immediate adjustment is needed.

---

**👤 You:**
> "How is my hydration affecting my pump potential if I am currently dehydrated?"

**🤖 AI Agent:**
> Dehydration is significantly reducing your pump potential. Increasing fluid intake is recommended to improve blood volume.


## ❓ FAQ

**Q: How is the pump score calculated?**
The `calculate_pump_score` tool evaluates the intersection of exercise selection, total volume, rest intervals, and nutritional status to produce a normalized quality score.

**Q: Can I use this to optimize my rest periods?**
Yes, you can use `get_rest_period_efficiency` to determine if your rest intervals were optimized for metabolic stress accumulation.

**Q: Does nutrition affect the results?**
Absolutely. The `evaluate_nutrition_timing` tool assesses how your hydration and feeding state impact your pump potential.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pump-quality-scorer](https://vinkius.com/en/ai-agent-connect/pump-quality-scorer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pump Quality Scorer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pump-quality-scorer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pump Quality Scorer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pump-quality-scorer": {
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

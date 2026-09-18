# Calorie Deficit Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/calorie-deficit-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Design safe, science-based weight loss strategies with precise caloric and metabolic calculations.

## Description
The Calorie Deficit Planner provides a scientific framework for weight loss. It uses tools like `calculate_metabolic_stats` to establish your physiological baseline and `analyze_deficit_plan` to determine if your weight loss goals are realistic and safe. The planner accounts for adaptive thermogenesis and uses `check_muscle_preservation_safety` to ensure you maintain lean muscle mass while losing weight. It is designed to prevent metabolic slowdown and ensure nutritional safety.


## Available Tools (4)
- **analyze_deficit_plan**: Provides a complete breakdown of a proposed weight loss strategy
- **calculate_metabolic_stats**: Determines the physiological baseline for the user
- **check_muscle_preservation_safety**: Evaluates if the current deficit plan is aggressive enough to risk significant muscle loss
- **estimate_adaptive_thermogenesis_impact**: Predicts how much metabolic adaptation might slow down progress over time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Calorie Deficit Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I weigh 90kg and want to reach 80kg in 12 weeks. I am moderately active. Can you plan my deficit?"

**🤖 AI Agent:**
> To reach 80kg from 90kg in 12 weeks, your daily calorie target should be approximately 2,150 calories. This plan is feasible and maintains a safe weight loss rate.

---

**👤 You:**
> "Calculate my metabolic stats. I am a 30 year old male, 180cm tall, weighing 85kg."

**🤖 AI Agent:**
> Your Basal Metabolic Rate (BMR) is 1,850 calories and your Total Daily Energy Expenditure (TDEE) is approximately 2,545 calories based on a sedentary activity level.

---

**👤 You:**
> "Is a 500 calorie deficit safe for someone weighing 70kg with a BMR of 1500?"

**🤖 AI Agent:**
> Yes, a 500 calorie deficit is safe as your target intake remains above your BMR, minimizing the risk of significant muscle loss.


## ❓ FAQ

**Q: How does this tool ensure my weight loss plan is safe?**
The tool uses `check_muscle_preservation_safety` and feasibility checks to ensure your daily calorie target does not fall below your BMR and that your weekly weight loss stays within healthy physiological limits.

**Q: What is adaptive thermogenesis?**
Adaptive thermogenesis is the metabolic slowdown that occurs as the body adapts to a prolonged caloric deficit. You can use `estimate_adaptive_thermogenesis_impact` to predict how this might affect your progress.

**Q: Can I use this with Claude or Cursor?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/calorie-deficit-planner](https://vinkius.com/en/ai-agent-connect/calorie-deficit-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Calorie Deficit Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `calorie-deficit-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Calorie Deficit Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "calorie-deficit-planner": {
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

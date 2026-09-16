# Breath-Hold Capacity Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/breath-hold-capacity-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [health](../categories/health.md)

Predict apnea capabilities and optimize training for surfers.

## Description
This MCP server provides specialized tools for surfers and apnea athletes to estimate their breath-hold capacity. It differentiates between static apnea and dynamic apnea to provide accurate physiological predictions. Use `estimate_static_apnea` to predict motionless breath-hold duration, or `estimate_dynamic_apnea` to account for movement during activities like surfing. The server also includes `get_training_recommendations` for tailored exercise plans and `analyze_training_progress` to track physiological adaptation over time.


## Available Tools (4)
- **analyze_training_progress**: Evaluates how recent training has influenced the user's estimated capacities
- **estimate_dynamic_apnea**: Predicts breath-hold duration during active movement, such as surfing or swimming
- **estimate_static_apnea**: Predicts how long a user can hold their breath while remaining motionless
- **get_training_recommendations**: Provides tailored training advice based on the user's current capacities and goals


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Breath-Hold Capacity Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Estimate my static apnea capacity with a lung capacity of 5 liters, moderate fitness, and a CO2 tolerance of 0.8."

**🤖 AI Agent:**
> Your estimated static apnea time is 145 seconds with a high confidence level.

---

**👤 You:**
> "What training should I do if my static capacity is 120s and my dynamic capacity is 45s, and I want to increase CO2 tolerance?"

**🤖 AI Agent:**
> To increase CO2 tolerance, you should focus on CO2 tables and specialized breath-holding drills to reduce the urge to breathe.

---

**👤 You:**
> "Estimate my dynamic apnea for a high-intensity surf session with 4 liters of lung capacity and elite fitness."

**🤖 AI Agent:**
> Your estimated dynamic apnea time is 55 seconds.


## ❓ FAQ

**Q: What is the difference between static and dynamic apnea?**
Static apnea is holding your breath while remaining still, whereas dynamic apnea involves movement like swimming or duck-diving, which consumes oxygen faster.

**Q: How can I improve my training?**
You can use the `get_training_recommendations` tool to receive specific exercises based on your current static and dynamic capacities.

**Q: Can I track my progress over time?**
Yes, the `analyze_training_progress` tool allows you to evaluate how your training volume has influenced your capacity improvements.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/breath-hold-capacity-estimator](https://vinkius.com/en/ai-agent-connect/breath-hold-capacity-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Breath-Hold Capacity Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `breath-hold-capacity-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Breath-Hold Capacity Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "breath-hold-capacity-estimator": {
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

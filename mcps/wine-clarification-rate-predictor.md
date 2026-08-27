# Wine Clarification Rate Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-clarification-rate-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [enology](../categories/enology.md)

Predict wine settling times and optimize clarification methods using fluid dynamics.

## Description
This MCP server provides advanced enology tools to predict how quickly suspended solids will separate from wine. By applying Stokes' Law to particle size distribution, viscosity, and temperature, it helps winemakers optimize their production workflows. Use `predict_settling_time` to estimate time to target clarity, `calculate_fining_impact` to model bentonite effectiveness, `calculate_centrifuge_performance` for mechanical throughput, and `optimize_method_selection` to choose between gravity, centrifuge, or flotation based on speed or cost priorities.


## Available Tools (4)
- **calculate_centrifuge_performance**: Estimates the processing capacity and speed when using mechanical centrifugation
- **calculate_fining_impact**: Predicts how much the clarification speed will increase if bentonite is added
- **optimize_method_selection**: Recommends the most efficient settling method based on the wine's current state
- **predict_settling_time**: Determines how long it will take for the wine to reach a specific clarity level


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Clarification Rate Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long will it take for my wine to reach a turbidity of 0.5 using gravity settling? The particle sizes are [10, 20, 30], viscosity is 1.2, and temperature is 20."

**🤖 AI Agent:**
> Based on the provided parameters, the estimated settling time to reach a turbidity of 0.5 using gravity is 48.5 hours.

---

**👤 You:**
> "Which method should I use if I need the fastest clarification possible? Particle sizes are [5, 15, 25], viscosity is 1.1, and temperature is 18."

**🤖 AI Agent:**
> To achieve the fastest clarification, the recommended method is Centrifuge.

---

**👤 You:**
> "What is the impact of adding 5 units of bentonite to my wine?"

**🤖 AI Agent:**
> Adding 5 units of bentonite is estimated to increase the settling velocity by 2.5x and reduce total clarification time by 40%.


## ❓ FAQ

**Q: How does temperature affect the prediction?**
Temperature influences wine viscosity. As temperature increases, viscosity typically decreases, which accelerates the settling velocity of particles.

**Q: Can I compare different settling methods?**
Yes, you can use `optimize_method_selection` to compare Gravity, Centrifuge, and Flotation based on whether you prioritize speed or cost.

**Q: What is the purpose of the bentonite tool?**
The `calculate_fining_impact` tool predicts how much the clarification speed will increase when bentonite is added to the wine.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-clarification-rate-predictor](https://vinkius.com/ai-agent-connect/wine-clarification-rate-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Clarification Rate Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-clarification-rate-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Clarification Rate Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-clarification-rate-predictor": {
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

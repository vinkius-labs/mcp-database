# Tilapia Growth & Thermal Modeling MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/tilapia-growth-thermal-modeling)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [biology](../categories/biology.md)

Predictive modeling for tilapia growth, feed efficiency, and survival based on thermal profiles.

## Description
This MCP server provides advanced predictive modeling for tilapia aquaculture. It allows AI agents to simulate growth trajectories, evaluate nutritional efficiency, and predict population survival by analyzing thermal unit growth coefficients (TGC) and environmental stressors. Use `predict_growth_trajectory` to estimate harvest timelines, `evaluate_efficiency_metrics` to analyze FCR, `estimate_survival_probability` to assess mortality risks, and `identify_thermal_optimum` to find the ideal temperature window for your specific stocking density.


## Available Tools (4)
- **evaluate_efficiency_metrics**: Analyzes the nutritional and economic efficiency of the feeding program
- **estimate_survival_probability**: Predicts the likelihood of the fish population surviving the growth cycle
- **identify_thermal_optimum**: Finds the most efficient temperature range for a specific feeding and density setup
- **predict_growth_trajectory**: Calculates the projected weight gain and time required to reach a target weight


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tilapia Growth & Thermal Modeling** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many days will it take for 50g tilapia to reach 500g if the temperature is consistently 28°C with a feeding rate of 3g/day and a density of 5 fish/m³?"

**🤖 AI Agent:**
> Based on a constant temperature of 28°C, it will take approximately 142 days to reach the target weight of 500g.

---

**👤 You:**
> "What is the predicted survival rate for 1000 fish at a density of 10 fish/m³ with a temperature profile fluctuating between 24°C and 30°C?"

**🤖 AI Agent:**
> The predicted survival rate for this population is 0.88, meaning approximately 880 fish are expected to survive the cycle.

---

**👤 You:**
> "What is the best temperature for growth if I am feeding 4g per day at a density of 4 fish/m³?"

**🤖 AI Agent:**
> The optimal temperature for these parameters is 29.5°C, with an efficiency window between 28.5°C and 30.5°C.


## ❓ FAQ

**Q: How does temperature affect the growth predictions?**
The model uses the Thermal Unit Growth Coefficient (TGC) to calculate how water temperature influences weight gain. Deviations from the optimal range or high fluctuations can trigger stress responses that reduce growth and survival.

**Q: Can I predict when my tilapia will be ready for harvest?**
Yes, by using the `predict_growth_trajectory` tool, you can provide initial weight, feeding rates, and a temperature profile to estimate the total days required to reach your target harvest weight.

**Q: How is feed efficiency measured?**
Efficiency is measured via the Feed Conversion Ratio (FCR). You can use `evaluate_efficiency_metrics` to analyze how effectively your feeding program converts feed into biomass relative to the thermal environment.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/tilapia-growth-thermal-modeling](https://vinkius.com/ai-agent-connect/tilapia-growth-thermal-modeling)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tilapia Growth & Thermal Modeling** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tilapia-growth-thermal-modeling` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tilapia Growth & Thermal Modeling** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tilapia-growth-thermal-modeling": {
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

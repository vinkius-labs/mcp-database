# Poultry Growth Curve Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/poultry-growth-curve-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predict broiler development and economic timing using the Gompertz growth model.

## Description
This MCP connects AI agents to specialized poultry biological modeling. It uses the Gompertz growth function to predict broiler weight gain, feed intake, and Feed Conversion Ratio (FCR) based on strain, sex, diet energy, and temperature. Use `calculate_growth_trajectory` to generate daily growth schedules, `estimate_optimal_market_day` to find the most efficient harvest time, `evaluate_environmental_impact` to assess thermal stress, and `compare_diet_scenarios` to test different feed energy levels.


## Available Tools (4)
- **calculate_growth_trajectory**: Generates a day-by-day growth schedule for a specific broiler profile
- **compare_diet_scenarios**: Analyzes how changing the feed energy affects the growth timeline and efficiency
- **estimate_optimal_market_day**: Identifies the best day to harvest birds to balance weight targets and economic efficiency
- **evaluate_environmental_impact**: Quantifies how much the temperature profile is degrading the potential performance of a specific strain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Poultry Growth Curve Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a growth schedule for Ross 308 males aiming for 2.5kg with 3000 kcal/kg diet at 25°C."

**🤖 AI Agent:**
> The growth trajectory for Ross 308 shows the birds reaching 2.5kg on day 38, with a cumulative feed intake of 4.8kg and an average FCR of 1.92.

---

**👤 You:**
> "What is the best day to harvest Cobb 500 birds if I want them to weigh at least 2kg?"

**🤖 AI Agent:**
> The optimal harvest day for Cobb 500 to reach 2kg is day 32, providing an economic efficiency score of 0.85.

---

**👤 You:**
> "How much will a temperature of 32°C impact the growth of my Ross 308 flock?"

**🤖 AI Agent:**
> At 32°C, the thermal stress level is categorized as Moderate, resulting in a performance penalty of 0.15 on the growth coefficient.


## ❓ FAQ

**Q: How does temperature affect the predictions?**
Temperature impacts the growth coefficient. High temperatures increase thermal stress, which reduces weight gain and increases the FCR.

**Q: Which broiler strains are supported?**
The model supports major commercial strains including Ross 308 and Cobb 500.

**Q: Can I compare different feed types?**
Yes, you can use `compare_diet_scenarios` to evaluate how different caloric densities affect the growth timeline and efficiency.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/poultry-growth-curve-predictor](https://vinkius.com/ai-agent-connect/poultry-growth-curve-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Poultry Growth Curve Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `poultry-growth-curve-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Poultry Growth Curve Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "poultry-growth-curve-predictor": {
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

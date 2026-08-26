# Peppermint Oil Composition Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/peppermint-oil-composition-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predict chemical composition and economic value of peppermint oil.

## Description
This MCP server provides predictive modeling for peppermint (*Mentha × piperita*) essential oil. By analyzing growth stages, temperature differentials, and plant stress, it calculates the expected concentrations of menthol, menthone, and menthofuran. Users can use `predict_composition` to model chemical profiles, `estimate_oil_value` to project market worth, `analyze_diurnal_impact` to optimize harvest timing, and `get_variety_baseline` to compare results against ideal cultivar standards.


## Available Tools (4)
- **get_variety_baseline**: Retrieves the standard expected chemical profile for a specific peppermint variety under ideal conditions
- **analyze_diurnal_impact**: Determines how the timing of the harvest within a 24-hour cycle would have affected the final oil concentration
- **estimate_oil_value**: Calculates the projected market value of the oil based on its predicted quality
- **predict_composition**: Provides a detailed chemical profile of the peppermint oil based on specific environmental and biological inputs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Peppermint Oil Composition Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the composition for a vegetative stage peppermint with 25C day and 15C night temperatures and no stress."

**🤖 AI Agent:**
> The predicted composition is 55% menthol, 12% menthone, and 2% menthofuran, with a total oil yield of 1.5%.

---

**👤 You:**
> "What is the estimated value for 50 liters of oil with 60% menthol and 5% menthofuran?"

**🤖 AI Agent:**
> The estimated value for 50 liters is $1,250.00 with a quality grade of A.

---

**👤 You:**
> "How much does harvesting at midday versus dawn affect the concentration?"

**🤖 AI Agent:**
> Harvesting at midday results in a concentration multiplier of 0.85, whereas dawn provides a multiplier of 1.15 due to higher oil accumulation overnight.


## ❓ FAQ

**Q: How does temperature affect the prediction?**
The model uses the difference between `dayTemperature` and `nightTemperature` to adjust the ratio of menthol to menthone, as temperature fluctuations significantly impact terpene biosynthesis.

**Q: Can I estimate the market value of my harvest?**
Yes, by using the `estimate_oil_value` tool with your predicted composition and expected volume, you can obtain a projected USD value and quality grade.

**Q: What happens if the plant is under stress?**
The `predict_composition` tool incorporates `stressHistory` to adjust the concentration of menthofuran, which can impact the final quality and value of the oil.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/peppermint-oil-composition-predictor](https://vinkius.com/ai-agent-connect/peppermint-oil-composition-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Peppermint Oil Composition Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `peppermint-oil-composition-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Peppermint Oil Composition Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "peppermint-oil-composition-predictor": {
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

# Wine Citric Acid Metabolism Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-citric-acid-metabolism-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [predictive-modeling](../categories/predictive-modeling.md)

Predicts diacetyl formation and sensory profiles during Malolactic Fermentation.

## Description
This MCP server provides predictive modeling for the conversion of citric acid into diacetyl during Malolactic Fermentation (MLF). It allows winemakers to forecast the buttery character of a wine by simulating the citrate lyase pathway. Using `simulate_citrate_degradation`, you can determine the peak diacetyl production based on bacterial strain and temperature. The `predict_sensory_profile` tool calculates the resulting buttery intensity after accounting for yeast-mediated diacetyl reduction. Additionally, `analyze_strain_efficiency` evaluates the metabolic potential of specific bacteria, while `calculate_mlf_timeline` provides the expected duration of the fermentation process and the window of sensory stability.


## Available Tools (4)
- **analyze_strain_efficiency**: Analyzes how much buttery potential a specific strain provides relative to its citrate consumption
- **calculate_mlf_timeline**: Calculates the total expected duration of the MLF process and the window of sensory stability
- **predict_sensory_profile**: Predicts when the wine will exhibit buttery characteristics and how intense they will be
- **simulate_citrate_degradation**: Simulates how quickly citric acid is consumed and the peak diacetyl production level


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Citric Acid Metabolism Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much diacetyl will be produced if I start with 2.5 g/L of citric acid using strain LAB-01 at 18 degrees Celsius and pH 3.2?"

**🤖 AI Agent:**
> The peak diacetyl concentration is predicted to be 0.45 mg/L with a degradation rate of 0.12 g/L per day.

---

**👤 You:**
> "What will the buttery intensity be for a peak diacetyl of 0.5 mg/L if the yeast activity level is 0.7?"

**🤖 AI Agent:**
> The predicted buttery intensity is 0.15, as the yeast will reduce a significant portion of the diacetyl.

---

**👤 You:**
> "How efficient is strain LAB-01 at converting citric acid?"

**🤖 AI Agent:**
> Strain LAB-01 has a conversion efficiency of 85% and a diacetyl yield of 0.18 mg per gram of citrate.


## ❓ FAQ

**Q: How does this tool help in predicting wine flavor?**
It uses the `simulate_citrate_degradation` tool to model how citric acid is converted into diacetyl, allowing you to predict the intensity of buttery aromas before fermentation is complete.

**Q: Can I account for yeast activity in my predictions?**
Yes, the `predict_sensory_profile` tool includes a yeast activity coefficient to simulate how much diacetyl will be reduced by yeast during the process.

**Q: What parameters are needed for the MLF timeline?**
To use `calculate_mlf_timeline`, you need to provide the bacterial strain, the fermentation temperature, and the initial citric acid concentration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-citric-acid-metabolism-predictor](https://vinkius.com/en/ai-agent-connect/wine-citric-acid-metabolism-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Citric Acid Metabolism Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-citric-acid-metabolism-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Citric Acid Metabolism Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-citric-acid-metabolism-predictor": {
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

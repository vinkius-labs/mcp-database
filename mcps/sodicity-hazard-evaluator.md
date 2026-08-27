# Sodicity Hazard Evaluator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sodicity-hazard-evaluator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Assess soil degradation risks and calculate gypsum requirements for sodic soil reclamation.

## Description
This MCP server provides specialized tools for irrigation management and soil health assessment. It allows AI agents to calculate the Sodium Adsorption Ratio (SAR) using `calculate_water_sar`, estimate soil Exchangeable Sodium Percentage (ESP) with `estimate_soil_esp`, and predict soil permeability loss via `evaluate_infiltration_risk`. Additionally, it calculates precise gypsum needs for soil reclamation using `recommend_reclamation_plan`. It is designed to help manage the risks of soil dispersion and surface sealing caused by sodium-rich irrigation water.


## Available Tools (4)
- **evaluate_infiltration_risk**: Predicts the risk of soil surface sealing and reduction in water infiltration
- **calculate_water_sar**: Determines the Sodium Adsorption Ratio (SAR) of irrigation water
- **estimate_soil_esp**: Estimates the Exchangeable Sodium Percentage (ESP) of a soil sample
- **recommend_reclamation_plan**: Calculates the necessary amount of gypsum required to reclaim sodic soil


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sodicity Hazard Evaluator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the SAR for water with 5 mmol/L sodium, 2 mmol/L calcium, and 1 mmol/L magnesium."

**🤖 AI Agent:**
> The calculated Sodium Adsorption Ratio (SAR) is 3.5, which falls under the Low hazard classification.

---

**👤 You:**
> "What is the risk of infiltration reduction if SAR is 15, EC is 2, and current infiltration is 10 mm/h?"

**🤖 AI Agent:**
> The risk level is Severe, with a predicted infiltration reduction of 65% and a high risk of clay dispersion.

---

**👤 You:**
> "How much gypsum is needed for a soil with 20% ESP, target 5% ESP, texture factor 1.2, depth 20cm, and bulk density 1.3?"

**🤖 AI Agent:**
> The required amount of gypsum is 4500 kg/ha, with high reclamation efficiency for this soil type.


## ❓ FAQ

**Q: How can I calculate the risk of soil sealing?**
You can use the `evaluate_infiltration_risk` tool by providing the SAR, EC, and the current infiltration rate of the soil.

**Q: What is the purpose of the gypsum recommendation tool?**
The `recommend_reclamation_plan` tool calculates the specific amount of gypsum needed per hectare to displace sodium and restore soil structure based on your target ESP.

**Q: Can I estimate the sodium levels in my soil?**
Yes, the `estimate_soil_esp` tool allows you to estimate the Exchangeable Sodium Percentage using the exchangeable sodium and cation exchange capacity values.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sodicity-hazard-evaluator](https://vinkius.com/ai-agent-connect/sodicity-hazard-evaluator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sodicity Hazard Evaluator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sodicity-hazard-evaluator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sodicity Hazard Evaluator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sodicity-hazard-evaluator": {
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

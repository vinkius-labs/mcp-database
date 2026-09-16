# Wine Higher Alcohol Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-higher-alcohol-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fermentation](../categories/fermentation.md)

Predicts fusel oil concentrations and sensory impact during wine fermentation.

## Description
This MCP server provides predictive modeling for wine fermentation. It uses yeast metabolism models to estimate the concentrations of higher alcohols like isoamyl alcohol and isobutanol. Users can use `get_predicted_alcohol_concentrations` to calculate specific levels, `predict_sensory_profile` to assess aroma impact, `evaluate_nitrogen_risk` to check for nitrogen deficiency, and `simulate_temperature_shift` to model how temperature changes affect the final profile.


## Available Tools (4)
- **evaluate_nitrogen_risk**: Determines if the current nitrogen level is sufficient to prevent excessive fusel oil production
- **get_predicted_alcohol_concentrations**: Predicts the specific concentrations of the four primary higher alcohols based on current fermentation parameters
- **predict_sensory_profile**: Translates predicted alcohol concentrations into a qualitative sensory description
- **simulate_temperature_shift**: Predicts how changing the fermentation temperature will alter the resulting higher alcohol profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Higher Alcohol Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What will the alcohol profile look like for a yeast strain with 20 mg/L nitrogen at 22 degrees Celsius and a fermentation rate of 1.5 g/L/h?"

**🤖 AI Agent:**
> The predicted concentrations are isoamyl alcohol: 12.5 mg/L, isobutanol: 8.2 mg/L, propanol: 4.1 mg/L, and phenylethanol: 3.5 mg/L. The sensory profile is expected to be slightly floral with a neutral finish.

---

**👤 You:**
> "Is my current nitrogen level of 15 mg/L sufficient for this yeast strain?"

**🤖 AI Agent:**
> No, the nitrogen level is deficient. It is recommended to add 10.0 mg/L of nitrogen to reach the optimal range for this strain.

---

**👤 You:**
> "What happens to the aroma if I drop the temperature from 25 to 18 degrees Celsius?"

**🤖 AI Agent:**
> Lowering the temperature will reduce the concentration of isoamyl alcohol by 2.4 mg/L and isobutanol by 1.8 mg/L, resulting in a cleaner, less solvent-like aroma profile.


## ❓ FAQ

**Q: How does nitrogen level affect the prediction?**
Nitrogen levels influence the Ehrlich pathway. Low nitrogen can trigger metabolic stress, increasing the production of higher alcohols via specific yeast pathways.

**Q: Can I simulate temperature changes?**
Yes, you can use `simulate_temperature_shift` to see how adjusting the fermentation temperature will change the predicted alcohol concentrations and sensory profile.

**Q: What alcohols are predicted?**
The model predicts concentrations for isoamyl alcohol, isobutanol, propanol, and phenylethanol.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-higher-alcohol-predictor](https://vinkius.com/en/ai-agent-connect/wine-higher-alcohol-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Higher Alcohol Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-higher-alcohol-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Higher Alcohol Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-higher-alcohol-predictor": {
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

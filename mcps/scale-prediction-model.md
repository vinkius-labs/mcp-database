# Scale Prediction Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/scale-prediction-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Predicts mineral scale formation in oilfield operations using water chemistry and environmental data.

## Description
This MCP server provides advanced thermodynamic analysis for oilfield water management. It allows AI agents to calculate the risk of mineral precipitation by analyzing ion concentrations, temperature, and pressure. Using `get_saturation_analysis`, agents can determine the saturation index and tendency for minerals like CaCO3 or BaSO4. The `predict_mixing_impact` tool helps forecast how seawater injection affects scaling risk, while `recommend_inhibitor` provides specific chemical dosage guidance. For broader operational planning, `evaluate_operational_risk` identifies critical temperature and pressure thresholds to maintain stable production.


## Available Tools (4)
- **predict_mixing_impact**: Predicts how the introduction of a second water source will affect scale formation
- **get_saturation_analysis**: Determines the thermodynamic state of specific minerals based on current water chemistry and environmental conditions
- **recommend_inhibitor**: Suggests the optimal chemical intervention to prevent the identified scale
- **evaluate_operational_risk**: Provides a high-level summary of scaling risk across a range of operating conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scale Prediction Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the scaling risk for water with high calcium and sulfate levels at 80°C and 150 bar?"

**🤖 AI Agent:**
> The saturation index for CaSO4 is 1.45, indicating a High scaling tendency at these conditions.

---

**👤 You:**
> "If I mix 20% seawater into my formation water, how will the scale risk change?"

**🤖 AI Agent:**
> Mixing 20% seawater increases the Barium Sulfate risk from Low to Moderate due to the introduction of sulfate ions.

---

**👤 You:**
> "Suggest an inhibitor for CaCO3 scale with a saturation index of 2.5 at 90°C."

**🤖 AI Agent:**
> A Phosphonate inhibitor is recommended with a dosage of 15 ppm to mitigate this scale.


## ❓ FAQ

**Q: What kind of scale can this model predict?**
The model predicts common oilfield scales including Calcium Carbonate (CaCO3), Barium Sulfate (BaSO4), and Calcium Sulfate (CaSO4) using `get_saturation_analysis`.

**Q: How does the model handle water mixing scenarios?**
You can use the `predict_mixing_impact` tool to simulate how mixing primary formation water with secondary sources like seawater changes the scaling tendency.

**Q: Can I get chemical dosage recommendations?**
Yes, the `recommend_inhibitor` tool provides the optimal inhibitor type and the required dosage in ppm based on the saturation index.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/scale-prediction-model](https://vinkius.com/en/ai-agent-connect/scale-prediction-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Scale Prediction Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `scale-prediction-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Scale Prediction Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scale-prediction-model": {
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

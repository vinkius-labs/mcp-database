# Wine MLF Progression Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-mlf-progression-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Models malolactic fermentation progression and predicts completion timelines.

## Description
This MCP server provides specialized tools for winemakers to model malolactic fermentation (MLF) progression. It calculates malic acid degradation rates, predicts the number of days until completion, and estimates diacetyl production. Using the `predict_mlf_progression` tool, users can analyze how pH, temperature, SO2, and alcohol levels impact fermentation. The `assess_mlf_risk` tool identifies potential fermentation failures, while `compare_strain_performance` allows for evaluating different Oenococcus oeni strains under specific wine profiles. Additionally, `get_optimal_conditions` provides the ideal environmental parameters for a chosen strain.


## Available Tools (4)
- **compare_strain_performance**: Compares how different Oenococcus oeni strains would perform under identical wine conditions
- **get_optimal_conditions**: Suggests the ideal environment to maximize fermentation speed for a specific strain
- **predict_mlf_progression**: Calculates the expected timeline and acid reduction for a specific wine profile
- **assess_mlf_risk**: Determines if the current wine conditions are likely to result in a stalled or failed fermentation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine MLF Progression Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the MLF progression for a wine with 5g/L malic acid, pH 3.4, 20°C, 30mg/L SO2, 13% alcohol, and strain 'standard_01'."

**🤖 AI Agent:**
> The malic acid degradation rate is 0.45 g/L per day, with an estimated 11 days to completion and a predicted diacetyl production of 1.2 mg/L.

---

**👤 You:**
> "Is there a risk of fermentation failure for a wine with 14.5% alcohol and high SO2?"

**🤖 AI Agent:**
> The failure risk score is 0.85, with High Alcohol identified as the primary risk factor.

---

**👤 You:**
> "What are the optimal conditions for strain 'acid_tolerant_v2' with 4g/L malic acid?"

**🤖 AI Agent:**
> The optimal temperature is 22°C, the target pH range is 3.2-3.5, and the maximum alcohol tolerance is 14.5%.


## ❓ FAQ

**Q: How can I predict if my fermentation will fail?**
You can use the `assess_mlf_risk` tool. It evaluates environmental inhibitors like high alcohol or SO2 levels to provide a failure risk score.

**Q: Can I compare different bacterial strains?**
Yes, the `compare_strain_performance` tool allows you to compare the degradation rates of multiple Oenococcus oeni strains under the same wine conditions.

**Q: What information is needed to estimate completion time?**
To use `predict_mlf_progression`, you need to provide the initial malic acid concentration, pH, temperature, SO2 level, alcohol content, and the specific strain ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-mlf-progression-model](https://vinkius.com/ai-agent-connect/wine-mlf-progression-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine MLF Progression Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-mlf-progression-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine MLF Progression Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-mlf-progression-model": {
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

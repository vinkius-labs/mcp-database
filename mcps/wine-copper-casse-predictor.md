# Wine Copper Casse Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-copper-casse-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [chemistry](../categories/chemistry.md)

Predict copper casse formation risk and stability in wine.

## Description
This MCP server provides specialized tools to predict the risk of copper casse (haze) formation in wine. By analyzing copper concentration, protein content, and pH, users can use `predict_casse_risk` to determine immediate risk levels. It also provides guidance on protein reduction via `calculate_bentonite_requirement`, actionable laboratory advice through `recommend_fining_trials`, and stability forecasting with `predict_shelf_life`.


## Available Tools (4)
- **predict_casse_risk**: Determines the immediate likelihood of copper casse formation in a specific wine sample
- **predict_shelf_life**: Forecasts how long the wine will remain stable before casse becomes visible
- **recommend_fining_trials**: Provides actionable guidance for laboratory trials to stabilize the wine
- **calculate_bentonite_requirement**: Estimates the amount of bentonite needed to reduce protein levels to a safe threshold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Copper Casse Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the risk of casse for a wine with 0.5 mg/L copper, 40 mg/L protein, and pH 3.3?"

**🤖 AI Agent:**
> The risk level is High due to the interaction between copper and protein at this pH level.

---

**👤 You:**
> "How much bentonite do I need for 50 mg/L protein to reach a target of 20 mg/L, with 0.4 mg/L copper?"

**🤖 AI Agent:**
> The required dosage is 1.2 grams per liter, which will achieve a 60% reduction in protein.

---

**👤 You:**
> "Predict the shelf life for a wine with 0.3 mg/L copper, 30 mg/L protein, pH 3.4, stored at 15°C with moderate light."

**🤖 AI Agent:**
> The estimated stability is 180 days with high confidence.


## ❓ FAQ

**Q: How do I know if my wine is at risk of casse?**
You can use the `predict_casse_risk` tool by providing the copper concentration, protein content, and pH of your wine sample.

**Q: Can this tool help me reduce protein levels?**
Yes, the `calculate_bentonite_requirement` tool estimates the exact dosage of bentonite needed to reach your target protein level.

**Q: How does storage temperature affect the prediction?**
The `predict_shelf_life` tool accounts for storage temperature and light exposure to forecast how many days the wine remains stable.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-copper-casse-predictor](https://vinkius.com/ai-agent-connect/wine-copper-casse-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Copper Casse Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-copper-casse-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Copper Casse Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-copper-casse-predictor": {
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

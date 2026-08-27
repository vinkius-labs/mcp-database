# Wine Brettanomyces Growth Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/wine-brettanomyces-growth-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predictive modeling for Brettanomyces yeast growth and volatile phenol production in wine.

## Description
This MCP server provides a predictive engine for winemakers to simulate the growth of Brettanomyces yeast and the subsequent production of volatile phenols like 4-EP and 4-EG. By analyzing environmental factors such as pH, alcohol, and free SO2, users can utilize `simulate_population_growth` to forecast yeast expansion. The engine also allows for estimating byproduct concentrations via `predict_phenol_production`, checking sensory limits with `check_sensory_threshold`, and determining the critical `calculate_intervention_window` to prevent wine spoilage.


## Available Tools (4)
- **calculate_intervention_window**: Identifies the optimal time to intervene before spoilage becomes irreversible
- **check_sensory_threshold**: Determines if and when the produced phenols will become detectable by human senses
- **predict_phenol_production**: Estimates the concentration of 4-EP and 4-EG produced as a byproduct of yeast activity
- **simulate_population_growth**: Predicts how the Brettanomyces population will expand over a specific timeframe


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Brettanomyces Growth Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the yeast growth for 30 days with an initial population of 100, 20g/L sugar, 25°C, 12% alcohol, pH 3.5, and 30mg/L SO2."

**🤖 AI Agent:**
> The simulated population reaches a stable density of 1500 cells/mL after 22 days, with minimal phenol production detected within this timeframe.

---

**👤 You:**
> "Will the phenol levels exceed a 4-EP threshold of 0.05 if the current growth trajectory is provided?"

**🤖 AI Agent:**
> No, the predicted 4-EP concentration is 0.03, which remains below the sensory threshold.

---

**👤 You:**
> "How much time do I have to act before the wine is spoiled based on these growth and phenol data?"

**🤖 AI Agent:**
> You have 12 days remaining before the sensory threshold for 4-EP is exceeded. The risk level is currently moderate.


## ❓ FAQ

**Q: How can I predict if my wine will develop off-flavors?**
You can use `simulate_population_growth` to model yeast expansion and then use `predict_phenol_production` to estimate the concentration of volatile phenols that cause off-flavors.

**Q: What factors influence the yeast growth simulation?**
The simulation accounts for initial population, residual sugar, temperature, alcohol, pH, and free SO2 levels.

**Q: How do I know when to intervene to prevent spoilage?**
Use the `calculate_intervention_window` tool to identify the remaining time before sensory thresholds are exceeded.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/wine-brettanomyces-growth-model](https://vinkius.com/ai-agent-connect/wine-brettanomyces-growth-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Brettanomyces Growth Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-brettanomyces-growth-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Brettanomyces Growth Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-brettanomyces-growth-model": {
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

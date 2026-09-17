# Wine Score Prediction Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-score-prediction-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predict professional critic scores and identify score drivers for wines.

## Description
This MCP server provides a predictive engine to estimate professional critic scores for wines. By analyzing varietal data, vintage conditions, winemaking methods, and chemical profiles, it calculates predicted score ranges and confidence intervals. Use `predict_wine_score` to get a score estimate, `analyze_score_drivers` to understand what influences the rating, `evaluate_improvement_opportunities` to suggest technical changes for higher scores, and `get_critic_profile` to account for specific critic preferences.


## Available Tools (4)
- **analyze_score_drivers**: Identify attributes responsible for the predicted score
- **evaluate_improvement_opportunities**: Suggest changes to increase the predicted score
- **get_critic_profile**: Retrieve historical scoring tendencies of a specific critic
- **predict_wine_score**: Predict a professional critic score for a wine based on its profile


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Score Prediction Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Predict the score for a 2018 Cabernet Sauvignon from Napa Valley with oak aging and a pH of 3.5."

**🤖 AI Agent:**
> The predicted score for this Cabernet Sauvignon is 92, with a confidence interval of 90-94.

---

**👤 You:**
> "What are the main drivers for this wine's score?"

**🤖 AI Agent:**
> The primary positive driver is the high alcohol content, while the moderate acidity is a slight negative driver for this specific profile.

---

**👤 You:**
> "How can I improve the score of my current wine profile to reach a 95?"

**🤖 AI Agent:**
> To reach a 95, consider increasing the barrel aging duration and slightly reducing the residual sugar levels.


## ❓ FAQ

**Q: How accurate are the predicted scores?**
Scores include a confidence interval based on historical data density for similar wine profiles, providing a range rather than a single fixed number.

**Q: Can I adjust predictions for specific critics?**
Yes, by using the `targetCritic` parameter in `predict_wine_score`, the model adjusts for the historical scoring tendencies and stylistic preferences of that specific critic.

**Q: What data is required for a prediction?**
You need to provide the grape variety, region, vintage year, winemaking techniques, and analytical chemical parameters like pH and alcohol content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-score-prediction-model](https://vinkius.com/en/ai-agent-connect/wine-score-prediction-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Score Prediction Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-score-prediction-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Score Prediction Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-score-prediction-model": {
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

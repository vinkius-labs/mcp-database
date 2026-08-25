# Pistachio Split Percentage Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/pistachio-split-percentage-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predict nut shell splitting, kernel quality, and harvest timing.

## Description
This MCP server provides advanced predictive modeling for pistachio growers. It uses environmental and biological data to estimate harvest outcomes. Use `estimate_split_composition` to determine the distribution of split, blank, and closed shell nuts based on growing degree days and water stress. Use `predict_harvest_dynamics` to forecast harvest dates and economic returns, and `analyze_uniformity_impact` to assess how rootstock affects crop consistency.


## Available Tools (3)
- **analyze_uniformity_impact**: 
- **estimate_split_composition**: 
- **predict_harvest_dynamics**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pistachio Split Percentage Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What percentage of my harvest will be split if I have 450 GDD, a water stress index of 0.8, a crop load of 2500, and I am growing Kerman?"

**🤖 AI Agent:**
> Based on the current parameters, your harvest is expected to be 72% split, 15% blank, and 13% closed shell.

---

**👤 You:**
> "When will my harvest happen and what is the expected return if split nuts are $4.50, blanks are $1.20, and closed shells are $2.00, with a split distribution of 70/15/15?"

**🤖 AI Agent:**
> The harvest is predicted to occur between August 15th and August 25th, with a projected economic return of $3.61 per unit.

---

**👤 You:**
> "How much is my rootstock affecting the consistency of my nut quality with 400 GDD and 0.7 water stress?"

**🤖 AI Agent:**
> Your expected uniformity score is 85, with a Low risk level for uneven nut development.


## ❓ FAQ

**Q: How accurate are the split percentage predictions?**
Predictions are based on a shell splitting model that accounts for GDD, water stress, and crop load. For the most accurate results, ensure the `waterStressIndex` and `gddSinceBloom` are updated regularly.

**Q: Can I predict my total revenue?**
Yes, by using `predict_harvest_dynamics` with your specific market prices, the tool calculates the projected economic return based on the predicted nut grade distribution.

**Q: Does the tool account for different pistachio varieties?**
Yes, the `estimate_split_composition` tool requires a variety input to apply the correct physiological growth profiles and shell thickness constants.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/pistachio-split-percentage-estimator](https://vinkius.com/ai-agent-connect/pistachio-split-percentage-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pistachio Split Percentage Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pistachio-split-percentage-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pistachio Split Percentage Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pistachio-split-percentage-estimator": {
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

# Gas Coning Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/gas-coning-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Predict gas coning in oil reservoirs and calculate critical production rates.

## Description
This MCP server provides specialized tools for reservoir engineers to manage gas coning risks. It allows for the calculation of the `calculate_critical_rate` to prevent gas breakthrough, estimation of time until gas reaches the wellbore using `predict_breakthrough`, and simulation of gas-oil ratio trends via `simulate_gor_evolution`. Additionally, it helps optimize well design through `evaluate_well_placement` to minimize coning risk based on reservoir anisotropy and thickness.


## Available Tools (4)
- **calculate_critical_rate**: Determines the maximum safe production rate to prevent or delay gas coning
- **evaluate_well_placement**: Analyzes how different well completions affect coning risk
- **predict_breakthrough**: Estimates when gas will first reach the wellbore
- **simulate_gor_evolution**: Models the progression of the gas-oil ratio over a production lifecycle


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gas Coning Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the critical production rate for a reservoir with 100m horizontal permeability, 20m vertical permeability, 50m oil thickness, 30m gas cap, and 10m perforation depth?"

**🤖 AI Agent:**
> The calculated critical rate is 450.5 bbl/day with an anisotropy ratio of 0.2.

---

**👤 You:**
> "If I produce at 500 bbl/day with a critical rate of 450 bbl/day, when will gas breakthrough occur?"

**🤖 AI Agent:**
> Breakthrough is expected in 120 days with an Immediate severity level.

---

**👤 You:**
> "Show me the GOR evolution for a production rate of 400 bbl/day and a critical rate of 450 bbl/day over 10 steps."

**🤖 AI Agent:**
> The GOR remains stable at 15.0 for all 10 time steps as the production rate is below the critical rate.


## ❓ FAQ

**Q: How do I prevent gas coning?**
You can use `calculate_critical_rate` to find the maximum safe production rate that minimizes gas coning risk.

**Q: Can I predict when gas will reach my well?**
Yes, the `predict_breakthrough` tool estimates the time until gas reaches the wellbore based on your production rate and reservoir properties.

**Q: How does well placement affect coning?**
The `evaluate_well_placement` tool analyzes how perforation intervals and gas cap thickness influence the risk score and provides a recommended offset.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/gas-coning-model](https://vinkius.com/en/ai-agent-connect/gas-coning-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gas Coning Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gas-coning-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gas Coning Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gas-coning-model": {
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

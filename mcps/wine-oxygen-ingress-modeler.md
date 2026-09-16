# Wine Oxygen Ingress Modeler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-oxygen-ingress-modeler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Predictive modeling for oxygen ingress through screw cap liners to assess wine stability.

## Description
This MCP server provides specialized tools for enologists and winemakers to model oxygen ingress through various screw cap liner types. By analyzing liner permeability and storage conditions, users can predict oxygen ingress rates and assess the risk of reductive development. The server includes tools like `calculate_ingress_rate` to determine daily oxygen entry, `assess_reductive_risk` to evaluate potential off-odors, `predict_evolution_timeline` for long-term dissolved oxygen projections, and `simulate_storage_impact` for a comprehensive end-state analysis of a bottle after storage.


## Available Tools (4)
- **assess_reductive_risk**: Evaluates if the wine is at risk of developing reductive off-odors due to lack of oxygen
- **calculate_ingress_rate**: Determines how much oxygen is entering the bottle per unit of time
- **predict_evolution_timeline**: Projects the change in dissolved oxygen over a specific duration
- **simulate_storage_impact**: A high-level tool to combine all factors to determine the end-state of a bottle after a period of storage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Oxygen Ingress Modeler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the daily oxygen ingress for a Saranex liner with an OTR of 0.5, a surface area of 5, and a temperature of 15 degrees Celsius."

**🤖 AI Agent:**
> The daily oxygen ingress rate for the Saranex liner under these conditions is 0.0025 mg/L per day.

---

**👤 You:**
> "What is the risk of reductive development if the ingress rate is 0.01 and the wine's reductive capacity is 0.05 with an initial DO of 0.2?"

**🤖 AI Agent:**
> The risk level is High, with a probability score of 0.85, because the ingress rate is significantly lower than the wine's reductive capacity.

---

**👤 You:**
> "Predict the dissolved oxygen evolution over 180 days for a bottle with 0.3 initial DO, 0.02 ingress rate, and 0.5L headspace."

**🤖 AI Agent:**
> After 180 days, the projected total dissolved oxygen level is 0.372 mg/L.


## ❓ FAQ

**Q: How accurate are the oxygen ingress predictions?**
Predictions are based on physical permeation models using the provided OTR specification and storage temperature. For precise results, ensure the `otrSpecification` matches the specific liner material used.

**Q: Can I model different liner materials?**
Yes, you can use `calculate_ingress_rate` or `simulate_storage_impact` with standard liner types such as Saranex, tin/Saran, or STELVIN.

**Q: What is the purpose of the reductive risk assessment?**
The `assess_reductive_risk` tool helps identify if a wine might develop sulfur-based off-odors due to insufficient oxygen ingress relative to its reductive capacity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-oxygen-ingress-modeler](https://vinkius.com/en/ai-agent-connect/wine-oxygen-ingress-modeler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Oxygen Ingress Modeler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-oxygen-ingress-modeler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Oxygen Ingress Modeler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-oxygen-ingress-modeler": {
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

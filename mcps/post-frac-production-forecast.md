# Post-Frac Production Forecast MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/post-frac-production-forecast)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Predict well production lifecycles, flow regime transitions, and EUR following hydraulic fracturing.

## Description
This MCP server provides specialized reservoir engineering tools to forecast production after hydraulic fracturing. It allows AI agents to model the transition from transient flow to boundary-dominated flow and calculate critical metrics like initial production rates and Estimated Ultimate Recovery (EUR). Use `calculate_initial_rate` to determine peak production, `predict_flow_regime_transition` to identify when pressure transients hit reservoir boundaries, `generate_decline_curve` for time-specific rate predictions, and `calculate_eur` to estimate the total lifetime hydrocarbon recovery.


## Available Tools (4)
- **calculate_eur**: Estimates the total lifetime production of the well
- **calculate_initial_rate**: Determines the peak production rate immediately following the completion of the hydraulic fracturing process
- **generate_decline_curve**: Provides the predicted production rate for a specific point in time based on the well's lifecycle
- **predict_flow_regime_transition**: Predicts when a well will transition from transient flow to boundary-dominated flow


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Post-Frac Production Forecast** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the estimated initial production rate for a reservoir with 50mD permeability, 100m fracture length, 10mD/ft conductivity, and 3000 psi pressure?"

**🤖 AI Agent:**
> The initial production rate is 1,250 bbl/d.

---

**👤 You:**
> "When will the well transition to boundary-dominated flow with a fracture volume of 500,000 cubic feet, porosity of 0.15, and fluid viscosity of 0.5 cP?"

**🤖 AI Agent:**
> The transition to boundary-dominated flow is predicted to occur at 450 days.

---

**👤 You:**
> "Calculate the EUR for a well with an IP of 1000 bbl/d, a decline exponent of 0.5, and an economic limit of 50 bbl/d."

**🤖 AI Agent:**
> The Estimated Ultimate Recovery (EUR) is 150,000 barrels with an estimated life span of 1,200 days.


## ❓ FAQ

**Q: How does this tool handle different flow regimes?**
The tool uses `predict_flow_regime_transition` to identify when a well moves from transient flow to boundary-dominated flow, allowing for accurate decline curve modeling.

**Q: Can I estimate the total lifetime production of a well?**
Yes, you can use the `calculate_eur` tool to estimate the Estimated Ultimate Recovery based on the initial production rate and the economic limit.

**Q: What inputs are required for the initial rate calculation?**
To use `calculate_initial_rate`, you need to provide reservoir permeability, fracture length, fracture conductivity, and the initial reservoir pressure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/post-frac-production-forecast](https://vinkius.com/ai-agent-connect/post-frac-production-forecast)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Post-Frac Production Forecast** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `post-frac-production-forecast` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Post-Frac Production Forecast** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "post-frac-production-forecast": {
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

# Sand Production Prediction MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/sand-production-prediction)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Predicts sand production potential by analyzing formation stability and fluid dynamics.

## Description
This MCP server provides critical tools for reservoir engineers to predict sand production risks. By analyzing formation strength, in-situ stress, and drawdown, users can determine the `get_critical_drawdown` threshold. The server also identifies the `analyze_failure_zone` extent, estimates the `predict_sand_volume` produced, and provides a full `assess_operational_stability` check to ensure wellbore integrity.


## Available Tools (4)
- **get_critical_drawdown**: Determines the maximum pressure reduction allowed before sand production is predicted to begin
- **analyze_failure_zone**: Identifies the extent of the area around the wellbore susceptible to sand liberation
- **assess_operational_stability**: Provides a comprehensive safety check by combining mechanical, hydraulic, and fluid composition data
- **predict_sand_volume**: Estimates the amount of sand expected to be produced given specific flow and stability conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sand Production Prediction** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the critical drawdown for a rock with 50 MPa strength and 30 MPa in-situ stress?"

**🤖 AI Agent:**
> The critical drawdown is 20 MPa, and the risk level is Moderate.

---

**👤 You:**
> "Calculate the sand volume for a failure radius of 0.5m, fluid velocity of 2 m/s, and a water cut of 0.2."

**🤖 AI Agent:**
> The expected sand volume is 12.5 kg with a Low transport risk.

---

**👤 You:**
> "Is my operation stable with 40 MPa strength, 35 MPa stress, 2 MPa drawdown, 1 m/s velocity, and 0.1 water cut?"

**🤖 AI Agent:**
> Yes, the operation is stable with a safety margin of 3 MPa. Conditions are safe.


## ❓ FAQ

**Q: How do I know if my well is at risk of sand production?**
You can use the `assess_operational_stability` tool to perform a comprehensive safety check that evaluates your current drawdown against the formation's strength.

**Q: Can I predict the volume of sand that will be produced?**
Yes, the `predict_sand_volume` tool estimates the expected sand mass based on the failure zone radius, fluid velocity, and water cut.

**Q: What is the critical drawdown?**
The critical drawdown is the maximum allowable pressure reduction before the formation becomes unstable. You can calculate this using `get_critical_drawdown`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/sand-production-prediction](https://vinkius.com/en/ai-agent-connect/sand-production-prediction)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sand Production Prediction** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sand-production-prediction` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sand Production Prediction** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sand-production-prediction": {
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

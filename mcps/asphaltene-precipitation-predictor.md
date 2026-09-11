# Asphaltene Precipitation Predictor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/asphaltene-precipitation-predictor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Predicts asphaltene precipitation onset, flocculation, and deposition risks in crude oil systems.

## Description
This MCP server provides specialized thermodynamic modeling to predict asphaltene stability in crude oil. It allows AI agents to calculate the Onset of Precipitation Pressure (OPP) using `get_onset_pressure`, determine aggregation states via `predict_flocculation_state`, assess the impact of gas injection with `evaluate_gas_injection_impact`, and evaluate mixing risks using `assess_commingling_risk`. It is designed to help reservoir engineers and production specialists mitigate deposition risks caused by pressure drops, temperature changes, or fluid commingling.


## Available Tools (4)
- **get_onset_pressure**: Identifies the specific pressure at which asphaltene precipitation begins for a given oil system
- **evaluate_gas_injection_impact**: Predicts how the addition of a specific gas will change the stability of the asphaltenes
- **predict_flocculation_state**: Determines if the current fluid state will cause asphaltenes to aggregate into clusters
- **assess_commingling_risk**: Evaluates the risk of precipitation when two different crude oils are mixed


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Asphaltene Precipitation Predictor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the onset pressure for an oil with these molar fractions: {"C1": 0.1, "C2": 0.2, "Asphaltenes": 0.7} at 80 degrees Celsius with solubility parameters {"a1": 1.5, "a2": 0.5}?"

**🤖 AI Agent:**
> The onset pressure for this oil system is 250.5 bar with a stability margin of 15.2 bar.

---

**👤 You:**
> "Will injecting methane at a 0.15 ratio into this oil composition {"C1": 0.5, "C2": 0.5} at 50 degrees Celsius cause precipitation?"

**🤖 AI Agent:**
> Yes, the injection will cause precipitation with a stability change of 0.45.

---

**👤 You:**
> "What is the flocculation risk for an oil with density 0.85 and viscosity 5.2 at 40 bar and 60 degrees Celsius?"

**🤖 AI Agent:**
> The current state is 'Aggregating' with a flocculation index of 0.65 and a High risk level.


## ❓ FAQ

**Q: What is the Onset of Precipitation Pressure (OPP)?**
OPP is the specific pressure at which asphaltenes begin to form solid aggregates. You can find this value using the `get_onset_pressure` tool.

**Q: How does gas injection affect asphaltene stability?**
Injecting gases like methane or CO2 can reduce the solubility of asphaltenes. The `evaluate_gas_injection_impact` tool predicts the resulting stability change.

**Q: Can I predict risks when mixing two different oils?**
Yes, the `assess_commingling_risk` tool evaluates the compatibility and precipitation probability when mixing different crude oil compositions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/asphaltene-precipitation-predictor](https://vinkius.com/en/ai-agent-connect/asphaltene-precipitation-predictor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Asphaltene Precipitation Predictor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `asphaltene-precipitation-predictor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Asphaltene Precipitation Predictor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "asphaltene-precipitation-predictor": {
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

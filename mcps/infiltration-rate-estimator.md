# Infiltration Rate Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/infiltration-rate-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environmental-science](../categories/environmental-science.md)

Estimates soil infiltration rates and runoff risks using physical soil properties.

## Description
This MCP server provides specialized tools for hydrological analysis. It calculates the immediate capacity of soil to absorb water using `get_initial_infiltration_rate`, determines total water volume via `get_cumulative_infiltration`, and assesses surface runoff likelihood with `estimate_runoff_risk`. It also evaluates how soil structure and density interact through `analyze_soil_structure_impact` to determine porosity and stability.


## Available Tools (4)
- **analyze_soil_structure_impact**: Evaluates how soil structure and bulk density interact to affect infiltration potential
- **estimate_runoff_risk**: Assesses the likelihood of surface runoff occurring during a rain event
- **get_cumulative_infiltration**: Determines the total volume of water absorbed by the soil over a specific duration
- **get_initial_infiltration_rate**: Calculates the immediate capacity of the soil to absorb water at the start of a rain event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Infiltration Rate Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the initial infiltration rate for sandy soil with a bulk density of 1.2 and a bare surface?"

**🤖 AI Agent:**
> The initial infiltration rate for the sandy soil is 25.5 mm/hr with an influence factor of 0.8 due to the bare surface condition.

---

**👤 You:**
> "Calculate the total volume of water infiltrated over 2 hours if the initial rate is 30 mm/hr and the final rate is 10 mm/hr using the Horton model."

**🤖 AI Agent:**
> The total volume of water infiltrated over 2 hours is 42.4 mm.

---

**👤 You:**
> "Assess the runoff risk if the rainfall intensity is 50 mm/hr, current infiltration is 30 mm/hr, moisture is 0.8, and vegetation cover is 10%."

**🤖 AI Agent:**
> The runoff risk is extreme with a probability of 0.92, primarily driven by high soil saturation and low vegetation cover.


## ❓ FAQ

**Q: What models are used for infiltration calculations?**
The server supports both Green-Ampt and Horton infiltration models to calculate cumulative water absorption.

**Q: How does soil texture affect the results?**
Soil texture is a primary input for `get_initial_infiltration_rate`, as sand, silt, and clay have different pore size distributions that dictate water entry speed.

**Q: Can I assess runoff risk for a specific rain event?**
Yes, by using `estimate_runoff_risk` with current infiltration rates, rainfall intensity, and vegetation cover, you can determine the probability of surface runoff.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/infiltration-rate-estimator](https://vinkius.com/ai-agent-connect/infiltration-rate-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Infiltration Rate Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `infiltration-rate-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Infiltration Rate Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "infiltration-rate-estimator": {
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

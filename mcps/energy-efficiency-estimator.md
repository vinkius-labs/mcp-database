# Energy Efficiency Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/energy-efficiency-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [real-estate](../categories/real-estate.md)

Classify your home's energy performance (A-E) and pinpoint specific improvements using building envelope metrics.

## Description
## 🏠 Residential Energy Efficiency Assessment

The cost of maintaining an inefficient home is high, stemming from continuous thermal losses and poor material performance. Before investing in major renovations, understanding the structural weakness points of your building envelope is critical.

**The Problem:** Standard energy audits are often broad or expensive to execute. Homeowners need a quick, precise assessment that pinpoints *why* their home loses energy--is it the walls, the windows, or the roof? They require an actionable score and prioritized fix list.

**The Mechanism (How It Works):** This service analyzes key building envelope properties (like U-values, wall thickness, and window SHGC) to calculate a Thermal Performance Index. Our system uses three specialized tools:
1. `query_structure_thermal_score`: Calculates the raw thermal index based on overall component metrics.
2. `query_orientation_bias`: Adjusts the score by assessing passive solar gain/loss based on your home's cardinal orientation (e.g., South-facing vs. North-facing).
3. `query_improvement_recommendations`: Takes the resulting A-E classification and provides a prioritized list of actionable upgrades, telling you exactly what to fix.

**The Advantage:** You receive an immediate, quantified energy rating (A-E) and a clear roadmap for improvement--a true blueprint for efficiency that prevents overspending on ineffective fixes. It connects raw structural data directly to measurable savings.


## Available Tools (3)
- **query_orientation_bias**: Determine the passive energy benefit or detriment of a building orientation
- **query_improvement_recommendations**: Get prioritized improvement recommendations for building envelope deficiencies
- **query_structure_thermal_score**: Calculate the thermal performance index for a residential structure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Energy Efficiency Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a 150 sqM house in the US with South-West exposure. The walls are 300mm thick, and I want to know my base thermal score."

**🤖 AI Agent:**
> First, run `query_structure_thermal_score` with the provided metrics. Then, use `query_orientation_bias` to factor in the South-West exposure for US climate zones. Finally, pass the resulting score and component data into `query_improvement_recommendations`.

---

**👤 You:**
> "My current rating is C (Average). I need to improve the glazing and roof. What should I do?"

**🤖 AI Agent:**
> Use `query_improvement_recommendations`. You must input your current classification ('C') and a detailed component metrics object, specifically noting the glazing SHGC and insulation levels. The tool will provide prioritized steps.

---

**👤 You:**
> "I live in Europe. My house faces North, but I suspect the U-value for my roof is too high."

**🤖 AI Agent:**
> Run `query_orientation_bias` specifying 'North' and 'Europe'. Next, use `query_structure_thermal_score`, ensuring the roof U-value is accurately input. This combined data will help determine if your North exposure needs specific compensation.


## ❓ FAQ

**Q: What inputs are needed to get the initial score?**
The core metrics include total heated area, wall thickness, and combined U-values. The `query_structure_thermal_score` tool uses these inputs to generate the raw thermal index.

**Q: Does my home's direction matter for the score?**
Yes. The `query_orientation_bias` tool accounts for passive solar gain and wind loads (e.g., South-East vs. North). This factor modifies the score to give a regionally accurate assessment.

**Q: How do I know what to fix after the rating?**
After receiving your A-E classification, use the `query_improvement_recommendations` tool. It analyzes component weaknesses and provides a prioritized list of actionable upgrades (e.g., upgrading glazing or improving roof insulation).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/energy-efficiency-estimator](https://vinkius.com/mcp/energy-efficiency-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Energy Efficiency Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `energy-efficiency-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Energy Efficiency Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "energy-efficiency-estimator": {
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

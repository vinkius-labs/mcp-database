# Tailings Dam Safety Assessment MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/tailings-dam-safety-assessment)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Professional engineering tool for evaluating tailings dam stability, seismic resilience, and flood risk.

## Description
This MCP server provides specialized engineering tools to assess the structural integrity of tailings storage facilities. It allows AI agents to perform critical safety calculations including `analyze_slope_stability` to check resistance against sliding, `evaluate_seismic_resilience` to assess liquefaction risks during earthquakes, and `simulate_flood_impact` to predict overtopping risks. Finally, it uses `classify_dam_risk` to assign formal risk categories based on technical metrics and consequence tiers.


## Available Tools (4)
- **analyze_slope_stability**: Determine if the current dam geometry and material properties provide sufficient resistance against sliding
- **classify_dam_risk**: Assign a formal risk category to the facility based on technical analyses
- **evaluate_seismic_resilience**: Assess how the dam reacts to earthquake-induced accelerations and the risk of liquefaction
- **simulate_flood_impact**: Predict the risk of overtopping and internal erosion during extreme precipitation or inflow events


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tailings Dam Safety Assessment** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the slope stability for a dam with height 50m, crest width 10m, slope angle 25 degrees, and slope length 100m, using cohesion 20, friction angle 30, and unit weight 18, with a phreatic surface height of 5m and pore pressure 2."

**🤖 AI Agent:**
> The factor of safety is 1.65, and the stability status is Stable.

---

**👤 You:**
> "What is the risk of overtopping if a flood with an inflow rate of 500 m3/s for 2 hours hits a dam with 5m of freeboard?"

**🤖 AI Agent:**
> The overtopping risk is Low, and the erosion potential is minimal.

---

**👤 You:**
> "Classify the risk for a dam with a factor of safety of 1.05 and a High consequence category."

**🤖 AI Agent:**
> The risk level is Extreme, with an urgency rating of High.


## ❓ FAQ

**Q: What can I calculate with this tool?**
You can calculate the factor of safety for slope stability, assess seismic resilience and liquefaction risk, simulate flood impacts, and classify the overall dam risk level.

**Q: How does the tool handle seismic events?**
The `evaluate_seismic_resilience` tool evaluates how earthquake-induced accelerations affect the dam, specifically looking at the risk of liquefaction in saturated tailings.

**Q: Can I predict overtopping during a flood?**
Yes, by using `simulate_flood_impact`, you can predict overtopping risks and erosion potential based on flood volume and available freeboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/tailings-dam-safety-assessment](https://vinkius.com/ai-agent-connect/tailings-dam-safety-assessment)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tailings Dam Safety Assessment** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tailings-dam-safety-assessment` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tailings Dam Safety Assessment** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tailings-dam-safety-assessment": {
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

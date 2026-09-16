# Bottom Contour Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bottom-contour-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design](../categories/design.md)

Analyze surfboard hydrodynamic performance including speed, lift, and maneuverability.

## Description
This MCP server provides specialized hydrodynamic analysis for surfboard design. It allows AI agents to evaluate how bottom contours, such as single or double concaves, impact performance. Users can use `analyze_contour_performance` to measure speed and lift, `evaluate_transition_turbulence` to predict flow disruption between shapes, `calculate_lift_profile` to determine planing thresholds, and `optimize_maneuverability` to receive design suggestions for better rail-to-rail transitions.


## Available Tools (4)
- **optimize_maneuverability**: Suggests adjustments to the board's bottom to improve turning agility
- **calculate_lift_profile**: Determines how much upward pressure the board will generate at various speeds
- **evaluate_transition_turbulence**: Predicts the disruption in water flow when moving between different contour shapes
- **analyze_contour_performance**: Evaluates the primary hydrodynamic performance metrics for a specific bottom configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bottom Contour Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze a single concave configuration with a V-panel and 5mm channels."

**🤖 AI Agent:**
> The analysis shows a high speed score and moderate lift, with a stability rating of Medium.

---

**👤 You:**
> "What happens if I transition from a single concave to a double concave over 10cm?"

**🤖 AI Agent:**
> The transition results in a Turbulent flow level with a flow disruption score of 0.65. A Gradual transition is recommended.

---

**👤 You:**
> "Calculate the lift for a double concave at a speed of 15 knots with 0.8 channel efficiency."

**🤖 AI Agent:**
> The total lift is 45.2 units with a planing threshold of 12 knots and a center-focused pressure distribution.


## ❓ FAQ

**Q: How can I improve my board's turning agility?**
You can use the `optimize_maneuverability` tool to receive specific design suggestions, such as adding a V-panel to improve rail-to-rail transitions.

**Q: Can I predict turbulence during contour transitions?**
Yes, the `evaluate_transition_turbulence` tool predicts flow disruption and turbulence levels when moving between different concave shapes.

**Q: What metrics are included in the performance analysis?**
The `analyze_contour_performance` tool provides speed scores, lift scores, maneuverability scores, and a stability rating.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bottom-contour-analysis](https://vinkius.com/en/ai-agent-connect/bottom-contour-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bottom Contour Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bottom-contour-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bottom Contour Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bottom-contour-analysis": {
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

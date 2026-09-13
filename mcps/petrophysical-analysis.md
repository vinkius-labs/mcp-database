# Petrophysical Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/petrophysical-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [energy](../categories/energy.md)

Perform detailed petrophysical evaluations including Archie parameter calculation and water saturation modeling.

## Description
This MCP server provides specialized tools for reservoir rock evaluation. It allows AI agents to calculate fundamental rock constants using `calculate_archie_parameters`, determine water saturation levels with `compute_water_saturation`, predict vertical saturation distributions via `generate_saturation_height_profile`, and evaluate complex reservoirs using `analyze_dual_porosity_system`.


## Available Tools (4)
- **calculate_archie_parameters**: Determines the fundamental rock constants required for electrical saturation modeling
- **analyze_dual_porosity_system**: Evaluates saturation in complex reservoirs containing both matrix and fracture porosity
- **compute_water_saturation**: Calculates the water saturation level for a specific depth or interval
- **generate_saturation_height_profile**: Predicts the vertical distribution of water saturation within a reservoir column


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Petrophysical Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the Archie constants for this resistivity data: [{'res': 10, 'sw': 0.2}, {'res': 15, 'sw': 0.15}] and porosity data: [{'phi': 0.12}, {'phi': 0.15}]."

**🤖 AI Agent:**
> { "a": 1.0, "m": 2.0, "n": 2.0 }

---

**👤 You:**
> "What is the water saturation if formation resistivity is 20, water resistivity is 0.05, porosity is 0.15, and Archie constants are {'a': 1, 'm': 2, 'n': 2}?"

**🤖 AI Agent:**
> { "sw": 0.25, "swSquared": 0.0625 }

---

**👤 You:**
> "Predict the saturation profile for a reservoir with permeability 100, porosity 0.2, and capillary pressure data: [{'pc': 5}, {'pc': 10}] at heights [1, 2]."

**🤖 AI Agent:**
> [{"height": 1, "sw": 0.4}, {"height": 2, "sw": 0.3}]


## ❓ FAQ

**Q: How do I calculate Archie constants?**
You can use the `calculate_archie_parameters` tool by providing resistivity and porosity data from core samples.

**Q: Can this tool handle clay effects?**
Yes, the `compute_water_saturation` tool includes an optional clay correction parameter to account for conductive clay minerals.

**Q: Does it support dual-porosity reservoirs?**
Yes, the `analyze_dual_porosity_system` tool is specifically designed to evaluate saturation in reservoirs with both matrix and fracture porosity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/petrophysical-analysis](https://vinkius.com/en/ai-agent-connect/petrophysical-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Petrophysical Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `petrophysical-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Petrophysical Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "petrophysical-analysis": {
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

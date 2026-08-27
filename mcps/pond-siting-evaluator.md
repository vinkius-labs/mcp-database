# Pond Siting Evaluator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/pond-siting-evaluator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Analyze pond site suitability using hydrologic and geological data.

## Description
This MCP server provides specialized tools for evaluating the suitability of pond sites. It uses NRCS design criteria to calculate expected runoff volume via `evaluate_runoff_potential`, determine usable storage and depth constraints with `calculate_pond_capacity`, and estimate earthwork needs using `estimate_construction_requirements`. Additionally, it assesses long-term water stability and spillway safety through `assess_site_reliability`.


## Available Tools (4)
- **evaluate_runoff_potential**: Determines how much water the watershed will contribute to the pond
- **assess_site_reliability**: Evaluates if the pond will remain functional and safe over time
- **calculate_pond_capacity**: Determines the usable volume and structural constraints of the pond
- **estimate_construction_requirements**: Calculates the volume of material needed to build the pond's containment structure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pond Siting Evaluator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the runoff for a 50 acre watershed with a 0.3 runoff coefficient and 5 inches of rain."

**🤖 AI Agent:**
> The expected runoff volume is 7.5 acre-feet.

---

**👤 You:**
> "What is the usable storage for a 2 acre pond with 15 feet of depth to bedrock and a 10% sediment factor?"

**🤖 AI Agent:**
> The usable storage is 27 acre-feet.

---

**👤 You:**
> "Estimate the cost for a containment structure with a 500 foot perimeter, 5 foot height, and 2:1 slope."

**🤖 AI Agent:**
> The estimated construction cost is $12,500.


## ❓ FAQ

**Q: What data is required for runoff calculation?**
To use `evaluate_runoff_potential`, you need the watershed area in acres, the runoff coefficient, and the rainfall depth in inches.

**Q: How does soil type affect reliability?**
Soil type is critical for `assess_site_reliability`. Sandy soils increase seepage losses, which lowers the reliability score compared to clay or silt.

**Q: Can I estimate construction costs?**
Yes, the `estimate_construction_requirements` tool provides an estimated cost in USD based on the required embankment volume.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/pond-siting-evaluator](https://vinkius.com/ai-agent-connect/pond-siting-evaluator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pond Siting Evaluator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pond-siting-evaluator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pond Siting Evaluator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pond-siting-evaluator": {
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

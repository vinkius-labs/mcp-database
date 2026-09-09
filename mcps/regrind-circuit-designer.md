# Regrind Circuit Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/regrind-circuit-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design optimal fine grinding circuits by selecting mill types and calculating power and media wear.

## Description
This MCP server provides specialized engineering tools for designing regrind circuits in mineral processing. It allows AI agents to determine the most suitable grinding technology--such as `calculate_mill_selection` for choosing between IsaMill, Vertimill, or SMD--and calculate critical operational parameters. Users can use `estimate_power_requirements` to find energy needs, `predict_media_consumption` to forecast media wear costs, and `evaluate_circuit_efficiency` to assess the technical viability of a design based on target liberation and throughput.


## Available Tools (4)
- **calculate_mill_selection**: Determines the most suitable grinding technology for a specific grinding task
- **estimate_power_requirements**: Calculates the energy needed to achieve the target liberation
- **evaluate_circuit_efficiency**: Provides a high-level summary of the design's viability
- **predict_media_consumption**: Forecasts the volume of grinding media lost to wear during operation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Regrind Circuit Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which mill should I use for a throughput of 500 tph and a target liberation of 20 microns with an ore hardness of 15?"

**🤖 AI Agent:**
> The most suitable mill for these parameters is the IsaMill.

---

**👤 You:**
> "Calculate the power needed for an SMD mill processing 300 tph at 10 microns with hardness 12."

**🤖 AI Agent:**
> The total power required for the SMD mill is 4500 kW, with a power consumption of 15 kW per tonne.

---

**👤 You:**
> "Predict the media wear for a Vertimill with 400 tph throughput and an ore abrasiveness of 0.5."

**🤖 AI Agent:**
> The predicted media consumption rate is 0.02 kg/t, with an estimated annual cost of $12,000.


## ❓ FAQ

**Q: How do I select the right mill for my ore?**
You can use the `calculate_mill_selection` tool, providing the target liberation, throughput, and ore hardness to find the optimal mill type.

**Q: Can I estimate the cost of grinding media?**
Yes, the `predict_media_consumption` tool provides both the consumption rate and an annual cost estimate based on your specific ore properties.

**Q: What parameters are needed for power calculations?**
To use `estimate_power_requirements`, you need to provide the throughput, target liberation, ore hardness, and the specific mill type being used.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/regrind-circuit-designer](https://vinkius.com/ai-agent-connect/regrind-circuit-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Regrind Circuit Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `regrind-circuit-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Regrind Circuit Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "regrind-circuit-designer": {
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

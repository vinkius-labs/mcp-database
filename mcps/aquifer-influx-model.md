# Aquifer Influx Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/aquifer-influx-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Simulates water influx from aquifers into reservoirs using advanced hydraulic models.

## Description
This MCP server provides specialized tools for reservoir engineering to model how water from an adjacent aquifer enters a reservoir. It supports both edge-water and bottom-water drive mechanisms using the van Everdingen-Hurst and Fetkovich mathematical models. Use `get_influx_rate` to find instantaneous flow, `get_cumulative_influx` for total volume, `get_pressure_support_analysis` to evaluate pressure maintenance, and `compare_drive_mechanisms` to evaluate different aquifer configurations.


## Available Tools (4)
- **compare_drive_mechanisms**: Compares the influx performance between edge-water and bottom-water configurations
- **get_cumulative_influx**: Determines the total volume of water that has moved into the reservoir over a period
- **get_influx_rate**: Calculates the instantaneous rate of water entering the reservoir at a specific time
- **get_pressure_support_analysis**: Evaluates how effectively the aquifer is maintaining reservoir pressure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aquifer Influx Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the instantaneous water influx rate for an aquifer with size 500, permeability 150, pressure differential 200, time 10, using edge-water drive and the fetkovich model?"

**🤖 AI Agent:**
> The instantaneous water influx rate is 45.2 cubic meters per day with a pressure support ratio of 0.12.

---

**👤 You:**
> "Calculate the total volume of water that has entered the reservoir after 50 units of time using the van-everdingen-hurst model with an aquifer size of 1000, permeability 200, pressure differential 300, and bottom-water drive."

**🤖 AI Agent:**
> The total cumulative influx is 1250.5 cubic meters, with an average rate of 25.01 cubic meters per unit of time.

---

**👤 You:**
> "How effective is the pressure support for an aquifer with size 800, permeability 100, pressure differential 150, time 20, using edge-water drive and the fetkovich model?"

**🤖 AI Agent:**
> The pressure support effectiveness is 0.65, with an estimated pressure drop of 12.4 units.


## ❓ FAQ

**Q: Which mathematical models are supported?**
The server supports the van-everdingen-hurst and fetkovich models for calculating influx dynamics.

**Q: Can I compare different drive types?**
Yes, you can use `compare_drive_mechanisms` to see the difference in performance between edge-water and bottom-water drives.

**Q: What inputs are required for influx calculations?**
You need to provide aquifer size, permeability, pressure differential, time, drive type, and the chosen model type.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/aquifer-influx-model](https://vinkius.com/en/ai-agent-connect/aquifer-influx-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aquifer Influx Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aquifer-influx-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aquifer Influx Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aquifer-influx-model": {
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

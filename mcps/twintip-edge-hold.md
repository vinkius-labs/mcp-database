# twintip-edge-hold MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/twintip-edge-hold)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [simulation](../categories/simulation.md)

Simulate hydrodynamic performance, grip force, and pop potential for twin-tip boards.

## Description
This MCP server provides specialized hydrodynamic simulation tools for twin-tip wakeboard and surfboard designs. It allows AI agents to calculate critical performance metrics including `calculate_grip_force` to determine lateral stability, `calculate_max_edging_angle` to find the washout threshold, and `calculate_pop_potential` to evaluate vertical launch capability. Users can also generate a complete performance profile using `analyze_performance_summary` to understand how fin configuration, rocker type, and board geometry interact under specific riding speeds.


## Available Tools (4)
- **analyze_performance_summary**: Provides a holistic view of how a specific setup will behave across all three performance metrics
- **calculate_grip_force**: Determines the lateral force (grip) the board's edge provides against the water
- **calculate_max_edging_angle**: Finds the steepest angle a rider can tilt the board before the edge loses grip
- **calculate_pop_potential**: Evaluates the explosive vertical launch capability of the board


## 💬 Prompt Examples

Here are some examples of how you can interact with the **twintip-edge-hold** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the grip force for a board with 5cm fins, quad configuration, 40cm width, and 5m/s speed with a concave."

**🤖 AI Agent:**
> The calculated grip force is 142.5 N with a high stability rating.

---

**👤 You:**
> "What is the maximum edging angle for a continuous rocker board with 4cm fins and 4m/s speed?"

**🤖 AI Agent:**
> The maximum edging angle is 28.4 degrees.

---

**👤 You:**
> "Evaluate the pop potential for a three-stage rocker board with a concave at 6m/s speed."

**🤖 AI Agent:**
> The pop score is 8.5 with a lift efficiency of 0.78.


## ❓ FAQ

**Q: What metrics can I calculate?**
You can calculate grip force, maximum edging angle, pop potential, and a complete performance summary.

**Q: How does fin configuration affect the results?**
The `calculate_grip_force` tool uses the fin configuration (single, dual, or quad) to determine how much lateral stability the board provides.

**Q: Can I simulate different rocker profiles?**
Yes, you can specify 'continuous' or 'three-stage' rocker types to see how they impact edging angles and pop potential.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/twintip-edge-hold](https://vinkius.com/ai-agent-connect/twintip-edge-hold)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **twintip-edge-hold** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `twintip-edge-hold` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **twintip-edge-hold** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "twintip-edge-hold": {
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

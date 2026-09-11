# Choke Performance Model MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/choke-performance-model)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculates fluid flow rates and pressure regimes through wellhead chokes.

## Description
This MCP server provides specialized calculation engines for determining fluid flow rates and pressure regimes through wellhead chokes. It models both critical and subcritical flow behaviors using physics-based equations. Users can determine the flow regime using `calculate_flow_regime`, calculate specific flow rates with `calculate_flow_rate`, determine pressure drops via `calculate_pressure_drop`, and evaluate orifice utilization with `analyze_choke_efficiency`. It accounts for fluid compressibility and gas-liquid ratios to ensure accurate modeling of multiphase fluid streams.


## Available Tools (4)
- **analyze_choke_efficiency**: Evaluates how effectively the choke size and current pressures are utilizing the orifice capacity
- **calculate_flow_rate**: Calculates the volume or mass flow rate of the fluid passing through the choke
- **calculate_flow_regime**: Determines whether the current wellhead conditions result in critical or subcritical flow
- **calculate_pressure_drop**: Determines the magnitude of the pressure reduction across the choke


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Choke Performance Model** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the flow regime for an upstream pressure of 2000 psi and downstream pressure of 500 psi with a compressibility of 0.8 and GLR of 10?"

**🤖 AI Agent:**
> The current conditions result in critical flow.

---

**👤 You:**
> "Calculate the pressure drop if upstream pressure is 1500 psi and downstream pressure is 1200 psi."

**🤖 AI Agent:**
> The pressure drop across the choke is 300 psi.

---

**👤 You:**
> "What is the flow rate for a choke size of 15, upstream pressure of 3000 psi, downstream pressure of 1000 psi, temperature of 520 K, compressibility of 0.7, and GLR of 5?"

**🤖 AI Agent:**
> The calculated flow rate is 450.5 units per hour.


## ❓ FAQ

**Q: What is the difference between critical and subcritical flow?**
Critical flow occurs when the downstream pressure is low enough that the fluid reaches sonic velocity at the choke throat, making the flow rate independent of downstream pressure. Subcritical flow occurs when downstream pressure is high enough to prevent sonic velocity.

**Q: How does this tool handle multiphase fluids?**
The tool accounts for multiphase characteristics by requiring fluid properties such as the gas-liquid ratio and compressibility in the input parameters.

**Q: Can I use this with Claude Desktop?**
Yes, this MCP server can be connected to Claude Desktop, Cursor, VS Code, Windsurf, and any other MCP-compatible client via Vinkius Edge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/choke-performance-model](https://vinkius.com/en/ai-agent-connect/choke-performance-model)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Choke Performance Model** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `choke-performance-model` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Choke Performance Model** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "choke-performance-model": {
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

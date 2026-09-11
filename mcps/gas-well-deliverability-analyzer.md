# Gas Well Deliverability Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/gas-well-deliverability-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate Absolute Open Flow (AOF) and analyze gas well deliverability with non-Darcy turbulence effects.

## Description
This MCP server provides specialized tools for reservoir engineering to assess gas well performance. It allows for the calculation of the Absolute Open Flow (AOF) using `calculate_aof`, predicting production rates at specific pressures with `get_flow_rate_at_pressure`, and generating full Inflow Performance Relationship (IPR) curves via `generate_ipr_curve`. Additionally, it quantifies the impact of turbulence on production using `analyze_turbulence_impact`, helping engineers understand how non-Darcy flow affects well potential.


## Available Tools (4)
- **calculate_aof**: Determines the theoretical maximum flow rate (AOF) of the gas well
- **generate_ipr_curve**: Generates a series of data points representing the Inflow Performance Relationship (IPR) curve
- **get_flow_rate_at_pressure**: Predicts the gas flow rate for a specific target bottomhole pressure
- **analyze_turbulence_impact**: Quantifies how much the non-Darcy effects are reducing the well's potential


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gas Well Deliverability Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the AOF for a well with reservoir pressure of 3500 psi, bottomhole pressure of 2500 psi, current flow rate of 5000 scf/d, and a turbulence coefficient of 0.05."

**🤖 AI Agent:**
> The calculated Absolute Open Flow (AOF) for this well is 12500 scf/d.

---

**👤 You:**
> "What will the flow rate be if the target bottomhole pressure is 2000 psi, given an AOF of 12500 scf/d, reservoir pressure of 3500 psi, and a turbulence coefficient of 0.05?"

**🤖 AI Agent:**
> The predicted gas flow rate at a bottomhole pressure of 2000 psi is 8250 scf/d.

---

**👤 You:**
> "Compare a Darcy flow rate of 6000 scf/d with an actual flow rate of 5000 scf/d."

**🤖 AI Agent:**
> The turbulence causes a 16.67% reduction in the well's potential, with an impact factor of 0.833.


## ❓ FAQ

**Q: What is Absolute Open Flow (AOF)?**
AOF is the theoretical maximum gas flow rate achievable if the bottomhole flowing pressure were reduced to zero.

**Q: How does this tool handle turbulence?**
The tools use a turbulence coefficient to account for non-Darcy flow effects, which reduce the actual flow rate compared to purely laminar flow.

**Q: Can I generate an IPR curve?**
Yes, you can use `generate_ipr_curve` to produce a series of data points representing the relationship between pressure and flow rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/gas-well-deliverability-analyzer](https://vinkius.com/ai-agent-connect/gas-well-deliverability-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gas Well Deliverability Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gas-well-deliverability-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gas Well Deliverability Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gas-well-deliverability-analyzer": {
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

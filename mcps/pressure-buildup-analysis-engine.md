# Pressure Buildup Analysis Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/pressure-buildup-analysis-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-science](../categories/data-science.md)

Analytical engine for evaluating reservoir performance through pressure buildup test data.

## Description
This MCP server provides advanced analytical tools for petroleum engineers to evaluate reservoir characteristics. By analyzing pressure recovery after a well shut-in, the engine identifies key parameters such as permeability and skin factor. Use `get_radial_flow_properties` to calculate primary reservoir characteristics, `get_wellbore_storage_parameters` to characterize early-time effects, `detect_boundary_effects` to identify reservoir limits, and `analyze_pressure_trends` for a high-level summary of recovery behavior.


## Available Tools (4)
- **analyze_pressure_trends**: Provides a high-level summary of the pressure recovery behavior
- **detect_boundary_effects**: Identifies if the pressure buildup has reached the limits of the reservoir
- **get_radial_flow_properties**: Calculates primary reservoir characteristics during the period of steady radial flow
- **get_wellbore_storage_parameters**: Characterizes the early-time effects caused by the wellbore volume


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pressure Buildup Analysis Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the reservoir permeability and skin factor from this pressure data."

**🤖 AI Agent:**
> The calculated permeability is 150 mD and the skin factor is 2.5.

---

**👤 You:**
> "Check if there are any boundary effects in this test."

**🤖 AI Agent:**
> Boundary effects were detected, indicating a drainage radius of 450 meters.

---

**👤 You:**
> "Summarize the pressure recovery trends."

**🤖 AI Agent:**
> The pressure recovery shows a transition from wellbore storage to a steady radial flow regime with a total pressure change of 500 psi.


## ❓ FAQ

**Q: How do I calculate permeability using this tool?**
You can use the `get_radial_flow_properties` tool. Provide the pressure data, the pre-shut-in flow rate, and the reservoir properties to receive the calculated permeability.

**Q: Can I detect if the reservoir boundaries have been reached?**
Yes, the `detect_boundary_effects` tool identifies if the pressure buildup has reached the limits of the reservoir and calculates the drainage radius.

**Q: What is the purpose of analyzing wellbore storage?**
The `get_wellbore_storage_parameters` tool characterizes early-time effects caused by the wellbore volume, which is essential for accurate reservoir response interpretation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/pressure-buildup-analysis-engine](https://vinkius.com/en/ai-agent-connect/pressure-buildup-analysis-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pressure Buildup Analysis Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pressure-buildup-analysis-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pressure Buildup Analysis Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pressure-buildup-analysis-engine": {
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

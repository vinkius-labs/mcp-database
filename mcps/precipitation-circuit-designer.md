# Precipitation Circuit Designer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/precipitation-circuit-designer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Engineering tool for designing metal recovery precipitation circuits.

## Description
This MCP server provides specialized engineering tools for designing hydrometallurgical precipitation circuits. It allows users to calculate reagent requirements, determine reactor dimensions, and evaluate kinetic feasibility for recovering metals like gold and copper. Use `design_precipitation_circuit` for a complete design plan, or `analyze_kinetics_feasibility` to verify if your planned retention time meets the target recovery rate.


## Available Tools (4)
- **analyze_kinetics_feasibility**: Evaluates if the desired recovery and retention time are chemically feasible
- **calculate_reactor_dimensions**: Determines the physical size of the reactor needed for the circuit
- **design_precipitation_circuit**: Performs a complete circuit design by integrating all inputs into a cohesive plan
- **get_reagent_requirements**: Calculates the amount of reagent needed to achieve a specific metal recovery


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Precipitation Circuit Designer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Design a circuit for a solution with 5.0 g/L gold and 2.0 g/L copper using the merrill-crowe method with 95% recovery and a flow rate of 10 m3/h."

**🤖 AI Agent:**
> The complete circuit design requires 45.2 kg of zinc dust, a reactor volume of 15.5 m3, and a retention time of 1.55 hours.

---

**👤 You:**
> "How much reagent is needed for 2.0 g/L copper with 90% recovery using direct precipitation?"

**🤖 AI Agent:**
> The required reagent mass is 12.4 kg with a molar ratio of 1.2.

---

**👤 You:**
> "Is a 2-hour retention time enough to recover 98% of gold?"

**🤖 AI Agent:**
> No, the target recovery of 98% is not feasible with a 2-hour retention time for gold; a longer residence time is required.


## ❓ FAQ

**Q: What metals can I design circuits for?**
The tool is optimized for gold and copper recovery using methods like `merrill-crowe` or direct precipitation.

**Q: How do I calculate the required reactor size?**
You can use the `calculate_reactor_dimensions` tool by providing the volumetric flow rate and the required retention time.

**Q: Can I check if my design is chemically viable?**
Yes, the `analyze_kinetics_feasibility` tool evaluates if your target recovery is achievable within the planned retention time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/precipitation-circuit-designer](https://vinkius.com/en/ai-agent-connect/precipitation-circuit-designer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Precipitation Circuit Designer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `precipitation-circuit-designer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Precipitation Circuit Designer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "precipitation-circuit-designer": {
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

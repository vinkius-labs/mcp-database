# Spiral Concentrator Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/spiral-concentrator-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Design mineral processing spiral concentrator circuits based on ore characteristics.

## Description
This MCP server provides specialized engineering tools for designing gravity separation circuits. Use `calculate_circuit_capacity` to determine the required number of units and footprint, `optimize_splitter_settings` to find the ideal radial position for mineral recovery, and `evaluate_flow_dynamics` to ensure stable slurry behavior. The toolset also includes `generate_design_summary` to aggregate all parameters into a final engineering specification.


## Available Tools (4)
- **calculate_circuit_capacity**: Determines the total number of spiral units and the required physical footprint for a given production target
- **evaluate_flow_dynamics**: Simulates how the slurry will behave on the spiral surface to ensure stable operation
- **generate_design_summary**: Aggregates all calculated parameters into a final engineering specification for the circuit
- **optimize_splitter_settings**: Recommends the precise position of splitters to maximize mineral recovery while minimizing gangue entrapment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spiral Concentrator Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the circuit capacity for a throughput of 50 tph with a mineral density of 4.5 and a particle size distribution of [0.1, 0.5, 1.0]."

**🤖 AI Agent:**
> The required circuit includes 5 spiral units with a total footprint area of 45 square meters in a parallel_banks configuration.

---

**👤 You:**
> "What is the optimal splitter position for a particle size of 0.2, mineral density of 4.0, pulp density of 0.3, and wash water flow of 5.0?"

**🤖 AI Agent:**
> The optimal splitter position is 35% with an expected recovery of 88% and an expected grade of 72%.

---

**👤 You:**
> "Evaluate the flow dynamics for a pulp density of 0.25, particle size of 0.15, and wash water flow of 2.0."

**🤖 AI Agent:**
> The flow stability index is 0.85 and the turbulence level is 0.12, indicating highly stable operation.


## ❓ FAQ

**Q: How do I determine the number of spiral units needed?**
You can use the `calculate_circuit_capacity` tool, providing the throughput, mineral density, and particle size distribution.

**Q: Can I optimize the splitter position for specific minerals?**
Yes, the `optimize_splitter_settings` tool allows you to input particle size, mineral density, pulp density, and wash water flow to find the best position.

**Q: How can I check if the slurry flow will be stable?**
Use the `evaluate_flow_dynamics` tool to simulate slurry behavior and receive a stability index and turbulence level.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/spiral-concentrator-design](https://vinkius.com/ai-agent-connect/spiral-concentrator-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spiral Concentrator Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `spiral-concentrator-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spiral Concentrator Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spiral-concentrator-design": {
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

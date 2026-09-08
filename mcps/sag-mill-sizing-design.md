# SAG Mill Sizing & Design MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/sag-mill-sizing-design)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate optimal SAG mill dimensions, power requirements, and ball charge.

## Description
This MCP server provides specialized engineering tools for Semi-Autogenous Grinding (SAG) mill design. It allows AI agents to determine physical mill dimensions using `calculate_mill_dimensions`, estimate electrical motor power with `calculate_power_requirements`, and optimize grinding media with `estimate_ball_charge`. Additionally, it can evaluate the necessity of a pebble crushing circuit via `evaluate_pebble_circuit` based on ore hardness and feed size.


## Available Tools (4)
- **calculate_mill_dimensions**: Determines the necessary physical size of the SAG mill
- **calculate_power_requirements**: Estimates the electrical power required to drive the mill
- **estimate_ball_charge**: Calculates the optimal amount of steel grinding media needed
- **evaluate_pebble_circuit**: Determines if a pebble crushing circuit is required


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SAG Mill Sizing & Design** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the dimensions for a SAG mill with 500 tph throughput, BWi of 15, feed size of 150mm, and target product size of 2mm?"

**🤖 AI Agent:**
> The required SAG mill dimensions are a diameter of 6.5 meters and a length of 8.0 meters, providing a total volume of 265.4 cubic meters.

---

**👤 You:**
> "Calculate the power requirements for a mill with 7m diameter, 9m length, 15% ball charge, and 60% ore volume."

**🤖 AI Agent:**
> The estimated motor power is 4250 kW with a torque of 185000 Nm.

---

**👤 You:**
> "Do I need a pebble crusher for an ore with BWi of 18, feed size of 120mm, and product size of 3mm if a crusher is available?"

**🤖 AI Agent:**
> Yes, based on the high Bond Work Index and size reduction requirements, a pebble crushing circuit is required to maintain efficiency.


## ❓ FAQ

**Q: How do I calculate the mill size?**
Use the `calculate_mill_dimensions` tool by providing the target throughput, Bond Work Index (BWi), feed size, and desired product size.

**Q: Can I estimate the power needed for the motor?**
Yes, the `calculate_power_requirements` tool estimates motor power and torque based on the mill's diameter, length, and charge volumes.

**Q: How is the ball charge determined?**
The `estimate_ball_charge` tool calculates the required steel media mass and volume percentage using the mill diameter, ore Abrasion Index (Ai), and throughput.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/sag-mill-sizing-design](https://vinkius.com/ai-agent-connect/sag-mill-sizing-design)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SAG Mill Sizing & Design** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sag-mill-sizing-design` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SAG Mill Sizing & Design** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sag-mill-sizing-design": {
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

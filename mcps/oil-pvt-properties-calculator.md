# Oil PVT Properties Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/oil-pvt-properties-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculates critical crude oil PVT properties like bubble point, viscosity, and formation volume factor.

## Description
This MCP server provides specialized petroleum engineering tools to calculate Pressure-Volume-Temperature (PVT) characteristics of crude oil. It uses established correlations such as Standing, Vasquez-Beggs, and Lasater to determine essential reservoir parameters. Use `get_pvt_summary` to obtain a complete overview of the oil's state, or specific tools like `calculate_bubble_point` and `calculate_viscosity` for targeted analysis of saturated and undersaturated conditions.


## Available Tools (4)
- **calculate_oil_properties**: Calculates the volume factor, solution gas ratio, and compressibility
- **calculate_viscosity**: Determines the oil's resistance to flow at specific reservoir conditions
- **get_pvt_summary**: Provides a comprehensive overview of the oil's state and properties
- **calculate_bubble_point**: Determines the pressure at which the first bubble of gas evolves from the oil


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Oil PVT Properties Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the bubble point pressure for an oil with 35 API, 500 GOR, 0.7 gas gravity, and 180°F using Standing correlation?"

**🤖 AI Agent:**
> The bubble point pressure is 2450.5 psi.

---

**👤 You:**
> "Calculate the oil viscosity for an oil with 30 API, 400 GOR, 0.65 gas gravity, 200°F, at 3000 psi, given a bubble point of 2500 psi."

**🤖 AI Agent:**
> The oil viscosity is 0.85 cP.

---

**👤 You:**
> "Provide a full PVT summary for oil with 32 API, 600 GOR, 0.75 gas gravity, 150°F, at 2000 psi and bubble point of 2200 psi."

**🤖 AI Agent:**
> The oil is in a saturated state. Bubble point pressure is 2200 psi, formation volume factor is 1.45, solution gas ratio is 600, viscosity is 1.12 cP, and compressibility is 3.5e-6 psi^-1.


## ❓ FAQ

**Q: Which mathematical models are supported?**
The server supports Standing, Vasquez-Beggs, and Lasater correlations for all PVT calculations.

**Q: How does the tool handle saturated vs undersaturated oil?**
The tool automatically determines the state by comparing the current pressure to the bubble point pressure calculated via `calculate_bubble_point`.

**Q: Can I get a full report of all properties at once?**
Yes, you can use the `get_pvt_summary` tool to receive a comprehensive overview including formation volume factor, solution gas ratio, and viscosity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/oil-pvt-properties-calculator](https://vinkius.com/ai-agent-connect/oil-pvt-properties-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Oil PVT Properties Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `oil-pvt-properties-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Oil PVT Properties Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "oil-pvt-properties-calculator": {
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

# Cycling Power Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/cycling-power-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [physics](../categories/physics.md)

Calculate precise power requirements for cycling based on speed, gradient, and wind.

## Description
This MCP server provides a deterministic engine to calculate the physiological and mechanical power requirements for cyclists. By accounting for gravitational resistance, rolling resistance, and aerodynamic drag, it helps riders understand the exact wattage needed to maintain specific speeds. It handles complex variables like wind direction (headwind, tailwind, or crosswind), altitude-based air density changes, and drivetrain efficiency. Use `calculate_power_requirement` for single scenarios, `simulate_climb_profile` for multi-stage climbs, or `get_aerodynamic_sensitivity` to analyze how wind or frontal area impacts your effort.


## Available Tools (3)
- **calculate_power_requirement**: Determines the exact power output needed to maintain a target speed under specific environmental conditions
- **get_aerodynamic_sensitivity**: Analyzes how changes in wind or frontal area affect the power requirement
- **simulate_climb_profile**: Calculates the power requirements for a multi-stage climb with changing gradients


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cycling Power Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much power do I need to ride at 30 km/h on a 5% gradient with a 10 km/h headwind? My total weight is 85 kg."

**🤖 AI Agent:**
> To maintain 30 km/h on a 5% gradient with a 10 km/h headwind at 85 kg, you need 342 Watts.

---

**👤 You:**
> "What is my power-to-weight ratio if I need 250 Watts and I weigh 70 kg?"

**🤖 AI Agent:**
> Your power-to-weight ratio is 3.57 W/kg.

---

**👤 You:**
> "How much will my power requirement increase if my frontal area increases by 10%?"

**🤖 AI Agent:**
> Increasing your frontal area by 10% will increase your required power by 12.4 Watts.


## ❓ FAQ

**Q: How does wind direction affect the calculation?**
The engine adjusts the relative airspeed based on the wind direction. A headwind increases the drag force, requiring more power, while a tailwind decreases it.

**Q: Does the tool account for altitude?**
Yes, the `calculate_power_requirement` tool adjusts for air density, which decreases as altitude increases, reducing aerodynamic drag.

**Q: Can I simulate a whole mountain climb?**
Yes, you can use the `simulate_climb_profile` tool by providing an array of segments, each with its own distance, gradient, and duration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/cycling-power-calculator](https://vinkius.com/ai-agent-connect/cycling-power-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cycling Power Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cycling-power-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cycling Power Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cycling-power-calculator": {
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

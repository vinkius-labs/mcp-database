# Formwork Tie Rod Design Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/formwork-tie-rod-design-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [construction](../categories/construction.md)

Calculates optimal tie rod spacing, waler sizing, and safety checks for concrete formwork.

## Description
This MCP server provides technical engineering tools to design concrete formwork systems. It calculates the required horizontal distance between tie rods using `get_rod_spacing` to prevent overloading. It also determines structural requirements for horizontal members with `get_waler_specification` and performs comprehensive safety evaluations via `get_system_safety_check`. Additionally, it provides precise placement coordinates for hardware using `get_tie_cone_layout`.


## Available Tools (4)
- **get_tie_cone_layout**: Defines the optimal placement of tie cones relative to the rod and waler intersections
- **get_waler_specification**: Determines the necessary structural size for the horizontal walers
- **get_rod_spacing**: Calculates the required horizontal distance between tie rods to prevent overloading
- **get_system_safety_check**: Evaluates if the current design configuration is safe against deflection and rod capacity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Formwork Tie Rod Design Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the required tie rod spacing for a pressure of 50 kPa, a rod capacity of 100 kN, and waler spacing of 1.5 m?"

**🤖 AI Agent:**
> The required tie rod spacing is 3.0 meters, with a safe working load of 100 kN.

---

**👤 You:**
> "Calculate the waler size for 40 kPa pressure, 0.6 m waler spacing, and 2.0 m tie rod spacing."

**🤖 AI Agent:**
> The required waler size is W10x22, with a maximum expected deflection of 0.004 m.

---

**👤 You:**
> "Is my design safe? Pressure: 60 kPa, Height: 4 m, Rod Spacing: 1.5 m, Rod Capacity: 120 kN, Waler Spacing: 1.2 m."

**🤖 AI Agent:**
> Yes, the design is safe with a margin of safety of 1.45.


## ❓ FAQ

**Q: How do I determine the spacing between my tie rods?**
You can use the `get_rod_spacing` tool by providing the concrete pressure, the rod capacity, and the vertical waler spacing.

**Q: Can this tool check if my formwork design is safe?**
Yes, the `get_system_safety_check` tool evaluates your design against deflection limits and rod capacity to ensure structural integrity.

**Q: What information is needed for waler sizing?**
To use `get_waler_specification`, you need to provide the concrete pressure, the waler spacing, and the horizontal tie rod spacing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/formwork-tie-rod-design-engine](https://vinkius.com/ai-agent-connect/formwork-tie-rod-design-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Formwork Tie Rod Design Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `formwork-tie-rod-design-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Formwork Tie Rod Design Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "formwork-tie-rod-design-engine": {
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

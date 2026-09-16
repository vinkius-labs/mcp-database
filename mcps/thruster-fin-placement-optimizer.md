# Thruster Fin Placement Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/thruster-fin-placement-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Optimizes surfboard fin configuration based on board geometry and wave conditions.

## Description
This MCP server provides precise hydrodynamic calculations for surfboard fin setups. By analyzing board dimensions, tail width, and wave energy, it determines the ideal longitudinal position for the center fin using `calculate_center_fin_position`, calculates lateral rail fin placement with `calculate_rail_fin_placement`, and determines optimal inward toe angles via `calculate_toe_angles`. For a complete configuration, use `optimize_full_setup` to receive a unified set of center, rail, and toe parameters tailored to specific tail shapes like Square, Swallow, or Round.


## Available Tools (4)
- **calculate_center_fin_position**: Determines the optimal longitudinal position for the center fin
- **calculate_rail_fin_placement**: Calculates the lateral distance of the side fins from the centerline
- **calculate_toe_angles**: Determines the optimal inward angle for the side fins
- **optimize_full_setup**: Provides a complete, unified fin configuration in a single call


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Thruster Fin Placement Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the best fin setup for a 6ft board with a 12 inch tail width in hollow waves?"

**🤖 AI Agent:**
> For a 6ft board in hollow waves, the optimal center position is 24.5 inches from the tail, with rail fins placed 7.2 inches from the centerline and a toe angle of 1.5 degrees.

---

**👤 You:**
> "Calculate the rail fin placement for a wide board in mushy waves."

**🤖 AI Agent:**
> The side fins should be placed 6.5 inches from the centerline to increase maneuverability in mushy conditions.

---

**👤 You:**
> "Find the center fin position for a narrow tail board."

**🤖 AI Agent:**
> The center fin should be placed 18.2 inches from the tail to prevent sliding out on a narrow tail setup.


## ❓ FAQ

**Q: How does wave type affect the fin setup?**
Different wave profiles require different stability and lift. For example, `calculate_toe_angles` adjusts angles to reduce drag in hollow waves or increase lift in mushy waves.

**Q: Can I get a complete setup in one go?**
Yes, you can use the `optimize_full_setup` tool to get the center position, rail distances, and toe angles all at once.

**Q: Does tail shape matter for the calculations?**
Yes, the tail shape (Square, Swallow, or Round) is a required input for `calculate_toe_angles` as it dictates how water flow is managed at the rear of the board.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/thruster-fin-placement-optimizer](https://vinkius.com/en/ai-agent-connect/thruster-fin-placement-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Thruster Fin Placement Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `thruster-fin-placement-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Thruster Fin Placement Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thruster-fin-placement-optimizer": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

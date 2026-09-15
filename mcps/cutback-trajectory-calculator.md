# Cutback Trajectory Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cutback-trajectory-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sports](../categories/sports.md)

Calculates optimal cutback points, turn radii, and re-entry angles for surfers.

## Description
This MCP server provides precise maneuver analysis for surfers. By analyzing wave geometry and board dynamics, it helps surfers determine the exact moment to initiate a turn. Use `get_optimal_cutback_point` to find the ideal initiation location, `calculate_maneuver_radius` to determine the turn's curvature, and `calculate_reentry_angle` to predict the return to the wave face. It also includes `analyze_section_timing` to ensure the surfer stays ahead of the breaking section.


## Available Tools (4)
- **analyze_section_timing**: Determines how much time the surfer has before the wave section moves past the cutback zone
- **calculate_maneuver_radius**: Calculates the curvature of the turn based on physical constraints
- **calculate_reentry_angle**: Predicts the angle at which the surfer will return to the wave face
- **get_optimal_cutback_point**: Determines the ideal location on the wave to begin the cutback maneuver


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cutback Trajectory Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Where should I start my cutback on a peeling wave if I'm on a shortboard going 5 m/s?"

**🤖 AI Agent:**
> The ideal initiation point is 4.5 meters ahead of your current position at a 15-degree angle.

---

**👤 You:**
> "What will my re-entry angle be if I have a maneuver radius of 3 meters on a hollow wave?"

**🤖 AI Agent:**
> The predicted re-entry angle is 42 degrees relative to the wave face.

---

**👤 You:**
> "How much time do I have to turn if the wave section is moving at 4 m/s and I am going 6 m/s?"

**🤖 AI Agent:**
> You have 2.5 seconds before the section becomes unmanageable for a cutback.


## ❓ FAQ

**Q: How do I find the best place to start my turn?**
You can use the `get_optimal_cutback_point` tool. Provide the wave shape, your current speed, and your board type to receive the distance to the ideal initiation point.

**Q: Can I adjust for different surfboard types?**
Yes, all tools account for board types like shortboard, fish, or longboard to adjust the physics of the turn radius and re-entry.

**Q: How do I know if I have enough time to complete the maneuver?**
Use the `analyze_section_timing` tool. It calculates the time remaining before the wave section moves past the cutback zone based on your speed and the section speed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cutback-trajectory-calculator](https://vinkius.com/en/ai-agent-connect/cutback-trajectory-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cutback Trajectory Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cutback-trajectory-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cutback Trajectory Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cutback-trajectory-calculator": {
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

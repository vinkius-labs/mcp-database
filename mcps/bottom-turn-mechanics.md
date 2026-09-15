# Bottom Turn Mechanics MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/bottom-turn-mechanics)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [simulation](../categories/simulation.md)

Analyze surfing bottom turn physics, G-forces, and board suitability.

## Description
This MCP server provides advanced fluid dynamics and physical modeling for surfing maneuvers. It allows AI agents to calculate the required speed and peak G-forces for specific turn configurations using `get_turn_physics_summary`. Users can evaluate how well a surfboard performs in specific wave conditions with `get_board_suitability` and analyze the transition between compression and extension phases via `analyze_compression_extension_efficiency`. Finally, `predict_performance_outcome` simulates the success probability of a maneuver based on wave speed, turn radius, and surfer flexibility.


## Available Tools (4)
- **get_board_suitability**: Determines if a specific surfboard is appropriate for a planned bottom turn
- **analyze_compression_extension_efficiency**: Evaluates how effectively a surfer can manage the transition between crouching and standing during the turn
- **predict_performance_outcome**: Simulates the likely result of the maneuver based on all mechanical inputs
- **get_turn_physics_summary**: Provides a comprehensive breakdown of the forces and requirements for a specific turn configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bottom Turn Mechanics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the physics requirements for a turn with a 5m radius in a 10m/s wave using a 30L board with 0.2 rocker?"

**🤖 AI Agent:**
> For a 5m radius turn in a 10m/s wave, the required speed is 8.5 m/s, the peak G-force is 2.4, and the optimal radius is 5.2m with a high stability rating.

---

**👤 You:**
> "Is a 25L board with 0.1 rocker suitable for a tight turn in a fast wave?"

**🤖 AI Agent:**
> The suitability score is 0.4, indicating low suitability for tight turns due to the low rocker and high drag coefficient.

---

**👤 You:**
> "Predict the outcome for a surfer with 0.8 flexibility performing a turn in a 12m/s wave."

**🤖 AI Agent:**
> The predicted outcome is a High Speed Glide with a 85% success probability and an expected G-force of 1.8.


## ❓ FAQ

**Q: How can I determine if my board is right for a specific wave?**
You can use the `get_board_suitability` tool to receive a suitability score, drag coefficient, and maneuverability index based on wave speed and board characteristics.

**Q: Can I predict the G-forces I will experience during a turn?**
Yes, the `get_turn_physics_summary` tool calculates the peak G-force experienced during a maneuver based on your turn radius and wave speed.

**Q: How does surfer flexibility affect the turn?**
Flexibility is a key input for `analyze_compression_extension_efficiency`, which determines how effectively you can manage the transition between crouching and standing during the maneuver.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/bottom-turn-mechanics](https://vinkius.com/en/ai-agent-connect/bottom-turn-mechanics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bottom Turn Mechanics** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bottom-turn-mechanics` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bottom Turn Mechanics** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bottom-turn-mechanics": {
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

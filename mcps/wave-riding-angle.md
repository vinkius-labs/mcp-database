# Wave Riding Angle MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wave-riding-angle)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [environment](../categories/environment.md)

Calculate optimal approach angles, section speeds, and air time potential for surfing.

## Description
This MCP server provides analytical tools for surfers to optimize their performance based on wave kinematics and environmental conditions. Use `get_optimal_approach_angle` to find the best angle to stay in the pocket, `calculate_section_matching_speed` to match the velocity of the breaking section, `estimate_air_time_potential` to predict verticality and flight time, and `evaluate_ride_safety` to assess the risks of specific wave and gear combinations.


## Available Tools (4)
- **calculate_section_matching_speed**: How fast do I need to travel to stay ahead of the breaking part of the wave?
- **estimate_air_time_potential**: How much verticality and air time can I expect from this wave?
- **evaluate_ride_safety**: Is this specific combination of wave and gear safe to ride?
- **get_optimal_approach_angle**: At what angle should I point my board to stay in the pocket of the wave?


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wave Riding Angle** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What angle should I point my board to stay in the pocket? The wave is moving at 5 m/s at 90 degrees, wind is at 45 degrees, and I am using a Shortboard."

**🤖 AI Agent:**
> You should maintain an approach angle of 15 degrees from the wave direction, resulting in a recommended heading of 105 degrees.

---

**👤 You:**
> "How fast do I need to go to stay ahead of the wave? Wave speed is 4 m/s, direction is 180 degrees, steepness is 0.3, and I have a Fish board."

**🤖 AI Agent:**
> Your target speed is 4.6 m/s, with a recommended velocity buffer of 0.4 m/s.

---

**👤 You:**
> "Is it safe to ride a 6 m/s wave with 0.5 steepness using a Shortboard? Wind is at 200 degrees and wave is at 180 degrees."

**🤖 AI Agent:**
> The safety rating is 65. The primary risk factor is High Wind Overturning. It is recommended to use a longer board.


## ❓ FAQ

**Q: How do I use the approach angle tool?**
Provide the wave speed, wave direction, wind direction, and your board type to `get_optimal_approach_angle` to receive a recommended heading.

**Q: Can I use this with different surfboard types?**
Yes, the tools account for Longboard, Shortboard, Fish, and Gun profiles to ensure accurate physics calculations.

**Q: Does wind direction affect the results?**
Yes, wind direction is a critical input for `estimate_air_time_potential` and `evaluate_ride_safety` as it influences wave steepness and stability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wave-riding-angle](https://vinkius.com/en/ai-agent-connect/wave-riding-angle)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wave Riding Angle** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wave-riding-angle` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wave Riding Angle** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wave-riding-angle": {
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

# Terrain Park Gap Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/terrain-park-gap-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [safety](../categories/safety.md)

Calculates jump trajectories, gap distances, and knuckle clearance for freestyle features.

## Description
This MCP server provides physics-based analysis for freestyle skiing and snowboarding features. It uses projectile motion models to calculate the flight path between takeoff and landing. Use `get_gap_analysis` to determine the horizontal gap distance and `knuckleClearance`. You can also use `check_knuckle_collision_risk` to assess the danger of hitting the landing knuckle, or `validate_speed_requirements` to ensure the approach speed is safe for a specific gap configuration.


## Available Tools (4)
- **check_knuckle_collision_risk**: Specifically assesses the danger of hitting the knuckle based on the flight path
- **get_feature_safety_buffer**: Calculates the necessary safety spacing based on feature types and environmental conditions
- **get_gap_analysis**: Calculates the physical distance and flight characteristics of a jump
- **validate_speed_requirements**: Determines if a specific approach speed is sufficient or excessive for a given gap configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Terrain Park Gap Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze a jump with an approach speed of 12 m/s, a takeoff angle of 30 degrees, a landing angle of 25 degrees, and a kicker feature on groomed snow."

**🤖 AI Agent:**
> The gap distance is 18.45 meters, with a knuckle clearance of 1.2 meters. Your speed is within the safe operating window.

---

**👤 You:**
> "Is 10 m/s enough speed to clear a 15 meter gap with a 35 degree takeoff angle?"

**🤖 AI Agent:**
> No, the minimum required speed to clear a 15 meter gap with a 35 degree takeoff angle is 11.2 m/s.

---

**👤 You:**
> "What is the risk of hitting the knuckle if I have a 5 meter gap, 15 degree takeoff, 20 degree landing, and 10 m/s speed?"

**🤖 AI Agent:**
> The risk level is critical because the clearance value is -0.4 meters.


## ❓ FAQ

**Q: How do I check if my speed is safe for a jump?**
You can use the `validate_speed_requirements` tool to compare your approach speed against the minimum required speed and maximum safe speed for your specific gap.

**Q: What is knuckle clearance?**
Knuckle clearance is the vertical distance between the lowest point of your flight path and the highest point (knuckle) of the landing feature. A positive value means you clear it.

**Q: Does snow condition affect the calculations?**
Yes, you can provide a `snowCondition` like 'icy' or 'powder' to `get_gap_analysis` to adjust the effective takeoff speed based on friction.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/terrain-park-gap-analyzer](https://vinkius.com/en/ai-agent-connect/terrain-park-gap-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Terrain Park Gap Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `terrain-park-gap-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Terrain Park Gap Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "terrain-park-gap-analyzer": {
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

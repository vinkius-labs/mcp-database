# Board Carve Radius Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/board-carve-radius-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [simulation](../categories/simulation.md)

Physics-driven engine for calculating surfboard turning mechanics, G-forces, and spray patterns.

## Description
This MCP server provides high-fidelity physics calculations for surfboard performance. It allows AI agents to determine the precise turning mechanics of a planing hull. Use `calculate_carve_radius` to find the turning path, `calculate_turn_gforce` to measure physical load, `simulate_spray_trajectory` to predict water displacement, and `get_optimized_configuration` to find the best equipment setup for specific maneuvers.


## Available Tools (4)
- **calculate_carve_radius**: Determines the primary turning radius of the board based on rider input and board geometry
- **calculate_turn_gforce**: Calculates the physical gravitational load experienced by the rider during the carve
- **get_optimized_configuration**: Recommends the ideal fin setup or rocker for a target radius
- **simulate_spray_trajectory**: Predicts the visual pattern and direction of the water spray kicked up by the rail


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Board Carve Radius Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the turning radius for a 180cm board at 5m/s with a 30 degree edge angle and a thruster fin setup?"

**🤖 AI Agent:**
> The calculated turning radius is 3.45 meters with a stability score of 0.82.

---

**👤 You:**
> "How much G-force will I feel if I carve at 6m/s with a 2.5 meter radius and a total mass of 85kg?"

**🤖 AI Agent:**
> You will experience a G-force of 1.48, which is categorized as moderate load intensity.

---

**👤 You:**
> "Predict the spray pattern for a hard rail at 4m/s with a high rocker profile and 45 degree edge angle."

**🤖 AI Agent:**
> The spray will reach a height of 0.85 meters at a 35 degree angle with high volume intensity.


## ❓ FAQ

**Q: How accurate are the turning radius calculations?**
The `calculate_carve_radius` tool uses fluid dynamics models to estimate the path based on edge angle, speed, and fin configuration.

**Q: Can I optimize my board setup for specific turns?**
Yes, you can use `get_optimized_configuration` to receive recommendations for fin types and rocker profiles based on your target radius.

**Q: Does this account for rider weight?**
Yes, the `calculate_turn_gforce` tool requires the combined mass of the rider and equipment to calculate the physical load.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/board-carve-radius-engine](https://vinkius.com/ai-agent-connect/board-carve-radius-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Board Carve Radius Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `board-carve-radius-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Board Carve Radius Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "board-carve-radius-engine": {
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

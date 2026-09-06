# Water Depth Clearance MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/water-depth-clearance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [safety](../categories/safety.md)

Calculates safety margins and minimum water depth for aquatic maneuvers.

## Description
This MCP server provides critical safety calculations for aquatic athletes. It uses a depth penetration model to determine if a maneuver is safe based on water depth, impact velocity, rider height, and seabed composition. Use `calculate_penetration_safety` to check current feasibility, `get_min_depth_requirements` to plan for specific tricks, or `compare_bottom_risks` to understand the impact of switching from sand to reef environments.


## Available Tools (4)
- **calculate_penetration_safety**: Determines if a planned trick is safe based on current depth and impact parameters
- **compare_bottom_risks**: Compares the safety implications of performing the same trick on different seabed types
- **get_min_depth_requirements**: Answers how much water is needed for a specific trick regardless of current conditions
- **validate_maneuver_parameters**: Validates if the provided physical inputs are within the logical bounds for aquatic maneuvers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Water Depth Clearance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Is it safe to perform a vertical drop in 3 meters of water with a 2 m/s impact velocity on a sand bottom?"

**🤖 AI Agent:**
> Yes, with a 3m depth and a 2 m/s velocity on sand, the safety margin is 1.2 meters, making the maneuver feasible.

---

**👤 You:**
> "How much water depth do I need for a sliding entry at 4 m/s velocity for a 1.8m tall rider on a reef?"

**🤖 AI Agent:**
> For a sliding entry at 4 m/s with a 1.8m rider on a reef, the minimum safe depth required is 4.5 meters.

---

**👤 You:**
> "Compare the risk of a vertical drop on sand versus reef at 5 m/s velocity."

**🤖 AI Agent:**
> Switching from sand to reef requires an additional 1.5 meters of depth to maintain the same safety margin due to the rigid nature of the reef.


## ❓ FAQ

**Q: How does seabed type affect safety?**
Seabed composition changes the required safety buffer. Using `compare_bottom_risks` helps identify how much more depth is needed when moving from a compliant sand bottom to a rigid reef.

**Q: Can I check if a specific trick is safe right now?**
Yes, you can use the `calculate_penetration_safety` tool by providing the current water depth, your impact velocity, and the bottom type.

**Q: What information is needed to calculate minimum depth?**
To use `get_min_depth_requirements`, you need the trick type, expected impact velocity, rider height, and the bottom type (sand or reef).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/water-depth-clearance](https://vinkius.com/ai-agent-connect/water-depth-clearance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Water Depth Clearance** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `water-depth-clearance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Water Depth Clearance** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "water-depth-clearance": {
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

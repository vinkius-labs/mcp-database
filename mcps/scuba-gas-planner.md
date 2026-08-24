# Scuba Gas Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/scuba-gas-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [safety](../categories/safety.md)

Deterministic gas consumption and depth limit calculations for scuba divers.

## Description
A specialized toolset for scuba divers to perform critical safety calculations. This MCP server provides precise tools to determine breathing endurance, identify safe depth limits based on oxygen toxicity, calculate narcotic effects, and determine the necessary rock-bottom gas reserves for safe ascents. Use `calculate_breathing_endurance` to find available time at depth, `calculate_depth_limits` to find your MOD, `calculate_narcotic_effect` for END, and `calculate_safety_reserve` for ascent planning.


## Available Tools (4)
- **calculate_depth_limits**: Identifies the safest depth limits for a specific gas mixture based on oxygen toxicity
- **calculate_narcotic_effect**: Determines the physiological narcotic impact of a gas mix at a specific depth
- **calculate_safety_reserve**: Calculates the minimum volume of gas required to perform a safe ascent from the bottom to the surface
- **calculate_breathing_endurance**: Determines how long a diver can safely breathe a specific gas supply at a specific depth


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Scuba Gas Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long can I breathe a 12L tank at 30 meters if my SAC rate is 20 L/min and current pressure is 200 bar?"

**🤖 AI Agent:**
> At 30 meters (4 ATA), your available breathing time is 30 minutes.

---

**👤 You:**
> "What is my maximum working depth for Nitrox 36 with a ppO2 limit of 1.4?"

**🤖 AI Agent:**
> Your maximum working depth for Nitrox 36 is 34.3 meters.

---

**👤 You:**
> "What is the equivalent narcotic depth for air at 30 meters?"

**🤖 AI Agent:**
> The equivalent narcotic depth is 30 meters.


## ❓ FAQ

**Q: How do I calculate my maximum depth for Nitrox 32?**
You can use the `calculate_depth_limits` tool by providing 32 as the oxygen percentage to find your maximum working and deco depths.

**Q: How much gas do I need for a safe ascent?**
Use the `calculate_safety_reserve` tool with your target depth and SAC rate to determine the required rock-bottom reserve.

**Q: Can I calculate my breathing time at a specific depth?**
Yes, use `calculate_breathing_endurance` with your cylinder volume, pressure, SAC rate, and target depth.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/scuba-gas-planner](https://vinkius.com/ai-agent-connect/scuba-gas-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Scuba Gas Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `scuba-gas-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Scuba Gas Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "scuba-gas-planner": {
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

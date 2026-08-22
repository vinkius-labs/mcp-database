# Paddle-Out Calorie Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/paddle-out-calorie-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate physiological energy expenditure and time for surfing paddle-outs based on water currents.

## Description
This MCP server provides deterministic tools for surfers to calculate the physical impact of water currents on their paddle-out. By accounting for current velocity, body mass, and distance, it calculates effective distance, time required, and total calories burned. Use `calculate_paddle_expenditure` to get a full physiological breakdown, `check_current_safety` to assess if a current is too strong for progression, or `get_session_summary` for a high-level overview of energy deficit or advantage.


## Available Tools (3)
- **check_current_safety**: Determines if the current is too strong for a standard paddle-out attempt
- **calculate_paddle_expenditure**: Calculates the total physiological impact of a specific paddle-out session including time and calories
- **get_session_summary**: Provides a high-level overview of the energy deficit or advantage provided by the current


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Paddle-Out Calorie Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many calories will I burn paddling 500 meters against a 1.5 knot outgoing current if I weigh 80kg?"

**🤖 AI Agent:**
> Paddling 500 meters against a 1.5 knot current with a weight of 80kg will result in an effective distance of 1500 meters, approximately 25 minutes of paddling, and a total burn of 234.3 calories.

---

**👤 You:**
> "Is it safe to paddle out 300 meters if the current is 2.5 knots?"

**🤖 AI Agent:**
> No, a 2.5 knot current is too strong for a standard paddle-out attempt as it exceeds the assumed paddling speed.

---

**👤 You:**
> "Give me a summary of a 400m paddle with a -0.5 knot incoming current."

**🤖 AI Agent:**
> The incoming current provides an energy advantage, making the paddle-out more efficient by reducing the effective distance.


## ❓ FAQ

**Q: How does the current affect my calorie calculation?**
An outgoing current increases the effective distance you must paddle, which increases the total calories burned. An incoming current reduces the effort required.

**Q: Can I use this to check if it is safe to go out?**
Yes, you can use the `check_current_safety` tool to determine if the current speed is within safe limits for a standard paddle-out attempt.

**Q: What factors are included in the energy estimation?**
The calculation includes your weight, the distance to the target, the speed of the water current, and a standard metabolic constant for surfing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/paddle-out-calorie-estimator](https://vinkius.com/ai-agent-connect/paddle-out-calorie-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Paddle-Out Calorie Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `paddle-out-calorie-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Paddle-Out Calorie Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "paddle-out-calorie-estimator": {
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

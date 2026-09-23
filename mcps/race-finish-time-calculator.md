# Race Finish Time Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/race-finish-time-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate race finish times, required paces, and distance coverage.

## Description
This MCP server provides precise tools for athletes and coaches to plan race performance. Use `get_estimated_finish_time` to predict completion times, `get_required_pace` to determine the speed needed for a target goal, `get_pace_comparison` to evaluate current speed against targets, and `get_distance_from_pace_and_time` to estimate distance covered within a time limit.


## Available Tools (4)
- **get_distance_from_pace_and_time**: Calculate distance covered given pace and time
- **get_estimated_finish_time**: Calculate estimated finish time based on distance and pace
- **get_pace_comparison**: Compare current pace with a target pace
- **get_required_pace**: Calculate the required pace to hit a target finish time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Race Finish Time Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How long will it take me to finish a 42.2 km marathon at a pace of 5.5 minutes per km?"

**🤖 AI Agent:**
> It will take you 03:52:11 to finish the marathon.

---

**👤 You:**
> "What pace do I need to run a 10k in 50 minutes?"

**🤖 AI Agent:**
> You need to maintain a pace of 05:00 per km.

---

**👤 You:**
> "How far can I run in 30 minutes if my pace is 6 minutes per mile?"

**🤖 AI Agent:**
> You can run 5.0 miles.


## ❓ FAQ

**Q: What units are supported?**
The server supports both kilometers (km) and miles for distance and pace calculations.

**Q: How can I find my target pace?**
You can use the `get_required_pace` tool by providing your total distance and your desired target finish time in seconds.

**Q: Can I compare two different paces?**
Yes, the `get_pace_comparison` tool allows you to see the difference between your current pace and a target pace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/race-finish-time-calculator](https://vinkius.com/en/ai-agent-connect/race-finish-time-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Race Finish Time Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `race-finish-time-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Race Finish Time Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "race-finish-time-calculator": {
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

# Running Lap Counter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/running-lap-counter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate completed laps and progress on a running track.

## Description
This MCP server provides tools to convert total distance traveled into track lap data. Use `get_lap_summary` for a complete overview, `get_completed_laps` to find whole circuits finished, `get_partial_progress` to see distance remaining in the current lap, or `get_exact_lap_count` for precise decimal values.


## Available Tools (4)
- **get_completed_laps**: Determines how many full circuits a runner has successfully finished
- **get_exact_lap_count**: Provides the precise mathematical number of laps, including fractional parts
- **get_lap_summary**: Provides a comprehensive overview of running progress including whole laps and the remaining distance
- **get_partial_progress**: Calculates the remaining distance covered in the current, unfinished lap


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Running Lap Counter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I ran 5000 meters on a 400 meter track. How many laps did I complete?"

**🤖 AI Agent:**
> You have completed 12 full laps.

---

**👤 You:**
> "Give me a summary of my progress: 1250m total distance on a 400m track."

**🤖 AI Agent:**
> You have completed 3 full laps, with 50 meters remaining in your current lap, for a total of 3.125 laps.

---

**👤 You:**
> "What is the exact lap count for 1000m on a 400m track?"

**🤖 AI Agent:**
> The exact lap count is 2.5 laps.


## ❓ FAQ

**Q: How do I calculate my total laps?**
You can use the `get_lap_summary` tool to get a full report of completed laps, remaining distance, and the exact decimal lap count.

**Q: Can I get the exact decimal number of laps?**
Yes, use the `get_exact_lap_count` tool to receive the precise mathematical lap count including fractional parts.

**Q: How much distance is left in my current lap?**
Use the `get_partial_progress` tool to find the remaining distance covered in your current, unfinished lap.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/running-lap-counter](https://vinkius.com/en/ai-agent-connect/running-lap-counter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Running Lap Counter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `running-lap-counter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Running Lap Counter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "running-lap-counter": {
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

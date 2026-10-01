# Rowing Pace Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/rowing-pace-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate rowing ergometer pace, power, and stroke rate.

## Description
This MCP server provides essential calculations for rowing ergometer training. It allows AI agents to determine the 500m split using `get_pace_from_time`, calculate total duration with `get_time_from_pace`, determine required wattage via `get_power_from_pace`, and estimate necessary stroke rates using `estimate_stroke_rate`.


## Available Tools (4)
- **estimate_stroke_rate**: Estimates the stroke rate (SPM) needed to achieve a specific power output at a specific pace
- **get_pace_from_time**: Calculates the 500m pace when the total distance and total time are known
- **get_power_from_pace**: Calculates the physical power output (Watts) required to maintain a specific pace
- **get_time_from_pace**: Calculates the total time required to complete a specific distance at a target pace


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rowing Pace Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I rowed 2000 meters in 420 seconds. What was my 500m pace?"

**🤖 AI Agent:**
> Your 500m pace was 1:45 per 500m.

---

**👤 You:**
> "How much time will it take to row 5000 meters at a 2:00 pace?"

**🤖 AI Agent:**
> It will take 1000 seconds (16 minutes and 40 seconds) to complete 5000 meters at a 2:00/500m pace.

---

**👤 You:**
> "What power do I need for a 1:50 pace?"

**🤖 AI Agent:**
> To maintain a 1:50 pace, you need to produce approximately 235 Watts.


## ❓ FAQ

**Q: How do I calculate my 500m split?**
You can use the `get_pace_from_time` tool by providing the total distance rowed and the total time taken.

**Q: Can I estimate the power needed for a specific pace?**
Yes, the `get_power_from_pace` tool calculates the required wattage for a given 500m split.

**Q: How is stroke rate estimated?**
The `estimate_stroke_rate` tool estimates the strokes per minute (SPM) based on your target power and pace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/rowing-pace-calculator](https://vinkius.com/en/ai-agent-connect/rowing-pace-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Rowing Pace Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rowing-pace-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Rowing Pace Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rowing-pace-calculator": {
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

# Swimming Pace Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/swimming-pace-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fitness](../categories/fitness.md)

Precision tools for calculating swimming pace, lap splits, stroke rates, and interval training plans.

## Description
This MCP server provides a suite of precision tools for swimmers to convert distances, times, and paces into actionable training metrics. Use `calculate_pace_metrics` to find your base pace per 100 units, `calculate_lap_splits` to generate a schedule of individual lap times, `estimate_stroke_rate` to analyze movement efficiency, and `generate_interval_plan` to structure repetitive training sets with rest periods. It supports both meters (m) and yards (yd) for standardized training across different pool environments.


## Available Tools (4)
- **estimate_stroke_rate**: Estimate strokes per minute
- **calculate_lap_splits**: Generate a schedule of individual lap times
- **calculate_pace_metrics**: Calculate base swimming pace per 100 units
- **generate_interval_plan**: Create a structured swimming interval plan


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Swimming Pace Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my pace per 100m if I swim 400m in 320 seconds?"

**🤖 AI Agent:**
> Your pace is 80 seconds per 100m (1:20/100m).

---

**👤 You:**
> "Calculate lap splits for 100m in a 25m pool with a pace of 90 seconds per 100m."

**🤖 AI Agent:**
> For a 100m distance in a 25m pool, you will complete 4 laps. Each lap split is 22.5 seconds.

---

**👤 You:**
> "Create an interval plan for 10 repetitions of 50m at 45 seconds per 100m with 15 seconds rest."

**🤖 AI Agent:**
> The total workout time is 300 seconds. Each 50m interval takes 22.5 seconds, and there are 135 seconds of total rest.


## ❓ FAQ

**Q: Does this support both meters and yards?**
Yes, all tools support both meters (m) and yards (yd) to ensure accuracy in any pool.

**Q: How can I plan my interval training?**
You can use the `generate_interval_plan` tool by providing the repetition distance, target pace, rest time, and number of repetitions.

**Q: Can I calculate my lap splits?**
Yes, the `calculate_lap_splits` tool generates a complete schedule of times for each length of the pool based on your target pace.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/swimming-pace-calculator](https://vinkius.com/en/ai-agent-connect/swimming-pace-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Swimming Pace Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `swimming-pace-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Swimming Pace Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "swimming-pace-calculator": {
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

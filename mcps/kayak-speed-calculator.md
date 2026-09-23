# Kayak Speed Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/kayak-speed-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate kayak velocity, pace, and performance tiers.

## Description
This MCP server provides tools to analyze kayak performance. Use `get_kayak_velocity` to find speed, `get_kayak_pace` to determine minutes per kilometer, `evaluate_performance_tier` to categorize skill levels, and `calculate_estimated_trip_time` to predict future durations.


## Available Tools (4)
- **calculate_estimated_trip_time**: Calculate the estimated trip time
- **evaluate_performance_tier**: Evaluate the performance tier of a kayak speed
- **get_kayak_pace**: Calculate the pace of a kayak
- **get_kayak_velocity**: Calculate the velocity of a kayak


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kayak Speed Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How fast was I going if I paddled 10km in 2 hours?"

**🤖 AI Agent:**
> Your speed was 5 km/h.

---

**👤 You:**
> "What is my pace if I cover 5km in 30 minutes?"

**🤖 AI Agent:**
> Your pace is 6 minutes per kilometer.

---

**👤 You:**
> "If I want to travel 20km at 4 km/h, how long will it take?"

**🤖 AI Agent:**
> It will take 5 hours to complete the trip.


## ❓ FAQ

**Q: How do I calculate my kayak speed?**
You can use the `get_kayak_velocity` tool by providing the total distance in kilometers and the total duration in hours.

**Q: Can I determine my skill level?**
Yes, the `evaluate_performance_tier` tool categorizes your speed into tiers such as Recreational, Intermediate, Advanced, or Elite.

**Q: How can I estimate how long a trip will take?**
Use the `calculate_estimated_trip_time` tool with your target distance and your current speed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/kayak-speed-calculator](https://vinkius.com/en/ai-agent-connect/kayak-speed-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Kayak Speed Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `kayak-speed-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Kayak Speed Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "kayak-speed-calculator": {
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

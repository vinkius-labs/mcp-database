# Travel Time Wave Quality MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/travel-time-wave-quality)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel](../categories/travel.md)

Evaluate surf trip efficiency by weighing wave quality against travel time and fuel costs.

## Description
This MCP server provides decision-support tools for surfers to determine if a trip is worth the effort. By analyzing the relationship between time investment, wave quality, and travel expenses, it calculates key metrics like quality-hours and trip scores. Use `calculate_trip_efficiency` to find the core value of a trip, `estimate_fuel_burden` to see the financial impact per wave, `analyze_swell_window_utility` to check swell window coverage, or `compare_trip_options` to choose between two different surf destinations.


## Available Tools (4)
- **analyze_swell_window_utility**: Determines how much of the optimal swell window is being utilized effectively
- **compare_trip_options**: Compares two different trip profiles to recommend the one with the best balance of quality and cost
- **calculate_trip_efficiency**: Evaluates the core value of a trip by comparing the time spent surfing against the time spent traveling
- **estimate_fuel_burden**: Calculates the financial impact of the trip relative to the expected surfing time


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Travel Time Wave Quality** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the efficiency of a trip with 4 hours of travel, 6 hours of surfing, and a wave quality score of 4."

**🤖 AI Agent:**
> The trip has 24 quality-hours and a trip score of 12.5.

---

**👤 You:**
> "I spent $50 on fuel for a 5-hour surf session. How much does each wave cost me?"

**🤖 AI Agent:**
> The fuel cost is $10 per hour, which results in an estimated cost of $0.25 per wave.

---

**👤 You:**
> "Is my 3-hour surf session a good use of a 10-hour swell window if I have 2 hours of travel time?"

**🤖 AI Agent:**
> The swell window utilization is 30%, and the effective window coverage is 0.8.


## ❓ FAQ

**Q: How is the trip score calculated?**
The trip score is a normalized metric that balances total quality-hours against travel time and fuel costs using the `calculate_trip_efficiency` logic.

**Q: Can I compare two different surf spots?**
Yes, you can use the `compare_trip_options` tool to compare two trip profiles and see which one offers a better balance of quality and cost.

**Q: What does 'quality-hours' mean?**
Quality-hours represent the 'effective surfing time,' calculated by multiplying the expected surfing duration by the numerical wave quality score.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/travel-time-wave-quality](https://vinkius.com/en/ai-agent-connect/travel-time-wave-quality)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Travel Time Wave Quality** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `travel-time-wave-quality` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Travel Time Wave Quality** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "travel-time-wave-quality": {
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

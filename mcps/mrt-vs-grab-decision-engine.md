# MRT vs Grab Decision Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/mrt-vs-grab-decision-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [transportation](../categories/transportation.md)

A deterministic decision tool to choose between MRT and ride-hailing in Singapore.

## Description
This MCP server provides precise transport recommendations for commuters in Singapore. By analyzing distance, urgency, weather, and peak hours, it calculates the exact time and cost trade-offs between the MRT and ride-hailing services like Grab or Gojek. Use `calculate_commute_strategy` to get a full comparison, `get_weather_surge_multiplier` to check weather-based price increases, or `is_peak_hour` to identify rush hour windows.


## Available Tools (3)
- **calculate_commute_strategy**: Provide a complete comparison between MRT and Grab/Gojek based on current trip conditions
- **get_weather_surge_multiplier**: Retrieve the specific cost multiplier applied to ride-hailing services based on environmental conditions
- **is_peak_hour**: Determine if the current time falls within Singapore's standard peak commuting periods


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MRT vs Grab Decision Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I need to travel 5km. I am in a hurry (high sensitivity), it is currently raining, and the time is 08:30. Should I take MRT or Grab?"

**🤖 AI Agent:**
> Take Grab

---

**👤 You:**
> "I have a 10km trip. Time sensitivity is low, weather is sunny, and it is 14:00. What is the best option?"

**🤖 AI Agent:**
> Take MRT

---

**👤 You:**
> "It is a storm and I have a 3km trip. I am not in a rush (low sensitivity). What should I do?"

**🤖 AI Agent:**
> Take Grab


## ❓ FAQ

**Q: How does the engine decide between MRT and Grab?**
The engine evaluates if the cost per minute saved by taking a Grab is worth the urgency. If you are in a storm or have high time sensitivity, it recommends Grab. Otherwise, it checks if the extra cost is less than $2 per minute saved.

**Q: Does weather affect the Grab cost?**
Yes, you can use `get_weather_surge_multiplier` to see how much the fare increases. Storms have the highest multiplier, followed by rain.

**Q: Can I check if it is currently peak hour?**
Yes, the `is_peak_hour` tool identifies if the provided 24-hour time falls within Singapore's morning or evening rush hours.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/mrt-vs-grab-decision-engine](https://vinkius.com/ai-agent-connect/mrt-vs-grab-decision-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MRT vs Grab Decision Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mrt-vs-grab-decision-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MRT vs Grab Decision Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mrt-vs-grab-decision-engine": {
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

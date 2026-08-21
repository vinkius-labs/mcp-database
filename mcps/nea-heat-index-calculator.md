# NEA Heat Index Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/nea-heat-index-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate heat stress, hydration needs, and safety scores using NEA methodology.

## Description
This MCP server provides deterministic heat stress metrics based on the Singapore National Environment Agency (NEA) methodology. It uses the Rothfusz regression equation to calculate the heat index, helping users understand how temperature and humidity combine to affect physical safety. Use `calculate_heat_metrics` to get a full profile including heat stress category and hydration needs, `get_hydration_guidelines` for specific fluid intake advice, or `get_activity_safety_summary` to assess risks for outdoor events.


## Available Tools (3)
- **calculate_heat_metrics**: Calculates the comprehensive heat stress profile for a specific environmental condition
- **get_activity_safety_summary**: Provides a high-level safety assessment for planning outdoor events
- **get_hydration_guidelines**: Retrieves specific hydration advice based on a known Heat Index level


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NEA Heat Index Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the heat stress profile for 34°C and 80% humidity?"

**🤖 AI Agent:**
> The heat index is 42.5°C, which falls into the Extreme Caution category. It is recommended to drink 1.5 liters of water per hour, and the outdoor activity safety score is 45.

---

**👤 You:**
> "Is it safe to run outside if the temperature is 28°C and humidity is 60%?"

**🤖 AI Agent:**
> The heat index is 31.2°C, which is categorized as Normal. Conditions are comfortable for most activities.

---

**👤 You:**
> "Give me hydration advice for a heat index of 55°C."

**🤖 AI Agent:**
> At a heat index of 55°C, you are in the Danger category. You must drink at least 3.0 liters of water per hour and avoid all outdoor exertion.


## ❓ FAQ

**Q: What methodology does this tool use?**
The tool uses the Singapore National Environment Agency (NEA) methodology, specifically utilizing a simplified Rothfusz regression equation optimized for tropical climates.

**Q: How can I plan an outdoor event safely?**
You can use the `get_activity_safety_summary` tool to receive a high-level assessment, including a risk level and practical activity recommendations.

**Q: Does this tool provide hydration advice?**
Yes, you can use `get_hydration_guidelines` to get specific advice and the minimum liters of water required per hour based on the current heat index.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/nea-heat-index-calculator](https://vinkius.com/ai-agent-connect/nea-heat-index-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NEA Heat Index Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nea-heat-index-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NEA Heat Index Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nea-heat-index-calculator": {
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

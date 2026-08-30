# Emergency Planning Zones MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/emergency-planning-zones)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [emergency-management](../categories/emergency-management.md)

Calculates protective action distances and emergency response strategies for chemical hazards.

## Description
This MCP server provides critical tools for chemical facility safety management. It enables AI agents to determine protective action distances using `calculate_protective_distances`, assess human impact via `analyze_population_impact`, select optimal response strategies with `determine_protective_strategy`, and prepare communication protocols through `generate_notification_plan`.


## Available Tools (4)
- **analyze_population_impact**: Evaluates how many people are at risk within the calculated hazard zones
- **calculate_protective_distances**: Determines the specific distances for safety actions based on the severity of the hazard
- **determine_protective_strategy**: Selects the optimal response (Evacuation vs. Shelter-in-Place) for a specific zone
- **generate_notification_plan**: Defines what alerts must be sent and to whom based on the threat level


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Emergency Planning Zones** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the protective distance for a High severity rapid rupture release."

**🤖 AI Agent:**
> The protective action distance is 5.2 km, with Shelter-in-Place as the primary action.

---

**👤 You:**
> "What is the best strategy for 5000 people at risk with a response capability of 0.8?"

**🤖 AI Agent:**
> The recommended action is Evacuation, with an estimated execution time of 2.5 hours.

---

**👤 You:**
> "Generate a notification plan for a High severity threat affecting 10000 people where evacuation is required."

**🤖 AI Agent:**
> The notification plan includes SMS, sirens, and radio alerts with a High priority level.


## ❓ FAQ

**Q: How does the tool determine the safety radius?**
The `calculate_protective_distances` tool determines the radius based on the provided hazard severity and the specific release scenario.

**Q: Can I use this to plan evacuation routes?**
While it doesn't map physical roads, `generate_notification_plan` provides message templates that include evacuation instructions when required.

**Q: What data is needed for population analysis?**
You need to provide the protective action distance and a population density map as a JSON string to `analyze_population_impact`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/emergency-planning-zones](https://vinkius.com/ai-agent-connect/emergency-planning-zones)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Emergency Planning Zones** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `emergency-planning-zones` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Emergency Planning Zones** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emergency-planning-zones": {
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

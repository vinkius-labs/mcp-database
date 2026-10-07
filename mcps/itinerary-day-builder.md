# Itinerary Day Builder MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/itinerary-day-builder)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Constructs feasible daily travel plans by reconciling attraction hours, visit durations, and travel times.

## Description
This MCP server acts as a sophisticated scheduling engine for travelers. It uses tools like `build_optimized_itinerary` to generate logical daily plans that respect attraction operating hours and travel latency. By utilizing `get_attraction_details` and `calculate_travel_time`, it ensures every stop is physically possible within a user's availability window. You can also use `validate_itinerary` to verify if a planned sequence of locations is feasible.


## Available Tools (4)
- **build_optimized_itinerary**: Generates the best possible schedule based on a user's desired locations and time constraints
- **get_attraction_details**: Retrieves the specific operating constraints and characteristics of a single attraction
- **calculate_travel_time**: Determines the time required to move between two points
- **validate_itinerary**: Checks if a proposed sequence of attractions is physically and logically possible


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Itinerary Day Builder** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Build me an itinerary for attractions A1, B2, and C3 starting at 09:00 and ending at 18:00."

**🤖 AI Agent:**
> Your optimized itinerary is: 09:00 - 10:30: Attraction A1, 11:00 - 13:00: Attraction B2, 13:30 - 15:30: Attraction C3.

---

**👤 You:**
> "Is it possible to visit the Grand Museum and the Central Park between 10:00 and 14:00?"

**🤖 AI Agent:**
> Yes, that itinerary is valid and fits within your time window.

---

**👤 You:**
> "What are the opening hours for attraction ID 'museum_01'?"

**🤖 AI Agent:**
> The museum is open from 09:00 to 18:00.


## ❓ FAQ

**Q: How does the engine ensure the itinerary is feasible?**
The engine uses `validate_itinerary` to check that all visits occur within attraction operating hours and that the total time for visits and travel fits within your specified availability window.

**Q: Can I prioritize specific locations?**
Yes, the `build_optimized_itinerary` tool prioritizes attractions based on their assigned importance, ensuring high-priority locations are included whenever possible.

**Q: How is travel time calculated?**
Travel time is determined by the `calculate_travel_time` tool, which uses a transit matrix to find the exact minutes required to move between specific attraction IDs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/itinerary-day-builder](https://vinkius.com/en/ai-agent-connect/itinerary-day-builder)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Itinerary Day Builder** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `itinerary-day-builder` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Itinerary Day Builder** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "itinerary-day-builder": {
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

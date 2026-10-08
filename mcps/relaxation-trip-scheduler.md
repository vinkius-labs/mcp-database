# Relaxation Trip Scheduler MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/relaxation-trip-scheduler)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates low-pressure, restorative travel itineraries by balancing activities with essential downtime.

## Description
This MCP server helps users design restorative travel plans that prioritize well-being. It uses specialized logic to ensure a proper restoration ratio between active engagements and rest blocks. You can use `get_available_slots` to find free time, `calculate_transition_requirements` to determine necessary buffers between events, `validate_itinerary_balance` to ensure the trip remains low-pressure, and `build_daily_agenda` to visualize a structured chronological view of your day.


## Available Tools (4)
- **build_daily_agenda**: Generate a structured, chronological view of a single day's schedule
- **calculate_transition_requirements**: Determine the necessary time gap between two specific scheduled events
- **get_available_slots**: Identify potential windows of time within a specific date range
- **validate_itinerary_balance**: Check if a proposed schedule meets the "low-pressure" threshold


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Relaxation Trip Scheduler** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find available time slots for my trip from 2024-06-01 to 2024-06-05."

**🤖 AI Agent:**
> I found several available slots: June 1st from 09:00 to 12:00, June 2nd from 14:00 to 17:00, and June 3rd from 10:00 to 15:00.

---

**👤 You:**
> "Is my itinerary balanced for a relaxing trip?"

**🤖 AI Agent:**
> No, the itinerary is currently too high-pressure because there are too many high-intensity activities without sufficient rest blocks.

---

**👤 You:**
> "Show me my schedule for June 2nd."

**🤖 AI Agent:**
> Your schedule for June 2nd is: 08:00-09:00 Breakfast, 09:00-09:30 Transition/Buffer, 09:30-11:30 Leisurely Walk, 11:30-12:00 Transition/Buffer, 12:00-13:00 Lunch.


## ❓ FAQ

**Q: How does the tool ensure a low-pressure trip?**
The tool uses `validate_itinerary_balance` to check the restoration ratio, ensuring there is enough rest and travel buffer time between activities.

**Q: Can I see a visual timeline of my day?**
Yes, you can use `build_daily_agenda` to generate a structured, chronological view of your schedule, including transition periods.

**Q: How are travel buffers calculated?**
The `calculate_transition_requirements` tool calculates the necessary gap based on the travel mode and the intensity of the preceding activity.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/relaxation-trip-scheduler](https://vinkius.com/en/ai-agent-connect/relaxation-trip-scheduler)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Relaxation Trip Scheduler** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `relaxation-trip-scheduler` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Relaxation Trip Scheduler** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "relaxation-trip-scheduler": {
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

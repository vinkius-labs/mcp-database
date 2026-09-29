# School Run Route Timetable MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/school-run-route-timetable)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [transportation](../categories/transportation.md)

Generates optimized departure timelines for school transport routes.

## Description
This MCP server provides a specialized scheduling engine for school transport. It calculates precise departure times by working backwards from a school arrival deadline, accounting for travel durations between stops and mandatory boarding buffers. Use `calculate_departure_schedule` to build a full timetable, `validate_route_feasibility` to check if a route is possible, `get_return_trip_timetable` for post-arrival journeys, and `optimize_buffer_allocation` to distribute slack time across stops.


## Available Tools (4)
- **calculate_departure_schedule**: Generates a complete, ordered timetable of departure times for a specific sequence of stops to meet a school arrival deadline
- **get_return_trip_timetable**: Calculates the timing for the vehicle's journey after the school drop-off/arrival is completed
- **optimize_buffer_allocation**: Suggests how to distribute available "slack time" across different stops to ensure a more comfortable schedule
- **validate_route_feasibility**: Checks if a proposed sequence of stops and durations is physically possible within a specific timeframe


## 💬 Prompt Examples

Here are some examples of how you can interact with the **School Run Route Timetable** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a timetable for stops at 123 Maple St and 456 Oak St, arriving at school by 08:30. Leg durations are 10 and 15 minutes, and each stop has a 5 minute buffer."

**🤖 AI Agent:**
> The departure times are: 123 Maple St at 07:50 and 456 Oak St at 08:05.

---

**👤 You:**
> "Is it feasible to visit 3 stops with 10 minute legs and 5 minute buffers, arriving at school at 08:00, if the earliest departure is 07:00?"

**🤖 AI Agent:**
> Yes, the route is feasible with a total duration of 45 minutes.

---

**👤 You:**
> "Calculate the return trip starting from school at 15:00, with a 20 minute leg to the first stop and a 10 minute leg to the depot."

**🤖 AI Agent:**
> The return schedule is: First stop at 15:20 and Depot at 15:30.


## ❓ FAQ

**Q: How do I generate a full timetable?**
You can use the `calculate_departure_schedule` tool by providing the pickup addresses, the school arrival deadline, leg durations, and stop buffers.

**Q: Can I check if my route is physically possible?**
Yes, the `validate_route_feasibility` tool checks if the sequence of stops and durations fits within your required timeframe.

**Q: How can I add extra safety time to my stops?**
Use the `optimize_buffer_allocation` tool to distribute available slack time across your stops using either an even or front-loaded distribution.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/school-run-route-timetable](https://vinkius.com/en/ai-agent-connect/school-run-route-timetable)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **School Run Route Timetable** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `school-run-route-timetable` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **School Run Route Timetable** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "school-run-route-timetable": {
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

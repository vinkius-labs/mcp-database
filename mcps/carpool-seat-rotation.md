# Carpool Seat Rotation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/carpool-seat-rotation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [transportation](../categories/transportation.md)

Automated rider assignment and vehicle scheduling based on capacity and fairness.

## Description
This MCP server automates the complex process of assigning riders to vehicles and specific driving days. It optimizes seat capacity, respects pickup constraints, and ensures equitable distribution using rotation history. Use `calculate_daily_assignments` to generate full schedules, `get_rider_availability` to check passenger constraints, `validate_vehicle_capacity` to monitor seat limits, and `get_fairness_score` to prioritize riders who have been assigned fewer seats in the past.


## Available Tools (4)
- **calculate_daily_assignments**: Generates the complete schedule of riders, vehicles, and drivers for a given period
- **get_fairness_score**: Calculates a priority score for a rider based on their previous assignments
- **get_rider_availability**: Determines if a specific rider can be accommodated on a specific date
- **validate_vehicle_capacity**: Checks if adding a rider to a specific vehicle on a specific day would exceed the vehicle's limit


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Carpool Seat Rotation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a daily assignment schedule for these riders, vehicles, and drivers."

**🤖 AI Agent:**
> The schedule for July 10th includes 3 vehicles with 12 riders assigned and 2 unassigned riders due to capacity limits.

---

**👤 You:**
> "Is rider R-123 available to travel on 2024-08-15?"

**🤖 AI Agent:**
> No, rider R-123 is not available on 2024-08-15 based on their specified availability constraints.

---

**👤 You:**
> "What is the priority score for rider R-456?"

**🤖 AI Agent:**
> The priority score for rider R-456 is 5, indicating they have been assigned seats 5 times previously.


## ❓ FAQ

**Q: How does the system ensure fairness among riders?**
The system uses `get_fairness_score` to calculate a priority score. Riders with lower historical assignment counts are prioritized for available seats to ensure equitable rotation.

**Q: Can I check if a vehicle has enough space for a new rider?**
Yes, you can use the `validate_vehicle_capacity` tool to check the remaining seats in a specific vehicle against its maximum capacity.

**Q: How are daily schedules generated?**
You can generate a complete schedule of riders, vehicles, and drivers by calling `calculate_daily_assignments` with the necessary rider, vehicle, and driver data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/carpool-seat-rotation](https://vinkius.com/en/ai-agent-connect/carpool-seat-rotation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Carpool Seat Rotation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `carpool-seat-rotation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Carpool Seat Rotation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "carpool-seat-rotation": {
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

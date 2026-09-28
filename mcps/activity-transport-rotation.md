# Activity Transport Rotation MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/activity-transport-rotation)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [transportation](../categories/transportation.md)

Optimizes driver assignments and vehicle routing for group activities.

## Description
This MCP server manages logistics for group transport by balancing driver workload and vehicle capacity. It uses `get_driver_roster` to ensure equitable driver rotation, `get_pickup_timeline` to generate safe transit schedules with travel buffers, `get_contact_sheet` for essential participant directories, and `get_backup_transport_plan` to handle capacity shortfalls.


## Available Tools (4)
- **get_contact_sheet**: Provides a directory of essential contact information for drivers and participants
- **get_driver_roster**: Provides a scheduled list of drivers assigned to specific activity dates
- **get_pickup_timeline**: Generates a chronological sequence of pickup events and estimated arrival times
- **get_backup_transport_plan**: Identifies alternative transport options when the primary roster fails


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Activity Transport Rotation** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you show me the driver assignments for the upcoming activity dates?"

**🤖 AI Agent:**
> The assigned drivers for the requested dates are Driver A, Driver B, and Driver C.

---

**👤 You:**
> "What is the pickup schedule for trip ID 123 starting from the main station?"

**🤖 AI Agent:**
> The pickup events are: 08:00 AM at Main Station, 08:15 AM at North Gate, and 08:30 AM at South Terminal.

---

**👤 You:**
> "I need the contact details for the participants in activity 456."

**🤖 AI Agent:**
> The contacts for activity 456 are: John Doe (Driver) - 555-0101, Jane Smith (Participant) - 555-0102.


## ❓ FAQ

**Q: How does the server ensure driver fairness?**
The `get_driver_roster` tool applies rotation rules to distribute assignments evenly among approved drivers, preventing burnout.

**Q: What happens if there aren't enough seats for everyone?**
You can use `get_backup_transport_plan` to identify alternative drivers or contingency plans when a capacity shortfall is detected.

**Q: Does the timeline include traffic delays?**
Yes, `get_pickup_timeline` allows for a travel buffer to be added to transit durations to account for unexpected delays.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/activity-transport-rotation](https://vinkius.com/en/ai-agent-connect/activity-transport-rotation)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Activity Transport Rotation** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `activity-transport-rotation` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Activity Transport Rotation** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "activity-transport-rotation": {
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

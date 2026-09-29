# Accessible Vehicle Transfer Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/accessible-vehicle-transfer-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [logistics](../categories/logistics.md)

Coordinates mobility equipment transfers by checking vehicle compatibility, staff availability, and scheduling conflicts.

## Description
This MCP server provides a specialized planning engine for coordinating the logistics of moving individuals using mobility equipment between vehicles. It ensures safe transfers by using `find_compatible_vehicles` to match equipment dimensions with vehicle clearances, `validate_assistance_availability` to confirm staff presence, `calculate_transfer_schedule` to build optimized timelines with necessary buffers, and `detect_transfer_conflicts` to identify overlapping appointments or resource shortages.


## Available Tools (4)
- **detect_transfer_conflicts**: Identifies overlapping appointments, resource shortages, or physical mismatches in a proposed plan
- **find_compatible_vehicles**: Identifies which vehicles in the fleet can physically accommodate a specific piece of mobility equipment
- **calculate_transfer_schedule**: Generates a proposed timeline for a sequence of transfers, including necessary buffers
- **validate_assistance_availability**: Checks if the required level of human assistance is available during a requested window


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accessible Vehicle Transfer Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Which vehicles can fit a wheelchair that is 60cm wide, 100cm long, and 110cm high?"

**🤖 AI Agent:**
> The following vehicles are compatible: Vehicle_ID_A1, Vehicle_ID_B2.

---

**👤 You:**
> "Check if specialized assistance is available tomorrow between 10:00 AM and 12:00 PM."

**🤖 AI Agent:**
> Yes, specialized assistance is available with 2 staff members currently scheduled.

---

**👤 You:**
> "Are there any conflicts in my current transfer plan?"

**🤖 AI Agent:**
> No conflicts detected. All vehicle assignments, assistance levels, and time windows are valid.


## ❓ FAQ

**Q: How does the system ensure a wheelchair will fit in a vehicle?**
The `find_compatible_vehicles` tool compares the width, height, and length of the mobility equipment against the door opening and internal floor space of the vehicle fleet.

**Q: Can I check if staff are available for a specific time?**
Yes, you can use `validate_assistance_availability` to check if the required assistance level is available during your requested time window.

**Q: How are scheduling delays handled?**
The `calculate_transfer_schedule` tool incorporates mandatory transfer buffers between consecutive moves to prevent delays from causing missed appointments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/accessible-vehicle-transfer-planner](https://vinkius.com/en/ai-agent-connect/accessible-vehicle-transfer-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accessible Vehicle Transfer Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accessible-vehicle-transfer-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accessible Vehicle Transfer Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accessible-vehicle-transfer-planner": {
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

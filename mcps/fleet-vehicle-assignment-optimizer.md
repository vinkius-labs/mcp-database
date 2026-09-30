# Fleet Vehicle Assignment Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/fleet-vehicle-assignment-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fleet-management](../categories/fleet-management.md)

Assigns service jobs to fleet vehicles based on payload, range, and driver authorization.

## Description
This MCP server provides tools to optimize logistical operations by matching service jobs to the most suitable fleet vehicles. It handles complex constraints including payload capacity, travel range, driver certifications, and maintenance schedules. Use `assign_fleet_jobs` to distribute a batch of jobs across the fleet, `check_driver_eligibility` to verify driver credentials, `validate_vehicle_availability` to check scheduling conflicts, and `calculate_remaining_capacity` to monitor leftover resources.


## Available Tools (4)
- **calculate_remaining_capacity**: 
- **check_driver_eligibility**: 
- **validate_vehicle_availability**: 
- **assign_fleet_jobs**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fleet Vehicle Assignment Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Assign these jobs to my fleet: jobs=[{'id': 'j1', 'weight': 500, 'distance': 50}, {'id': 'j2', 'weight': 200, 'distance': 30}], vehicles=[{'id': 'v1', 'capacity': 1000, 'range': 200, 'class': 'Medium'}], drivers=[{'id': 'd1', 'classes': ['Medium']}]"

**🤖 AI Agent:**
> Job j1 has been assigned to vehicle v1 with driver d1. Job j2 has also been assigned to vehicle v1 with driver d1. Remaining capacity for v1 is 300kg payload and 120km range.

---

**👤 You:**
> "Is driver d1 eligible to drive a Heavy class vehicle?"

**🤖 AI Agent:**
> No, driver d1 is only authorized for Medium and Light vehicle classes.

---

**👤 You:**
> "Check if vehicle v1 is available from 2024-05-01T10:00:00Z to 2024-05-01T14:00:00Z."

**🤖 AI Agent:**
> Vehicle v1 is available for the requested time window.


## ❓ FAQ

**Q: How does the assignment logic handle driver qualifications?**
The system uses `check_driver_eligibility` to ensure that a driver's specific vehicle class authorization matches the vehicle they are being assigned to.

**Q: Can I check if a vehicle is available for a specific time window?**
Yes, you can use the `validate_vehicle_availability` tool to check if a vehicle is free or if it conflicts with scheduled maintenance blackouts.

**Q: How do I know if a vehicle has enough space for a heavy load?**
You can use `calculate_remaining_capacity` to determine the leftover payload and range of a vehicle after previous assignments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/fleet-vehicle-assignment-optimizer](https://vinkius.com/en/ai-agent-connect/fleet-vehicle-assignment-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fleet Vehicle Assignment Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fleet-vehicle-assignment-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fleet Vehicle Assignment Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fleet-vehicle-assignment-optimizer": {
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

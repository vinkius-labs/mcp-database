# Honeywell Forge MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/honeywell-forge)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Connect Honeywell Forge to any AI agent via MCP.



## Available Tools (11)
- **acknowledge_alarm**: Acknowledgment does not resolve or clear the underlying condition—it simply records that a human has reviewed the alarm and is aware of it. This updates the alarm state from "unacknowledged" to "acknowledged" in the Forge audit log, which is important for compliance and incident-tracking workflows. Provide the exact alarm ID as returned by get_alarms. Use this during incident response to track which alarms have been seen by the operations team.

Acknowledge an active alarm in Honeywell Forge
- **get_alarms**: Alarms cover a wide range of conditions: security breaches (door forced, tailgating), fire and life safety (smoke detector activation, pull station), HVAC faults, and system health warnings. Each alarm record includes severity level, timestamp, source device, description, and acknowledgment status. Optionally filter by building_id to scope results to a single site. Use this to triage active incidents, audit historical events, or identify recurring fault patterns.

List active and historical alarms across all buildings or a specific building
- **get_building_details**: Returns comprehensive metadata including HVAC zones, floor plans, linked subsystems (access control, fire life safety, video surveillance), energy targets, and operating schedules. Use this when you need a deep-dive view of a single site before performing operations like checking alarms or querying energy usage.

Get detailed information about a specific Honeywell Forge building
- **get_door_status**: The response includes whether the door is currently open or closed, locked or unlocked, and any active fault conditions such as "door held open" or "forced open". This is a read-only, point-in-time snapshot—use it to verify the physical state of a door before granting access or investigating a security event.

Get the real-time status of a specific door or access point
- **get_energy_usage**: Returns aggregated consumption data including total kWh, cost estimates, demand peaks, and breakdowns by subsystem (HVAC, lighting, plug loads). Metrics may be presented as time-series data points with timestamps, allowing trend analysis and comparison against energy budgets. Use this to monitor sustainability KPIs, identify wasteful consumption patterns, or prepare energy audit reports for facility managers.

Get energy consumption data for a specific building
- **get_temperature_data**: Returns data points including zone temperature, setpoint targets, humidity levels, and HVAC equipment status (compressor running, valve position, fan speed). This data is essential for thermal comfort analysis, energy optimization, and proactive maintenance—such as identifying zones that consistently deviate from setpoints or detecting equipment degradation before failure. Use this to diagnose comfort complaints or validate HVAC scheduling changes.

Get temperature and HVAC sensor data for a specific building
- **list_access_points**: An access point represents a physical entry device—door, gate, turnstile, or barrier—managed by the Forge access control subsystem. Each record includes the access point ID, name, current lock state, door status (open/closed/forced), assigned access level, and the zone it belongs to. Use this to audit physical security surfaces before running lock/unlock commands or investigating door-forced alarm events.

List all access control points (doors, gates, turnstiles) for a building
- **list_buildings**: Each record contains the building identifier, name, address, operational status, and metadata such as time zone and total floor area. Use this tool as the entry point for any building-centric workflow—once you have the building ID you can drill down into access points, alarms, energy metrics, or video feeds.

List all buildings registered in Honeywell Forge
- **list_video_feeds**: Each record represents a camera or NVR channel with metadata including camera name, location within the building, stream URL (RTSP or HLS), resolution, current online/offline status, and recording mode (continuous, motion-triggered, scheduled). Use this to discover which cameras are available for live viewing or forensic review, and to map camera IDs to physical locations before correlating video with alarm events.

List available video surveillance feeds for a building
- **lock_door**: The door will immediately engage its locking mechanism and transition to a secured state. Only authorized credentials holders can override this lock via normal badge or PIN access. Use this when securing a building after hours, during a lockdown event, or to enforce temporary access restrictions. Confirm the door identity with list_access_points before executing.

Lock a specific door or access point in Honeywell Forge
- **unlock_door**: The door will disengage its lock and enter a free-access state until explicitly re-locked or returned to its scheduled access control mode. Use this for emergency egress, visitor accommodation, or maintenance access. Always verify the correct access point ID before unlocking to avoid unintended security gaps.

Unlock a specific door or access point in Honeywell Forge






## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/honeywell-forge](https://vinkius.com/mcp/honeywell-forge)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Honeywell Forge** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `honeywell-forge` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Honeywell Forge** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "honeywell-forge": {
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

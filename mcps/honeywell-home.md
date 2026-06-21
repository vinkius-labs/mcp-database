# Honeywell Home MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/honeywell-home)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Connect Honeywell Home to any AI agent via MCP.



## Available Tools
- **get_air_quality**: Returns data such as PM2.5 particulate levels, VOC (volatile organic compounds) index, CO2 concentration, humidity, and overall air quality rating. Use this to assess whether ventilation or air purification is needed.

Get air quality readings from a Honeywell Home device
- **arm_system**: Choose the arming mode: "stay" (arms perimeter sensors like doors and windows but ignores interior motion detectors, ideal when occupants are home) or "away" (arms all sensors including interior motion, ideal when the property is empty). After arming, verify the new state with get_security_status.

Arm the Honeywell Home security system
- **get_camera_snapshot**: The returned data includes an image URL or base64-encoded snapshot. This is useful for a quick visual check of a room or area without streaming live video. Provide the camera device_id from get_devices.

Capture a snapshot image from a Honeywell Home camera
- **get_camera_status**: Use the device_id obtained from get_devices. Useful for quickly verifying that a security camera is active and functioning before reviewing footage.

Get the status of a Honeywell Home camera
- **get_devices**: Provide a locationId obtained from the get_locations tool. If no locationId is supplied, returns all devices across all locations. Useful for inventorying connected hardware.

List all devices at a Honeywell Home location
- **disarm_system**: Use this when returning home or when authorized personnel need access. After disarming, verify the new state with get_security_status.

Disarm the Honeywell Home security system
- **get_locations**: ) associated with the authenticated Honeywell Home account. Each location contains metadata such as name, address, timezone, and the list of devices registered at that address. Use this tool first to discover location IDs before querying devices or security systems.

List all registered Honeywell Home locations
- **get_security_status**: Returns whether the system is armed (stay or away mode), disarmed, or in alarm, along with the status of connected sensors (doors, windows, motion detectors). Provide a location_id from get_locations.

Get the current status of the Honeywell Home security system
- **update_setpoint**: You can adjust the heat setpoint (minimum temperature), the cool setpoint (maximum temperature), or switch the operating mode (heat, cool, auto, off). Only send the parameters you want to change. After modifying setpoints, verify the change with get_thermostat_data. Use this to help users regulate heating and cooling remotely.

Adjust the temperature setpoint on a Honeywell thermostat
- **get_thermostat_data**: Use this to check what temperature the thermostat is targeting and whether the HVAC system is actively running.

Get detailed thermostat readings and configuration






## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/honeywell-home](https://vinkius.com/mcp/honeywell-home)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Honeywell Home** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `honeywell-home` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Honeywell Home** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "honeywell-home": {
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

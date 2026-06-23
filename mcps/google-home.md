# Google Home MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-home)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Control Google Nest devices — thermostats, cameras, and doorbells via Smart Device Management (SDM) API.

## Description
Connect to **Google Nest devices** via the Smart Device Management (SDM) API and control your smart home from any AI agent. Manage thermostats, view camera feeds, and interact with doorbells.

### What you can do

- **List Devices** — See all your Nest thermostats, cameras, doorbells, and displays
- **Thermostat Control** — Set mode (Heat/Cool/Off), adjust temperatures, enable eco mode, and control fan timer
- **Camera Streaming** — Generate live RTSP or WebRTC stream URLs from Nest cameras and doorbells
- **Doorbell Management** — View doorbell camera feeds and stream events
- **Structure & Rooms** — Browse your home's structures and room organization
- **Device Details** — Get full device state including all traits and current settings

### How it works

1. Subscribe to this server
2. Obtain OAuth 2.0 access token and Project ID from Google Device Access console
3. Start controlling your Nest devices from Claude, Cursor, or any MCP-compatible client

Your AI becomes a smart home assistant, helping you manage climate, security, and monitoring.

### Who is this for?

- **Smart Home Owners** — control thermostats, view cameras, and manage Nest devices from AI assistants
- **Home Automation Enthusiasts** — integrate Nest devices into broader automation workflows
- **Property Managers** — monitor and adjust climate across multiple properties remotely
- **Security-Conscious Users** — check camera feeds and doorbell streams on demand
- **Energy-Conscious Users** — optimize thermostat settings and eco mode for energy savings


## Available Tools (12)
- **generate_camera_stream**: The stream token is temporary and should be used immediately. Stop the stream when done.

Generate a live camera stream URL from a Nest camera or doorbell
- **get_device**: Use device ID from list_devices or device name.

Get details for a specific Google Nest device
- **list_devices**: Shows device types, traits, and room assignments.

USE WHEN:
- User wants to see all their Nest devices
- User needs to find device IDs for other commands
- User is exploring their smart home setup
- User asks "what Nest devices do I have"

EXAMPLES:
- "List all my Nest devices" → call with no params
- "Show my smart home devices" → call with no params
- "What Nest devices are connected?" → call with no params

List all Google Nest devices in your home
- **list_rooms**: Useful for understanding device locations and room organization.

List all rooms in a specific structure
- **list_structures**: Each structure contains rooms and devices.

List all structures (homes) in your Google Nest account
- **set_fan_timer**: Turns the fan on for a specified duration. Duration is optional and defaults to the thermostat setting.

Set the fan timer on a Nest thermostat
- **set_thermostat_cool**: Use this when the thermostat is in COOL or HEATCOOL mode.

Set the cooling temperature on a Nest thermostat
- **set_thermostat_eco**: This is a manual override of the eco/eco-friendly temperature settings.

Set Nest thermostat to eco mode for energy savings
- **set_thermostat_heat**: Use this when the thermostat is in HEAT or HEATCOOL mode.

Set the heating temperature on a Nest thermostat
- **set_thermostat_mode**: Supported modes: HEAT, COOL, HEATCOOL, OFF. Use device ID from list_devices to target a specific thermostat.

USE WHEN:
- User wants to change thermostat mode
- User asks to turn heating/cooling on or off
- User wants to switch thermostat operating mode
- User says "set thermostat to heat/cool/off"

PARAMETERS:
- device_id (REQUIRED): Thermostat device ID
- mode (REQUIRED): One of HEAT, COOL, HEATCOOL, or OFF

EXAMPLES:
- "Set thermostat to heat mode" → call with device_id, mode="HEAT"
- "Turn off the thermostat" → call with device_id, mode="OFF"
- "Set thermostat to cool" → call with device_id, mode="COOL"

Set the mode of a Nest thermostat
- **set_thermostat_range**: Useful for HEATCOOL mode to define the comfort range.

Set both heating and cooling temperatures on a Nest thermostat
- **stop_camera_stream**: Use the stream token returned from generate_camera_stream to properly terminate the stream session.

Stop an active camera stream from a Nest camera or doorbell


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Home** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Nest devices and show me what thermostats I have."

**🤖 AI Agent:**
> I found 4 Nest devices in your home: 1) Nest Thermostat (Living Room) — currently in HEAT mode at 21°C, 2) Nest Camera (Front Door) — streaming ready, 3) Nest Doorbell (Backyard) — battery powered, 4) Nest Hub (Kitchen). Would you like to adjust any thermostat settings?

---

**👤 You:**
> "Set my living room thermostat to 22°C heating mode."

**🤖 AI Agent:**
> Setting thermostat to HEAT mode at 22°C... Done! Your Living Room Nest Thermostat is now heating to 22°C. Current room temperature is 19.5°C. The HVAC system has activated and is heating. Estimated time to reach target: approximately 15 minutes.

---

**👤 You:**
> "Show me the live feed from my front door camera."

**🤖 AI Agent:**
> Generating live stream URL for Front Door Nest Camera... Stream URL generated (RTSP). The stream is active for the next 5 minutes. Use any RTSP-compatible player to view the live feed. Remember to stop the stream when done to free up resources. Would you like me to stop the stream?


## ❓ FAQ

**Q: What Google Nest devices are supported by this API?**
The SDM API supports: Nest Thermostats (Nest Learning Thermostat, Nest Thermostat E, Nest Thermostat 2020), Nest Cameras (legacy, battery, wired, with spotlight), Nest Doorbells (legacy battery, wired, battery), and Nest Hub displays. Each device exposes specific traits (e.g., ThermostatMode, CameraLiveStream) that can be queried and controlled.

**Q: How do I get OAuth 2.0 credentials for the Google SDM API?**
Visit the [**Google Device Access console**](https://console.nest.google.com/device-access/) and create a project. You'll receive a Project ID. Then, set up OAuth 2.0 credentials in Google Cloud Console, link them to your Device Access project, and complete the OAuth flow to obtain an access token. The token expires after 1 hour and must be refreshed.

**Q: Can I control multiple thermostats in different locations?**
Yes! The API returns all devices across all structures and rooms in your project. Use `list_devices` to see all thermostats with their room assignments, then use each device's unique ID to control them individually. You can set different modes and temperatures for each thermostat.

**Q: How long do camera stream URLs last?**
Camera stream URLs (both RTSP and WebRTC) are temporary and typically expire after 5 minutes. The stream token returned in the response should be used immediately and the stream should be stopped with `stop_camera_stream` when no longer needed to free up device resources.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-home](https://vinkius.com/mcp/google-home)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Google Home** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `google-home` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Google Home** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "google-home": {
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

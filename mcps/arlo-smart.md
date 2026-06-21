# Arlo Smart MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arlo-smart)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/arlo-smart-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/arlo-smart-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Control Arlo security cameras — view recordings, arm/disarm devices, and manage security modes via Arlo Smart API.

## Description
Connect to **Arlo Smart API** and control your Arlo security cameras, review recordings, and manage security modes from any AI agent. Arm and disarm cameras, browse recorded videos, and monitor your home security through natural language commands.

### What you can do

- **Device Discovery** — List all Arlo devices including basestations, cameras, doorbells, and floodlights
- **Recording Access** — Browse and download recorded videos from any camera with presigned URLs
- **Recent Activity** — Quickly check today's recordings across all cameras
- **Security Modes** — View and change automation modes (armed, disarmed, custom modes)
- **Arm/Disarm** — Enable or disable security monitoring on individual devices or basestations
- **Recording Management** — Delete old recordings to free up cloud storage space
- **Metadata Access** — Get detailed recording metadata including duration, timestamps, and download links

### How it works

1. Subscribe to this server
2. Enter your Arlo authentication token
3. Start controlling your Arlo security system from Claude, Cursor, or any MCP-compatible client

Your AI becomes a security assistant, helping you monitor recordings, manage security modes, and protect your home.

### Who is this for?

- **Homeowners** — monitor security cameras and review recordings through natural language
- **Property Managers** — manage Arlo security systems across multiple properties
- **Security-Conscious Users** — arm/disarm cameras and check recent activity remotely
- **Smart Home Enthusiasts** — integrate Arlo cameras into broader home automation workflows
- **Travelers** — check home security recordings and adjust security modes while away


## Available Tools
- **arm_arlo_device**: This enables motion detection and recording for the device.

USE WHEN:
- User wants to enable security monitoring
- User asks to "arm the cameras" or "turn on security"
- User wants to enable motion detection and recording
- User is leaving home and wants security enabled

PARAMETERS:
- deviceId (REQUIRED): Arlo device ID to arm

EXAMPLES:
- "Arm the front door camera" → call with deviceId="FRONT_DOOR_ID"
- "Enable security on the backyard camera" → call with deviceId="BACKYARD_ID"
- "Arm the basestation" → call with deviceId="BASESTATION_ID"

Arm an Arlo device (enable security monitoring)
- **delete_arlo_recordings**: This action is permanent and cannot be undone.

USE WHEN:
- User wants to free up cloud storage space
- User wants to remove old or unwanted recordings
- User asks to "delete recordings from [date]"
- User is managing their Arlo cloud storage

PARAMETERS:
- recordings (REQUIRED): JSON array of recording objects to delete (from get_arlo_recordings response)

EXAMPLES:
- "Delete these recordings" → call with recordings=[{...}]

Delete Arlo recordings from the library
- **disarm_arlo_device**: This disables motion detection and recording for the device.

USE WHEN:
- User wants to disable security monitoring
- User asks to "disarm the cameras" or "turn off security"
- User wants to disable motion detection temporarily
- User is home and wants to disable security

PARAMETERS:
- deviceId (REQUIRED): Arlo device ID to disarm

EXAMPLES:
- "Disarm the front door camera" → call with deviceId="FRONT_DOOR_ID"
- "Disable security on the backyard camera" → call with deviceId="BACKYARD_ID"
- "Disarm the basestation" → call with deviceId="BASESTATION_ID"

Disarm an Arlo device (disable security monitoring)
- **get_arlo_device_modes**: Shows whether the device is armed, disarmed, or in a custom mode.

Get the current automation modes for an Arlo device
- **get_recent_arlo_recordings**: Useful for quickly checking recent security activity.

Get recent Arlo recordings from the last 24 hours
- **get_arlo_recording_metadata**: Get detailed metadata for an Arlo recording
- **get_arlo_recordings**: Returns presigned URLs for downloading video files along with metadata like duration, device ID, and creation date.

USE WHEN:
- User wants to download or view Arlo recordings
- User needs to check what was recorded on specific dates
- User is reviewing security footage
- User asks "show me recordings from [date range]"

PARAMETERS:
- dateFrom (REQUIRED): Start date in YYYYMMDD format (e.g. 20260407)
- dateTo (REQUIRED): End date in YYYYMMDD format
- deviceId (OPTIONAL): Filter by specific device ID

EXAMPLES:
- "Get recordings from April 7 2026" → call with dateFrom="20260407", dateTo="20260407"
- "Show recordings from last week" → call with dateFrom="20260331", dateTo="20260406"
- "Get recordings for camera XYZ on April 5" → call with dateFrom="20260405", dateTo="20260405", deviceId="XYZ"

Get Arlo camera recordings for a date range
- **list_arlo_basestations**: Basestations are the central hubs that connect wireless Arlo cameras to your network.

List Arlo basestation/hub devices only
- **list_arlo_cameras**: List Arlo camera devices only
- **list_arlo_devices**: Each device includes deviceId, deviceName, deviceType, state, and connection status.

USE WHEN:
- User wants to see all their Arlo security devices
- User needs to find device IDs for other commands
- User is exploring their Arlo security setup
- User asks "what Arlo devices do I have"

EXAMPLES:
- "List all my Arlo devices" → call with no params
- "Show my Arlo security devices" → call with no params
- "What Arlo cameras and basestations do I have?" → call with no params

List all Arlo devices (basestations and cameras)
- **set_arlo_device_mode**: Common modes: mode0 (disarmed), mode1 (armed), mode2 (armed with all motion). You can also use custom mode IDs created in the Arlo app.

USE WHEN:
- User wants to arm or disarm their Arlo security system
- User wants to switch between different security modes
- User asks to "arm the cameras" or "disarm the system"
- User wants to enable/disable motion detection

PARAMETERS:
- deviceId (REQUIRED): Arlo device ID
- mode (REQUIRED): Mode identifier (mode0=disarmed, mode1=armed, mode2=armed all motion, or custom mode ID)

EXAMPLES:
- "Arm the front door camera" → call with deviceId="FRONT_DOOR_ID", mode="mode1"
- "Disarm all cameras" → call with deviceId="BASESTATION_ID", mode="mode0"
- "Set to home mode" → call with deviceId, mode="mode_custom_home"

Set the automation mode for an Arlo device


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Arlo Smart** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Arlo devices and show me which cameras I have."

**🤖 AI Agent:**
> I found 4 Arlo devices in your account: 1) Front Door (Basestation VMB5000) — connected, 2) Backyard Camera (Arlo Pro 4) — connected, 3) Garage Camera (Arlo Essential) — connected, 4) Side Door Camera (Arlo Pro 3) — connected. All devices are online and ready for security monitoring.

---

**👤 You:**
> "Show me today's recordings from all my Arlo cameras."

**🤖 AI Agent:**
> Found 5 recordings from today: 1) Backyard Camera — 2:34pm, 30s motion detected, 2) Garage Camera — 4:12pm, 15s motion detected, 3) Front Door — 5:45pm, 45s person detected, 4) Backyard Camera — 7:20pm, 20s animal detected, 5) Side Door — 8:05pm, 25s motion detected. All recordings are available for download via presigned URLs.

---

**👤 You:**
> "Arm all my Arlo cameras for when I leave the house."

**🤖 AI Agent:**
> Arming devices... Front Door basestation set to armed mode (mode1). Backyard Camera armed. Garage Camera armed. Side Door Camera armed. All cameras are now actively monitoring for motion and will record and send alerts when movement is detected.


## Installation & Usage

To install and use the **Arlo Smart** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arlo-smart](https://vinkius.com/mcp/arlo-smart)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

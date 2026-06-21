# DJI Developer MCP Server

Orchestrate DJI drones and payloads — manage flight logs, monitor device health, and handle firmware updates directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dji-developer)

## Overview
**Category:** superpower
**Tools Count:** 10

## Description
Connect your AI agents to the **DJI Developer Platform**, the industry standard for unmanned aerial systems (UAS). This MCP provides 10 tools to manage enterprise drone fleets, monitor real-time telemetry logs, and orchestrate firmware lifecycle management for aircraft and payloads.

### What you can do

- **Fleet Monitoring** — List registered aircraft and payloads to track operational readiness and hardware versions
- **Flight Orchestration** — Retrieve detailed flight logs and telemetry data for post-mission analysis and compliance
- **Hardware Intelligence** — Get granular health reports and technical specifications for any device in your DJI ecosystem
- **Firmware Lifecycle** — Check for latest firmware releases and monitor the progress of remote updates programmatically
- **Resource Management** — Manage organization structures and retrieve pilot profiles linked to your developer account

### How it works

1. Subscribe to this server
2. Log in to the [**DJI Developer Center**](https://developer.dji.com/)
3. Register your application to obtain your **App ID** and **App Key**
4. Enable the **Cloud API** or **Enterprise API** for your devices
5. Insert your credentials into the fields below to start managing your DJI fleet operations.

### Who is this for?

- **Fleet Managers** — automate the tracking of aircraft health and flight compliance across multiple sites
- **Data Analysts** — integrate drone telemetry into broader GIS and operational reporting systems
- **DevOps Engineers** — monitor remote firmware deployments and device synchronization at scale


## Available Tools
- **create_mission**: Create a new flight mission for a drone or dock
- **get_device_osd**: Retrieve real-time flight data (OSD)
- **get_device_status**: Get the online status and basic state of a drone
- **get_firmware_info**: Check firmware versions for a device
- **get_hms_stats**: Retrieve health management system (HMS) alerts
- **get_media_upload_url**: Request a cloud storage upload URL for media
- **get_mission_status**: Check the progress of an active flight mission
- **list_devices**: List all drones and docks bound to your account
- **list_media_files**: List photos and videos captured by a drone
- **list_waylines**: List available flight wayline files


## Installation & Usage

To install and use the **DJI Developer** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dji-developer](https://vinkius.com/mcp/dji-developer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

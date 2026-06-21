# Google Home MCP Server

Control Google Nest devices — thermostats, cameras, and doorbells via Smart Device Management (SDM) API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/google-home)

## Overview
**Category:** the-unthinkable
**Tools Count:** 12

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


## Available Tools
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


## Installation & Usage

To install and use the **Google Home** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-home](https://vinkius.com/mcp/google-home)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

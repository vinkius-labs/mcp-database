# Alexa Smart Home MCP Server

Control Alexa-connected smart home devices — lights, thermostats, speakers, and sensors via Alexa Smart Properties API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/alexa-smart-home)

## Overview
**Category:** industry-titans
**Tools Count:** 16

## Description
Connect to **Alexa Smart Home** devices via the Alexa Smart Properties API and control your smart home from any AI agent. Manage lights, thermostats, speakers, and sensors across your connected endpoints.

### What you can do

- **List Devices** — See all your Alexa-connected smart home devices with names, manufacturers, and features
- **Device Details** — Get full device information including serial numbers, connections, and capabilities
- **Power Control** — Turn devices on and off (lights, plugs, switches)
- **Light Control** — Get and set brightness levels, adjust brightness relatively
- **Speaker Control** — Get and set speaker volume on Alexa devices
- **Thermostat Monitoring** — View thermostat state including mode and target temperatures
- **Temperature Sensors** — Read current temperature from connected sensors
- **Rename Devices** — Update friendly names for your devices
- **Room Management** — Assign devices to specific rooms/units
- **Device Management** — Deregister or forget devices from your Alexa account

### How it works

1. Subscribe to this server
2. Obtain OAuth 2.0 access token from Login with Amazon (LWA)
3. Start controlling your Alexa devices from Claude, Cursor, or any MCP-compatible client

Your AI becomes a smart home assistant, helping you manage lighting, climate, and audio across your connected home.

### Who is this for?

- **Smart Home Owners** — control lights, thermostats, and speakers from AI assistants
- **Property Managers** — manage devices across multiple properties and rooms
- **Hospitality Operators** — monitor and adjust climate and lighting in hotel rooms
- **Energy-Conscious Users** — optimize device power states for energy savings
- **Home Automation Enthusiasts** — integrate Alexa devices into broader automation workflows


## Available Tools
- **adjust_brightness**: Positive values increase brightness, negative values decrease it.

Adjust the brightness of an Alexa-connected light relatively
- **deregister_alexa_device**: This removes the device from your account but does not reset the device itself.

Deregister an Alexa-connected device from your account
- **forget_alexa_device**: The device will need to be re-discovered and set up again to be used with Alexa.

Remove (forget) an Alexa-connected device from Alexa
- **get_brightness_state**: Use endpoint ID from list_alexa_devices.

Get the current brightness level of an Alexa-connected light
- **get_alexa_device**: Use endpoint ID from list_alexa_devices.

Get detailed information for a specific Alexa-connected device
- **get_power_state**: Use endpoint ID from list_alexa_devices.

Get the current power state of an Alexa-connected device
- **get_speaker_state**: Use endpoint ID from list_alexa_devices.

Get the current speaker volume state of an Alexa device
- **get_temperature_sensor**: Use endpoint ID from list_alexa_devices.

Get the current temperature reading from an Alexa-connected sensor
- **get_thermostat_state**: Use endpoint ID from list_alexa_devices.

Get the current state of an Alexa-connected thermostat
- **list_alexa_devices**: Shows device names, manufacturers, models, features, and display categories.

USE WHEN:
- User wants to see all their Alexa-connected smart devices
- User needs to find endpoint IDs for other commands
- User is exploring their smart home setup
- User asks "what Alexa devices do I have"

PARAMETERS:
- max_results (OPTIONAL): Number of results (1-50, default: 10)
- next_token (OPTIONAL): Pagination token from previous response

EXAMPLES:
- "List all my Alexa devices" → call with no params
- "Show my smart home devices" → call with no params
- "What Alexa devices are connected?" → call with no params

List all Alexa-connected smart home devices and endpoints
- **set_brightness**: Use endpoint ID from list_alexa_devices.

Set the brightness level of an Alexa-connected light
- **set_volume**: Use endpoint ID from list_alexa_devices.

Set the speaker volume of an Alexa device
- **turn_off_alexa_device**: Works for lights, switches, plugs, and other power-controllable devices.

Turn off an Alexa-connected device
- **turn_on_alexa_device**: Works for lights, switches, plugs, and other power-controllable devices.

Turn on an Alexa-connected device
- **update_alexa_device_name**: Use endpoint ID from list_alexa_devices.

Update the friendly name of an Alexa-connected device
- **update_device_room**: Use endpoint ID from list_alexa_devices and unit ID from your Alexa Smart Properties account.

Update the room/unit assignment for an Alexa-connected device


## Installation & Usage

To install and use the **Alexa Smart Home** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alexa-smart-home](https://vinkius.com/mcp/alexa-smart-home)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

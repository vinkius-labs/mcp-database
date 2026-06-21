# Alexa Smart Home MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/alexa-smart-home)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Control Alexa-connected smart home devices — lights, thermostats, speakers, and sensors via Alexa Smart Properties API.

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


## Available Tools (16)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Alexa Smart Home** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Alexa-connected smart home devices."

**🤖 AI Agent:**
> I found 6 Alexa-connected devices in your account: 1) Living Room Lamp (Philips Hue) — brightness controllable, 2) Bedroom Thermostat (Ecobee) — temperature monitoring, 3) Kitchen Echo (Amazon) — speaker volume controllable, 4) Front Porch Light (LIFX) — on/off and brightness, 5) Hallway Temperature Sensor, 6) Office Smart Plug. Would you like to control any of these devices?

---

**👤 You:**
> "Turn on the living room lamp and set brightness to 70%."

**🤖 AI Agent:**
> Turning on the Living Room Lamp... Done! The lamp is now ON. Setting brightness to 70%... Done! Your Living Room Lamp is now at 70% brightness.

---

**👤 You:**
> "What's the current temperature in the bedroom and what mode is the thermostat in?"

**🤖 AI Agent:**
> Checking bedroom thermostat... Current temperature reading: 21.5°C (70.7°F). The thermostat is currently in HEAT mode with a target temperature of 22°C (71.6°F). The HVAC system is actively heating to reach the target.


## ❓ FAQ

**Q: What Alexa-connected devices are supported by this API?**
The Alexa Smart Properties API supports: smart lights (on/off, brightness, color), smart plugs and switches, thermostats (mode and temperature monitoring), temperature sensors, Echo devices and speakers (volume control), security sensors, and other Alexa-connected endpoints. Each device exposes specific features (power, brightness, speaker, thermostat, etc.) that can be queried and controlled.

**Q: How do I get an OAuth 2.0 access token for the Alexa API?**
Visit the [**Alexa Developer Console**](https://developer.amazon.com/alexa/console/ask) and create a Smart Home Skill. Set up Login with Amazon (LWA) credentials in your Amazon Developer account. Complete the OAuth 2.0 authorization flow to obtain an access token. The token must be refreshed periodically as it expires after a set duration.

**Q: Can I control devices in different rooms or properties?**
Yes! The API returns all devices across all properties and rooms in your Alexa Smart Properties account. Use `list_alexa_devices` to see all devices with their room assignments, then use each device's unique endpoint ID to control them individually. You can also reassign devices to different rooms using the `update_device_room` action.

**Q: What's the difference between deregister and forget a device?**
`Deregister` removes the device from your Alexa Smart Properties account but keeps it available for re-discovery. The device itself remains configured. `Forget` completely removes the device from Alexa — it will need to be re-discovered and set up again as if it were a new device. Use deregister for temporary removal and forget for permanent removal.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/alexa-smart-home](https://vinkius.com/mcp/alexa-smart-home)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Alexa Smart Home** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `alexa-smart-home` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Alexa Smart Home** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "alexa-smart-home": {
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

# ESPHome MCP Server

Control and monitor your ESPHome-powered IoT devices directly from any AI agent via the Web Server API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/esphome)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

## Description
Connect your **ESPHome** microcontrollers to any AI agent and take full control of your smart home or industrial IoT setup through natural conversation.

### What you can do

- **Real-time Monitoring** — Fetch the current state and values of any sensor, switch, or binary sensor using the `get_entity_state` tool.
- **Lighting Control** — Manage lights with precision using `light_action`, including brightness and RGB color adjustments.
- **Appliance Management** — Toggle switches, control fans with `fan_action`, and adjust covers (blinds/garage doors) with `cover_action`.
- **Interactive Components** — Press buttons via `button_press`, set numeric values with `number_set`, and choose options from dropdowns with `select_option`.
- **Security & Safety** — Arm or disarm alarm panels using `alarm_action` directly from your chat interface.

### How it works

1. Enable the `web_server` component in your ESPHome YAML configuration.
2. Subscribe to this server.
3. Enter your device's local URL and optional password.
4. Start interacting with your hardware from Claude, Cursor, or any MCP client.

### Who is this for?

- **Home Automation Enthusiasts** — control your local environment without complex dashboards.
- **IoT Developers** — test and debug ESP32/ESP8266 entity behaviors using natural language.
- **Hardware Engineers** — monitor sensor metrics and trigger actions during prototyping phases.


## Available Tools
- **alarm_action**: Perform an action on an alarm control panel
- **button_press**: Press a button entity
- **cover_action**: g., blinds, garage door), optionally setting position and tilt.

Perform an action on a cover entity
- **fan_action**: Perform an action on a fan entity
- **get_entity_state**: g., sensor, switch) using the Web Server REST API.

Get the state of an ESPHome entity
- **get_metrics**: Get Prometheus metrics from the ESPHome device
- **light_action**: Perform an action on a light entity
- **number_set**: Set a value for a number entity
- **select_option**: Set an option for a select entity
- **switch_action**: Perform an action on a switch entity


## Installation & Usage

To install and use the **ESPHome** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/esphome](https://vinkius.com/mcp/esphome)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

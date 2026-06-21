# Home Assistant MCP Server

Control smart home devices and automations via Home Assistant REST API — lights, climate, media, covers, sensors, and more.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/home-assistant)

## Overview
**Category:** superpower
**Tools Count:** 15

## Description
Connect to your **Home Assistant** instance (local or Nabu Casa cloud) and control your entire smart home from any AI agent. Manage lights, climate, media players, covers, switches, and trigger automations via the Home Assistant REST API.

### What you can do

- **Entity Discovery** — List all entities and their current states across all integrations
- **Device Control** — Turn lights on/off, adjust brightness, set thermostat temperatures, open/close covers
- **Service Calls** — Call any Home Assistant service (light, switch, climate, cover, media_player, automation, script)
- **State Monitoring** — Get real-time state of any entity including sensors, binary sensors, and device trackers
- **History & Logbook** — Query historical state changes and logbook entries for analysis
- **Calendar Management** — List and query calendar events from Home Assistant calendars
- **Event Automation** — Fire custom events to trigger Home Assistant automations
- **Template Rendering** — Render Jinja2 templates for advanced state access
- **Configuration** — View system configuration, loaded components, and validate configuration
- **Local or Cloud** — Works with local instances (http://IP:8123) or Nabu Casa cloud (https://INSTANCE.ui.nabu.casa)

### How it works

1. Subscribe to this server
2. Enter your Home Assistant URL and Long-Lived Access Token
3. Start controlling your smart home from Claude, Cursor, or any MCP-compatible client

Your AI becomes a smart home assistant, helping you manage lighting, climate, media, and automations across your entire home.

### Who is this for?

- **Smart Home Enthusiasts** — control all Home Assistant-connected devices from AI assistants
- **Home Automation Builders** — integrate HA into broader automation workflows and scripts
- **Property Managers** — monitor and control devices across multiple properties
- **Energy-Conscious Users** — optimize device states for energy savings via automations
- **Security-Conscious Users** — monitor sensors, cameras, and alarm states remotely


## Available Tools
- **get_api_status**: Use this as a connectivity test before making other API calls.

Check if the Home Assistant API is running
- **get_calendar_events**: Get events from a Home Assistant calendar
- **list_ha_calendars**: List all calendars configured in Home Assistant
- **call_ha_service**: This is the primary way to control devices in Home Assistant.

COMMON SERVICE CALLS:
- light.turn_on: entity_id, brightness (0-255), color_temp, rgb_color
- light.turn_off: entity_id
- switch.turn_on: entity_id
- switch.turn_off: entity_id
- climate.set_temperature: entity_id, temperature
- climate.set_hvac_mode: entity_id, hvac_mode (heat, cool, auto, off)
- cover.open_cover: entity_id
- cover.close_cover: entity_id
- media_player.turn_on: entity_id
- media_player.turn_off: entity_id
- media_player.media_play: entity_id
- automation.trigger: entity_id
- script.turn_on: entity_id

DOMAINS: light, switch, climate, cover, fan, lock, media_player, automation, script, scene, input_boolean, input_number, notify

PARAMETERS:
- domain (REQUIRED): Domain name (e.g. light, switch, climate)
- service (REQUIRED): Service name (e.g. turn_on, turn_off, set_temperature)
- service_data (OPTIONAL): JSON object with service parameters including entity_id

EXAMPLES:
- "Turn on living room light" → domain="light", service="turn_on", service_data={"entity_id":"light.living_room"}
- "Set bedroom temperature to 20" → domain="climate", service="set_temperature", service_data={"entity_id":"climate.bedroom","temperature":20}

Call a Home Assistant service on a domain
- **check_ha_configuration**: Check Home Assistant configuration validity
- **list_ha_components**: List all loaded components/integrations in Home Assistant
- **get_ha_config**: Get the Home Assistant configuration details
- **list_ha_events**: Useful for understanding what events Home Assistant is tracking.

List all event types currently registered in Home Assistant
- **fire_ha_event**: The event type must match automation triggers configured in Home Assistant.

Fire a custom event in Home Assistant
- **get_entity_state**: Use entity IDs from list_entity_states (e.g., light.living_room, climate.bedroom, sensor.temperature).

Get the current state of a specific entity
- **get_entity_history**: Useful for analyzing trends and past behavior.

Get historical state data for an entity
- **get_logbook_entries**: Can be filtered by entity and time range.

Get Home Assistant logbook entries
- **render_ha_template**: Useful for accessing HA template functions and state from the API.

Render a Jinja2 template in Home Assistant
- **list_available_services**: g., light: turn_on, turn_off, toggle; climate: set_temperature, set_hvac_mode). Essential for discovering what actions can be performed.

List all available services across all domains
- **list_entity_states**: Each entity includes entity_id, state, last_changed timestamp, and attributes. Essential for discovering available devices.

List all entity states in Home Assistant


## Installation & Usage

To install and use the **Home Assistant** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/home-assistant](https://vinkius.com/mcp/home-assistant)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

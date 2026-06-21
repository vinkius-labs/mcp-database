# Zapier Smart Home MCP Server

Control smart home devices via natural language through Zapier NLA API — access 5000+ app integrations for home automation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/zapier-smart-home)

## Overview
**Category:** friends-mcp
**Tools Count:** 12

## Description
Connect to **Zapier Natural Language Actions (NLA) API** and control your entire smart home through natural language commands across 5000+ app integrations. Turn on lights, adjust thermostats, lock doors, trigger cameras, and automate any connected device — all through simple English commands.

### What you can do

- **Natural Language Control** — Send commands like "turn on the kitchen lights" or "set thermostat to 72°F" in plain English
- **Action Discovery** — Search and discover available smart home actions across 5000+ app integrations
- **Exposed Actions** — List and manage all smart home actions you've exposed in your Zapier account
- **AI-Enabled Zaps** — List, preview, and trigger AI-enabled automation workflows (zaps)
- **Lighting Control** — Find and execute lighting actions (turn on/off, dim, color) across supported integrations
- **Climate Control** — Discover and execute thermostat and climate actions
- **Security Management** — Find and execute security, camera, and alarm actions
- **Zap Preview** — Preview automation workflows from natural language descriptions before creating them
- **Configuration** — Get setup links to expose new smart home actions for AI control

### How it works

1. Subscribe to this server
2. Enter your Zapier NLA API key (get it at https://nla.zapier.com/)
3. Start controlling your smart home with natural language from Claude, Cursor, or any MCP-compatible client

Your AI becomes a universal smart home assistant, translating your natural language commands into actions across Philips Hue, Nest, Ring, Ecobee, SmartThings, and thousands of other integrations.

### Who is this for?

- **Smart Home Owners** — control any connected device with simple natural language commands
- **Home Automation Enthusiasts** — discover and execute actions across 5000+ app integrations
- **Property Managers** — manage smart home devices across multiple properties through a unified interface
- **Accessibility Users** — control smart home devices with natural language instead of complex apps
- **Integration Builders** — build automations and workflows through Zapier's NLA API


## Available Tools
- **list_climate_actions**: List available climate/thermostat control actions
- **get_zapier_config_link**: Use this link to expose new actions for AI control.

Get the configuration link for setting up more smart home actions
- **execute_zapier_action**: Primary method for controlling devices through Zapier NLA.

Execute a specific exposed action by ID with natural language instructions
- **list_lighting_actions**: List available lighting control actions (turn on/off, dim, color)
- **list_ai_zaps**: List all AI-enabled zaps in your Zapier account
- **list_exposed_actions**: List all exposed smart home actions in your Zapier account
- **send_natural_language_command**: Zapier interprets the command and routes it to the best matching action automatically.

Send any smart home command using natural language through Zapier
- **preview_zapier_zap**: Preview a Zap from a natural language description
- **search_zapier_actions**: Returns matching actions that can be executed via the NLA API.

Search for available actions across 5000+ apps using natural language
- **list_security_actions**: List available security, camera, and alarm control actions
- **list_smarthome_actions**: Returns up to 50 matching actions that can be used for home automation.

List available smart home actions across 5000+ app integrations
- **trigger_ai_zap**: Trigger/execute a specific AI-enabled zap


## Installation & Usage

To install and use the **Zapier Smart Home** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zapier-smart-home](https://vinkius.com/mcp/zapier-smart-home)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

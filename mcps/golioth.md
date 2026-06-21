# Golioth MCP Server

Manage IoT devices and projects via Golioth — list projects, register hardware, and control LightDB state directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/golioth)

## Overview
**Category:** developer-tools
**Tools Count:** 7

## Description
Connect your **Golioth** IoT cloud to any AI agent and take full control of your connected hardware fleet through natural conversation.

### What you can do

- **Project Management** — List all available Golioth projects and create new ones to organize your IoT infrastructure.
- **Device Fleet Control** — List registered devices within any project, register new hardware, or remove decommissioned units.
- **LightDB State Interaction** — Read and write real-time data to your devices using LightDB State. Query specific paths (like sensors) or update configurations (like LEDs or thresholds) instantly.
- **Hardware Orchestration** — Monitor device connectivity and manage credentials without leaving your development environment.

### How it works

1. Subscribe to this server
2. Enter your Golioth API Key
3. Start managing your IoT fleet from Claude, Cursor, or any MCP-compatible client

No more switching between the Golioth Console and your code. Your AI acts as a remote terminal for your entire hardware ecosystem.

### Who is this for?

- **IoT Engineers** — instantly check sensor values and device statuses while debugging firmware.
- **Product Managers** — monitor fleet deployment progress and project growth through simple queries.
- **Embedded Developers** — register and test new devices directly from the IDE without manual API calls.


## Available Tools
- **create_project**: Create a new Golioth project
- **get_lightdb_state**: Get LightDB State for a device
- **list_devices**: List devices in a Golioth project
- **list_projects**: List Golioth projects
- **register_device**: Register a new device in a Golioth project
- **remove_device**: Remove a device from a Golioth project
- **set_lightdb_state**: Set LightDB State for a device


## Installation & Usage

To install and use the **Golioth** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/golioth](https://vinkius.com/mcp/golioth)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

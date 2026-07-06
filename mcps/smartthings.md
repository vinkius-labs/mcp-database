# SmartThings MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/smartthings)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Control and monitor your smart home ecosystem — manage devices, check real-time statuses, and trigger scenes directly from your AI agent.

## Description
Connect your **SmartThings** ecosystem to any AI agent and take full control of your smart home or office through natural conversation.

### What you can do

- **Device Management** — List all connected devices and fetch detailed metadata for specific hardware components.
- **Real-time Monitoring** — Query the current state and attribute values (temperature, switch status, battery levels) of any device.
- **Command Execution** — Send direct commands to devices, such as toggling switches, adjusting levels, or changing modes.
- **Spatial Organization** — List locations and rooms, or create new room subdivisions to better organize your IoT environment.
- **Scene Automation** — List and execute pre-configured scenes to trigger multiple device actions simultaneously.
- **App Insights** — Monitor installed SmartApps and manage event subscriptions for advanced automation workflows.

### How it works

1. Subscribe to this server
2. Enter your SmartThings Personal Access Token (PAT)
3. Start managing your IoT environment from Claude, Cursor, or any MCP-compatible client

No more jumping between mobile apps to check if you left the lights on or to trigger a 'Movie Night' scene. Your AI acts as your central smart home controller.

### Who is this for?

- **Home Automation Enthusiasts** — centralize control of diverse IoT brands under a single conversational interface.
- **Developers** — test device capabilities and monitor status attributes directly from your coding environment.
- **Smart Office Managers** — automate and monitor office environments, rooms, and energy usage through simple queries.


## Available Tools (13)
- **create_room**: Create a new room in a SmartThings location
- **execute_device_command**: g., switch on/off, set level).

Send commands to a SmartThings device
- **get_device_status**: Get the current state of all device components
- **list_devices**: List all SmartThings devices
- **execute_scene**: Execute a SmartThings scene
- **get_device**: Get details for a specific SmartThings device
- **get_location**: Get details for a specific SmartThings location
- **list_installed_apps**: List all installed instances of SmartApps
- **list_locations**: g., Home) accessible by the token.

List all SmartThings locations
- **list_rooms**: List all rooms in a SmartThings location
- **list_scenes**: List all SmartThings scenes
- **list_subscriptions**: Manage event subscriptions for SmartApps
- **list_apps**: List all SmartApps


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SmartThings** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my connected SmartThings devices."

**🤖 AI Agent:**
> I've retrieved your devices. You have 3 active devices: 'Living Room Light' (ID: d23...), 'Smart Thermostat' (ID: a45...), and 'Front Door Lock' (ID: e89...). Which one would you like to inspect?

---

**👤 You:**
> "Turn on the Living Room Light (ID: d23-abc)."

**🤖 AI Agent:**
> Executing command... I've successfully sent the 'on' command to the 'Living Room Light' component. The device should now be active.

---

**👤 You:**
> "What is the current temperature on my Smart Thermostat (ID: a45-xyz)?"

**🤖 AI Agent:**
> Checking status... The 'Smart Thermostat' is currently reporting a temperature of 22°C (71.6°F) with the operating mode set to 'Auto'.


## ❓ FAQ

**Q: Can I check if my lights are on and see the current brightness level?**
Yes. Use the `get_device_status` tool with the specific Device ID. It will return the current state of all components, including switch status and level attributes.

**Q: How do I trigger a 'Movie Night' scene that I already created in the SmartThings app?**
First, use `list_scenes` to find the ID of your 'Movie Night' scene. Then, use the `execute_scene` tool with that ID to trigger all associated actions at once.

**Q: Is it possible to organize my devices into a new room using this server?**
Yes. You can use the `create_room` tool by providing the target Location ID and the desired name for the new room subdivision.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/smartthings](https://vinkius.com/mcp/smartthings)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SmartThings** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `smartthings` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SmartThings** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "smartthings": {
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

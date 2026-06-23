# ESPHome MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/esphome)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Control and monitor your ESPHome-powered IoT devices directly from any AI agent via the Web Server API.

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


## Available Tools (10)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ESPHome** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current reading of the 'living_room_temperature' sensor?"

**🤖 AI Agent:**
> Checking the sensor... The current state of 'living_room_temperature' is 22.5°C.

---

**👤 You:**
> "Turn on the kitchen light and set it to a warm orange color."

**🤖 AI Agent:**
> I've sent the command to the kitchen light. It is now on with the RGB values set to (255, 165, 0).

---

**👤 You:**
> "Close the garage door cover."

**🤖 AI Agent:**
> Executing the close action on the garage door cover. The command has been sent successfully.


## ❓ FAQ

**Q: Can I control my lights and set specific colors using this server?**
Yes! Use the `light_action` tool. You can specify the entity name, the action (turn_on), and optional parameters like brightness (0-255) and RGB values (r, g, b) to get the perfect ambiance.

**Q: How do I check the current temperature or humidity from my sensors?**
Simply use the `get_entity_state` tool. Provide the domain (e.g., 'sensor') and the entity ID. The agent will return the current value and state of that specific hardware component.

**Q: Is it possible to trigger a physical button or restart a device?**
Yes. If you have a button entity configured in ESPHome (like a restart button), you can use the `button_press` tool with the entity name to trigger that action remotely.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/esphome](https://vinkius.com/mcp/esphome)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ESPHome** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `esphome` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ESPHome** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "esphome": {
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

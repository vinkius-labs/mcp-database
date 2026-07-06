# Golioth MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/golioth)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage IoT devices and projects via Golioth — list projects, register hardware, and control LightDB state directly from your AI agent.

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


## Available Tools (7)
- **get_lightdb_state**: Get LightDB State for a device
- **list_devices**: List devices in a Golioth project
- **list_projects**: List Golioth projects
- **register_device**: Register a new device in a Golioth project
- **remove_device**: Remove a device from a Golioth project
- **set_lightdb_state**: Set LightDB State for a device
- **create_project**: Create a new Golioth project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Golioth** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Golioth projects."

**🤖 AI Agent:**
> I've retrieved your projects. You have access to: 'Smart-Home-Hub' (ID: proj_123) and 'Industrial-Sensors' (ID: proj_456). Which one would you like to explore?

---

**👤 You:**
> "Show me the devices registered in project proj_123."

**🤖 AI Agent:**
> In project 'Smart-Home-Hub', I found 3 devices: 'Living-Room-Temp', 'Kitchen-Light', and 'Main-Gateway'. All are currently showing as active.

---

**👤 You:**
> "Set the LightDB state for device 'Kitchen-Light' in project proj_123 at path 'power' to {"on": true}."

**🤖 AI Agent:**
> Successfully updated the LightDB state. The 'power' path for 'Kitchen-Light' is now set to {"on": true}. The device should receive this update immediately.


## ❓ FAQ

**Q: How can I read the current sensor data from a specific device?**
Use the `get_lightdb_state` tool by providing the Project ID, Device ID, and the specific path (e.g., 'sensor/temp'). The agent will return the current value stored in Golioth's LightDB.

**Q: Can I register a new device to my project using the AI?**
Yes! Use the `register_device` action. You just need to provide the Project ID and a name for the new device. The agent will handle the registration and return the device details.

**Q: Is it possible to update device configurations remotely?**
Absolutely. Use the `set_lightdb_state` tool to write JSON data to any path on the device. This is perfect for updating thresholds, toggling states, or sending commands to your hardware.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/golioth](https://vinkius.com/mcp/golioth)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Golioth** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `golioth` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Golioth** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "golioth": {
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

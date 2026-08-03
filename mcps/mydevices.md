# myDevices MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mydevices)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

IoT device management — monitor telemetry and control assets via myDevices Cayenne.

## Description
Connect your **myDevices Cayenne** account to empower your AI agents with IoT capabilities. This server allows for real-time monitoring and control of connected sensors and actuators.

### What you can do

- **Device Visibility** — List and inspect all connected IoT devices and their metadata
- **Telemetry Monitoring** — Access real-time sensor data and historical telemetry records
- **Remote Control** — Send commands to actuators and control hardware programmatically
- **Alert Management** — Monitor and track IoT system alerts and notifications

### How it works

1. Subscribe to this server
2. Enter your **Client ID**, **Client Secret**, **Username**, and **Password**
3. Start managing your IoT fleet directly from Claude, Cursor, or any MCP client


## Available Tools (8)
- **get_device**: Get device details
- **get_sensor_data**: Get current sensor value
- **get_sensor_history**: Get historical sensor data
- **list_alerts**: List IoT alerts
- **list_applications**: List all applications
- **list_devices**: List all IoT devices
- **list_sensors**: List sensors for a device
- **send_command**: Send command to device


## 💬 Prompt Examples

Here are some examples of how you can interact with the **myDevices** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my connected IoT devices."

**🤖 AI Agent:**
> Retrieving devices... I've found 5 active devices, including your Raspberry Pi and ESP32 nodes.

---

**👤 You:**
> "What is the current temperature reading from 'Sensor #1'?"

**🤖 AI Agent:**
> Checking telemetry... The current temperature for Sensor #1 is 24.5°C.


## ❓ FAQ

**Q: How do I get my API credentials?**
Register a developer account at mydevices.com and create a new application in the developer portal to get your Client ID and Secret.

**Q: Does this work with Cayenne LPP?**
Yes, as long as the data is correctly indexed in the Cayenne dashboard, this server can retrieve it via the REST API.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mydevices](https://vinkius.com/mcp/mydevices)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **myDevices** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mydevices` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **myDevices** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mydevices": {
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

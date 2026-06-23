# Tuya MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tuya)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Control and monitor your Tuya IoT ecosystem — query device status and send real-time commands to smart hardware via AI.

## Description
Connect your **Tuya IoT** account to any AI agent and manage your smart home or industrial hardware through natural conversation.

### What you can do

- **Device Inspection** — Retrieve detailed metadata for any connected device, including its online status, category, and local key for advanced integrations.
- **Real-time Control** — Send precise commands to your hardware using standard instruction sets (e.g., toggling switches, adjusting brightness, or setting modes).
- **Status Monitoring** — Instantly check if your devices are reachable and functioning correctly within your cloud project.

### How it works

1. Subscribe to this server
2. Enter your Tuya Client ID, Secret, and Endpoint
3. Start controlling your smart environment from Claude, Cursor, or any MCP-compatible client

No more jumping between mobile apps to check if a sensor is online or to toggle a smart plug. Your AI acts as a centralized IoT dashboard.

### Who is this for?

- **Smart Home Enthusiasts** — manage complex automation setups and check device health directly from your workspace.
- **IoT Developers** — quickly inspect device categories and local keys while building or debugging integrations.
- **Facility Managers** — monitor and control distributed hardware across different locations using simple text commands.


## Available Tools (2)
- **get_device**: Query Tuya device details
- **send_commands**: g., switch_led: true).

Send control commands to a Tuya device


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tuya** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check the status and details of device ID 'bf78234567890abcdef'."

**🤖 AI Agent:**
> I've queried the device. It is currently Online. It's a 'Smart Plug' (Category: cz) with the local key 'a1b2c3d4...'. Would you like to send any commands to it?

---

**👤 You:**
> "Turn on the LED for device 'eb4567890123456789'."

**🤖 AI Agent:**
> Command sent successfully. I've instructed device 'eb4567890123456789' to set 'switch_led' to true. The device has confirmed receipt of the command.

---

**👤 You:**
> "Is my smart heater (ID: 0123456789) reachable right now?"

**🤖 AI Agent:**
> Checking connectivity... Yes, the smart heater is currently reporting as Online in the Tuya Cloud. Its last heartbeat was received successfully.


## ❓ FAQ

**Q: How can I check if a specific smart device is currently online?**
Use the `get_device` tool with the target Device ID. The agent will return the current connectivity status along with other technical metadata from the Tuya Cloud.

**Q: Can I send multiple commands to a device at once?**
Yes! The `send_commands` tool accepts an array of command objects. You can trigger multiple actions, such as turning on a light and setting its color, in a single request.

**Q: What kind of technical details does the agent provide for my hardware?**
By running `get_device`, the agent retrieves the device category, its unique local key, the product name, and its current operational status, allowing for deep technical auditing.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tuya](https://vinkius.com/mcp/tuya)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tuya** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tuya` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tuya** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tuya": {
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

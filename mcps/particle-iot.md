# Particle IoT MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/particle-iot)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access Particle IoT devices via API — read sensor variables, control device functions, manage devices, and publish events from any AI agent.

## Description
Connect your **Particle IoT API** to any AI agent and take full control of your IoT device fleet, sensor monitoring, remote actuator control, and event management through natural conversation.

### What you can do

- **Device Management** — List all connected devices, check online status, rename devices, and manage ownership
- **Sensor Monitoring** — Read real-time sensor data from cloud variables (temperature, humidity, soil moisture, etc.)
- **Remote Control** — Execute cloud functions to control actuators, trigger calibrations, and change device modes
- **Event Publishing** — Broadcast custom events to the cloud for logging, alerting, and webhook integration
- **Health Monitoring** — Ping devices to verify connectivity and troubleshoot communication issues
- **Fleet Overview** — Get comprehensive views of your entire IoT deployment and device status

### How it works

1. Subscribe to this server
2. Enter your Particle Access Token (from Particle Console or CLI)
3. Start controlling your IoT devices from Claude, Cursor, or any MCP-compatible client

No more manual device checking or complex API calls. Your AI acts as a dedicated IoT fleet manager and sensor analyst.

### Who is this for?

- **Agriculture Tech** — monitor soil moisture, control irrigation pumps, and receive crop alerts remotely
- **Smart Home** — read environmental sensors, control actuators, and automate home systems
- **Industrial IoT** — manage sensor networks, monitor equipment status, and trigger maintenance functions
- **Developers** — prototype IoT applications, test device functions, and integrate with external systems


## Available Tools (8)
- **call_function**: Functions are defined in the device firmware and can control actuators (turn on pump, open valve), trigger calibrations, change device modes, or perform system tasks. Accepts a single string argument (max 63 characters) to pass to the function. Returns the function execution result code. Essential for remote device control, automation, and actuator management. AI agents should use this when users ask "turn on the water pump on device X", "trigger calibration on sensor Y", or need to remotely control any function exposed by a device.

Execute a cloud function on a specific Particle IoT device
- **get_device_info**: Essential for understanding device capabilities before interacting with it. AI agents should reference this when users ask "what variables does device X expose", "what functions can I call on device Y", or need to understand the specific interface of a device.

Get detailed information about a specific Particle IoT device
- **get_devices**: Returns device IDs, names, online status, firmware versions, and last connection times. Essential for device inventory management, monitoring connection health, and selecting specific devices for interaction. AI agents should use this when users ask "show me all my devices", "list connected sensors", or need to identify available devices before reading variables or calling functions.

List all Particle IoT devices connected to your account
- **ping_device**: Returns current online/offline status and last heard time. Essential for connectivity diagnostics, health monitoring, and verifying device availability before attempting to read variables or call functions. AI agents should reference this when users ask "is device X online", "check connectivity for sensor Y", or need to troubleshoot device communication issues.

Check if a specific Particle IoT device is online and responsive
- **publish_event**: Events are broadcast to all subscribed listeners and can be used for inter-device communication, logging, alerting, or triggering external workflows via webhooks. Requires an event name and optional data string (max 255 bytes for data). Essential for sending alerts, logging custom data, and integrating with external systems like IFTTT or custom dashboards. AI agents should use this when users ask "send a low moisture alert", "publish a system status event", or need to broadcast data from the cloud to devices or webhooks.

Publish a custom event to the Particle Cloud
- **read_variable**: Variables are defined in the device firmware and can represent sensor readings (temperature, humidity, soil moisture), system status, or configuration values. Returns the variable name, data type, and current value. Essential for real-time sensor monitoring, data collection, and system state verification. AI agents should use this when users ask "what is the temperature from sensor X", "read soil moisture from device Y", or need to get the current value of any sensor or status variable.

Read the current value of a cloud variable from a specific device
- **rename_device**: This name appears in the console and API responses, making it easier to identify devices. Essential for device organization, fleet management, and improving readability of device lists. AI agents should use this when users ask "rename device X to Greenhouse Sensor 1", "change the name of device Y to Pump Controller", or need to update device naming for better organization.

Rename a specific Particle IoT device
- **unclaim_device**: This action is irreversible for the current account and should be used when transferring device ownership or decommissioning devices. Essential for device lifecycle management, transferring devices, and account cleanup. AI agents should use this when users ask "remove device X from my account", "unclaim sensor Y so I can sell it", or need to manage device ownership. WARNING: This requires confirmation as it removes access to the device.

Remove a Particle IoT device from your account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Particle IoT** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all my connected Particle devices and their online status."

**🤖 AI Agent:**
> Fetching device list... Found 5 devices. Device 1: 'Greenhouse Sensor' (ID: a1b2c3) - Online, Firmware: 5.8.0, Last seen: 1 min ago. Device 2: 'Irrigation Pump' (ID: d4e5f6) - Online, Firmware: 5.8.0, Last seen: 2 mins ago. Device 3: 'Soil Moisture Node' (ID: g7h8i9) - Offline, Last seen: 3 hours ago. Device 4: 'Weather Station' (ID: j0k1l2) - Online, Firmware: 5.7.2, Last seen: 30 secs ago. Device 5: 'Tank Level Sensor' (ID: m3n4o5) - Online, Firmware: 5.8.0, Last seen: 45 secs ago. Total: 4 online, 1 offline. Would you like to troubleshoot the offline device?

---

**👤 You:**
> "Read the current soil moisture from my greenhouse sensor."

**🤖 AI Agent:**
> Reading variable 'soilMoisture' from device 'Greenhouse Sensor'... Current value: 68%. Status: Adequate moisture for most crops. Historical trend: Stable over the last 6 hours. Recommendation: No irrigation needed at this time. Next check recommended in 2 hours. Would you like to read the temperature as well?

---

**👤 You:**
> "Turn on the irrigation pump for 15 minutes."

**🤖 AI Agent:**
> Calling function 'pumpOn' on device 'Irrigation Pump' with argument '900' (15 minutes)... Result: Success (return code 1). Pump activated successfully. Estimated water delivery: 250 liters based on flow rate. Status: Pump running, will auto-shutoff in 15 minutes. Would you like me to monitor soil moisture during the irrigation cycle?


## ❓ FAQ

**Q: Can my AI read sensor data from my Particle devices?**
Yes! Use the `read_variable` tool with your device ID and the variable name (e.g., temperature, humidity, soilMoisture). Your device must expose this variable in its firmware using `Particle.variable()`. The AI will return the current sensor value in real-time. You can find available variables using `get_device_info`.

**Q: How do I remotely turn on a pump or actuator connected to a Particle device?**
Use the `call_function` tool with your device ID and the function name (e.g., pumpOn, valveOpen). The function must be exposed in your device firmware using `Particle.function()`. You can pass an optional argument (like duration or intensity) to control the actuator behavior. Check available functions with `get_device_info`.

**Q: Can I check if my IoT device is online and responding?**
Yes! Use the `ping_device` tool to instantly check the online status of any Particle device. You can also use `get_devices` to see the online status of all your devices at once. If a device shows as offline, it may be powered off, disconnected from Wi-Fi, or experiencing firmware issues.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/particle-iot](https://vinkius.com/mcp/particle-iot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Particle IoT** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `particle-iot` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Particle IoT** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "particle-iot": {
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

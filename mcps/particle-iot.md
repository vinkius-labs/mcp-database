# Particle IoT MCP Server

Access Particle IoT devices via API — read sensor variables, control device functions, manage devices, and publish events from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/particle-iot)

## Overview
**Category:** the-unthinkable
**Tools Count:** 8

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


## Available Tools
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


## Installation & Usage

To install and use the **Particle IoT** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/particle-iot](https://vinkius.com/mcp/particle-iot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

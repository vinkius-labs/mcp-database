# ThingsBoard MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thingsboard)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/thingsboard-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/thingsboard-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Manage your IoT ecosystem via ThingsBoard — monitor telemetry, control devices with RPC, and track alarms directly from your AI agent.

## Description
Connect your **ThingsBoard** instance to any AI agent to orchestrate your IoT infrastructure through natural language. This server provides deep integration with the ThingsBoard REST API for real-time device management and data analysis.

### What you can do

- **Telemetry & Attributes** — Save and retrieve time-series data or manage entity attributes (Server, Shared, or Client scopes) instantly.
- **Remote Procedure Calls (RPC)** — Send one-way or two-way commands to your devices to trigger actions and receive immediate feedback.
- **Entity Discovery** — Use complex filters to find specific devices, assets, or other entities across your entire organization.
- **Alarm Monitoring** — Query and filter alarms by severity and status to maintain high operational awareness.

### How it works

1. Subscribe to this server
2. Provide your ThingsBoard Host URL and API Key
3. Start monitoring and controlling your hardware from Claude, Cursor, or any MCP client

### Who is this for?

- **IoT Engineers** — quickly debug device behavior and check telemetry without switching to the dashboard.
- **DevOps & SREs** — automate alarm reporting and system health checks via AI-driven queries.
- **Data Analysts** — extract latest sensor values and entity metadata for rapid prototyping and reporting.


## Available Tools
- **find_alarms**: Search alarms with severity and status filters
- **find_entities**: Search entities with complex filters
- **get_telemetry**: Read latest telemetry values for an entity
- **save_attributes**: g., SERVER_SCOPE, SHARED_SCOPE) for an entity.

Save attributes for an entity
- **save_telemetry**: g., DEVICE, ASSET).

Save time series telemetry data for an entity
- **send_oneway_rpc**: Send a one-way RPC command to a device
- **send_twoway_rpc**: Send a two-way RPC command to a device


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ThingsBoard** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the latest telemetry for device ID 'eb5672a0-1234-11ed'."

**🤖 AI Agent:**
> I've retrieved the telemetry for device eb5672a0-1234-11ed. The current temperature is 24.5°C and humidity is at 48%.

---

**👤 You:**
> "Send a two-way RPC command 'toggleSwitch' with params {'state': true} to device 'eb5672a0-1234-11ed'."

**🤖 AI Agent:**
> RPC command sent. The device responded with success: true. The switch state has been updated.

---

**👤 You:**
> "Find all active alarms with CRITICAL severity."

**🤖 AI Agent:**
> I found 2 critical alarms. One is a 'High Temperature' alarm on Thermostat-01 and the other is 'Connectivity Loss' on Gateway-Main.


## Installation & Usage

To install and use the **ThingsBoard** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thingsboard](https://vinkius.com/mcp/thingsboard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

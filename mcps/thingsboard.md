# ThingsBoard MCP Server

Manage your IoT ecosystem via ThingsBoard — monitor telemetry, control devices with RPC, and track alarms directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/thingsboard)

## Overview
**Category:** iot-hardware
**Tools Count:** 7

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


## Installation & Usage

To install and use the **ThingsBoard** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thingsboard](https://vinkius.com/mcp/thingsboard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

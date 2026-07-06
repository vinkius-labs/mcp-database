# ThingsBoard MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/thingsboard)
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


## Available Tools (7)
- **find_entities**: Search entities with complex filters
- **get_telemetry**: Read latest telemetry values for an entity
- **save_attributes**: g., SERVER_SCOPE, SHARED_SCOPE) for an entity.

Save attributes for an entity
- **save_telemetry**: g., DEVICE, ASSET).

Save time series telemetry data for an entity
- **send_oneway_rpc**: Send a one-way RPC command to a device
- **send_twoway_rpc**: Send a two-way RPC command to a device
- **find_alarms**: Search alarms with severity and status filters


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


## ❓ FAQ

**Q: Can I check the latest sensor readings for a specific device?**
Yes. Use the `get_telemetry` tool by providing the entity type and ID. The agent will return the most recent time-series data points recorded for that device.

**Q: Is it possible to trigger a physical action on a device, like turning on a light?**
Absolutely. You can use `send_oneway_rpc` for simple commands or `send_twoway_rpc` if you need to wait for a confirmation response from the device hardware.

**Q: How do I find all devices that currently have active critical alarms?**
You can use the `find_alarms` tool with a query body specifying the severity as 'CRITICAL' and status as 'ACTIVE_UNACK' or 'ACTIVE_ACK'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/thingsboard](https://vinkius.com/mcp/thingsboard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ThingsBoard** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `thingsboard` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ThingsBoard** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "thingsboard": {
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

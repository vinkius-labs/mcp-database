# Losant MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/losant)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Manage IoT applications, devices, and workflows via Losant — control hardware, query time-series data, and automate smart infrastructure directly from any AI agent.

## Description
Connect your **Losant** Enterprise IoT Platform to any AI agent and take full control of your connected environment through natural conversation.

### What you can do

- **Application Management** — List, create, and clone applications to organize your IoT resources efficiently.
- **Device Control** — Manage device fleets, send commands, and update device states or connection statuses in real-time.
- **Data Analytics** — Query time-series data, fetch last values, and export historical data for deep analysis.
- **Workflow Automation** — List and manage workflows, or trigger logic manually by pressing virtual buttons.
- **Data Tables & Storage** — Interact with data tables, manage files, and execute notebooks for advanced data processing.

### How it works

1. Subscribe to this server
2. Enter your Losant API Token
3. Start managing your IoT ecosystem from Claude, Cursor, or any MCP-compatible client

No more navigating complex dashboards to check a sensor value or trigger a maintenance workflow. Your AI acts as your IoT operations center.

### Who is this for?

- **IoT Engineers** — quickly inspect device states and debug workflows directly from the terminal or code editor.
- **Data Scientists** — retrieve historical sensor data for analysis without writing custom API scripts.
- **Operations Managers** — monitor fleet health and trigger manual overrides or reports through simple voice or text commands.


## Available Tools (38)
- **create_application**: Create a new Losant application
- **create_data_table**: Create a new data table
- **create_device**: Create a new device
- **create_workflow**: Create a new workflow
- **delete_application**: Delete a Losant application
- **delete_data_table_rows**: Delete rows from a data table
- **delete_device**: Delete a device
- **delete_workflow**: Delete a workflow
- **execute_notebook**: Execute a notebook
- **export_application**: Export a Losant application
- **export_data**: Export device data
- **get_application**: Get a specific Losant application
- **get_dashboard**: Get a specific dashboard
- **get_data_table_rows**: Get rows from a data table
- **get_device**: Get a specific device
- **get_workflow**: Get a specific workflow
- **import_application**: Import a Losant application
- **insert_data_table_row**: Insert a row into a data table
- **list_applications**: Get all Losant applications
- **list_dashboards**: Get all dashboards
- **list_data_tables**: Get data tables for an application
- **list_devices**: Get devices for an application
- **list_files**: Get files for an application
- **list_notebooks**: Get notebooks for an application
- **list_workflows**: Get workflows for an application
- **press_virtual_button**: Press a virtual button in a workflow
- **query_data_table_rows**: Query rows in a data table
- **query_last_value**: Query last value data
- **query_time_series**: Query time series data
- **send_dashboard_report**: Send a dashboard report
- **send_device_command**: Send a command to a device
- **send_device_state**: Send state data for a device
- **set_device_connection_status**: Set connection status for a device
- **update_application**: Update a Losant application
- **update_device**: Update a device
- **update_workflow**: Update a workflow
- **upload_file**: Upload a file to an application
- **clone_application**: Clone a Losant application


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Losant** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Losant applications."

**🤖 AI Agent:**
> I've retrieved your applications. You have 3 active apps: 'Smart Factory' (ID: 60a...), 'Office HVAC' (ID: 61b...), and 'Fleet Tracker' (ID: 62c...). Which one would you like to explore?

---

**👤 You:**
> "Show me all devices in application 60a123456789."

**🤖 AI Agent:**
> In the 'Smart Factory' application, I found 12 devices. 10 are currently 'Online' and 2 are 'Offline'. Notable devices include 'Main Boiler' and 'Assembly Line 1'. Would you like the details for a specific one?

---

**👤 You:**
> "Trigger the 'Emergency Reset' virtual button in workflow 5f987654321."

**🤖 AI Agent:**
> The virtual button for 'Emergency Reset' in workflow 5f987654321 has been successfully pressed. The workflow logic is now executing.


## ❓ FAQ

**Q: Can I manually trigger a Losant workflow using this integration?**
Yes! You can use the `press_virtual_button` tool by providing the Application ID and Workflow ID. This allows your AI agent to trigger specific automation logic on demand.

**Q: How do I check the current status of a specific sensor or device?**
Use the `get_device` tool with the Application ID and Device ID. The agent will return the full device metadata, including its last reported state and connection status.

**Q: Is it possible to retrieve historical data for analysis?**
Absolutely. You can use `query_time_series` to fetch historical attribute data or `query_last_value` for the most recent data points across your device fleet.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/losant](https://vinkius.com/mcp/losant)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Losant** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `losant` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Losant** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "losant": {
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

# Parklio PMS MCP Server

Manage smart parking hardware: barriers, displays, and gateways via Parklio PMS API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/parklio-pms)

## Overview
**Category:** iot-hardware
**Tools Count:** 10

## Description
Connect **Parklio PMS** to any AI agent and take full control of your smart parking infrastructure — manage barrier gates, digital displays, LPR cameras, and monitor hardware health through natural conversation.

### What you can do
- **Lot Management** — List and inspect all parking facilities in your network
- **Gateway Control** — Monitor barrier and camera status (online/offline)
- **Remote Operations** — Open/close barriers and reboot devices remotely
- **Display Messaging** — Update digital signs for maintenance or welcome messages
- **Activity Auditing** — View logs of all barrier movements and system events
- **System Health** — Get global operational metrics and uptime stats

### How it works
1. Subscribe to this server
2. Enter your Parklio Auth Token and Base URL
3. Start managing your parking hardware from Claude, Cursor, or any MCP-compatible client

Parklio is a forward-looking company dedicated to developing smart parking hardware and software solutions.

### Who is this for?
- **Parking Operators** — Monitor barrier health and update displays instantly without logging into the PMS dashboard
- **Maintenance Teams** — Remotely reboot offline gateways and check system logs for error diagnosis
- **Security Staff** — Review activity logs to audit unauthorized access or barrier overrides


## Available Tools
- **create_gateway**: Requires lot_id, name, and type (e.g., entry_barrier, exit_camera, lpr_reader). Use this when installing new physical hardware.

Register a new hardware gateway (barrier, reader) to a parking lot
- **list_displays**: Useful for auditing what drivers see when entering lots.

List digital display screens deployed in parking lots
- **run_gateway_operation**: Common operations: open_barrier, close_barrier, reboot, reset_error. Use this for remote troubleshooting or manual override of barriers.

Execute a remote operation on a specific gateway device
- **list_gateways**: Use this to audit hardware health and locate offline devices.

List all hardware gateways (barriers, cameras) connected to Parklio
- **pms_login**: Returns an authentication token valid for subsequent API calls. Use this to refresh your session token before making other requests.

Authenticate with the Parklio Parking Management System to get a token
- **get_activity_logs**: Optional lot_id filter. Use this for security auditing and operational troubleshooting.

View system activity and audit logs
- **get_lot_details**: Get detailed configuration and statistics for a specific parking lot
- **list_lots**: Essential for discovering available lots before managing hardware.

List all managed parking lots in the Parklio system
- **get_system_status**: Use this for a high-level operational check.

Get the overall health and operational status of the Parklio system
- **update_display_message**: Use for maintenance alerts ("Lot Full", "System Maintenance", "Welcome to VIP Parking").

Update the text shown on a digital display screen in a parking lot


## Installation & Usage

To install and use the **Parklio PMS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/parklio-pms](https://vinkius.com/mcp/parklio-pms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

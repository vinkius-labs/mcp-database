# Parklio PMS MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/parklio-pms)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/parklio-pms-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/parklio-pms-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [iot-hardware](../categories/iot-hardware.md)

Manage smart parking hardware: barriers, displays, and gateways via Parklio PMS API.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Parklio PMS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all offline gateways."

**🤖 AI Agent:**
> Found 2 offline gateways: 1. Exit Barrier at Lot A (Last seen 45m ago). 2. LPR Reader at Lot C (Last seen 2h ago). Recommend remote reboot.

---

**👤 You:**
> "Update display at Lot B to show 'Valet Parking This Way'."

**🤖 AI Agent:**
> Display updated successfully. Drivers entering Lot B will now see: 'Valet Parking This Way'.

---

**👤 You:**
> "Reboot the entry barrier at Lot A."

**🤖 AI Agent:**
> Reboot command sent to Gateway ID #101 (Entry Barrier Lot A). Status: Rebooting. Check system status in 2 minutes.


## Installation & Usage

To install and use the **Parklio PMS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/parklio-pms](https://vinkius.com/mcp/parklio-pms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

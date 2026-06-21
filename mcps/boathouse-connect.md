# Boathouse Connect MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/boathouse-connect)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/boathouse-connect-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/boathouse-connect-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage marina operations with boat slip reservations, customer records, and facility maintenance in one connected system.

## Description
Connect your **Boathouse Connect** account to any AI agent and manage your marina or rowing club operations through natural conversation.

### What you can do

- **Reservation Management** — List all reservations, inspect individual bookings, and create new equipment reservations
- **Equipment Inventory** — Browse the complete inventory of rowing shells, oars, and gear with availability status
- **Member Directory** — List all club members and view detailed profiles with contact info and membership tier
- **Location Management** — View all boathouse and marina locations configured in the system
- **Schedule Access** — List all practice and event schedules for the organization
- **Health Check** — Verify API connectivity and account status

### How it works

1. Subscribe to this server
2. Enter your **API Token** and **Whitelabel ID** from your Boathouse Connect account
3. Start managing your club from Claude, Cursor, or any MCP client

### Who is this for?

- **Club Managers** — check equipment availability and member reservations without opening the dashboard
- **Coaches** — review schedules and member rosters directly from the AI assistant
- **Operations Staff** — create reservations and monitor equipment inventory on the go


## Available Tools
- **check_boathouse_status**: Verify API connectivity
- **create_reservation**: Create a reservation
- **get_equipment**: Get equipment details
- **get_reservation**: Get reservation details
- **get_user**: Get member details
- **list_equipment**: List all equipment
- **list_locations**: List all locations
- **list_reservations**: List all reservations
- **list_schedules**: List all schedules
- **list_users**: List all members


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Boathouse Connect** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available rowing equipment."

**🤖 AI Agent:**
> Your club has 12 items: 4 singles (2 available), 3 doubles (1 available), 2 quads (both reserved), and 3 sets of oars. The singles 'Resolute' and 'Swift' are free tomorrow morning. Would you like to reserve one?

---

**👤 You:**
> "Book the single 'Resolute' for member usr_1029 on 2026-05-01 at 6AM."

**🤖 AI Agent:**
> Reservation confirmed! The single 'Resolute' (eq_0042) is booked for member Sarah K. (usr_1029) on May 1st at 6:00 AM. Reservation ID: res_8291. Would you like to check the schedule for that day?

---

**👤 You:**
> "Show me all club locations."

**🤖 AI Agent:**
> Your organization has 2 locations: 'Main Boathouse' at 123 River Road (8 rack slots, dock access) and 'South Marina' at 456 Harbor Ave (4 rack slots, covered storage). Would you like to see the equipment stored at each location?


## Installation & Usage

To install and use the **Boathouse Connect** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/boathouse-connect](https://vinkius.com/mcp/boathouse-connect)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# OfficeRnD Hybrid MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/officernd-hybrid)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/officernd-hybrid-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/officernd-hybrid-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Hybrid work management — book desks, rooms, and manage office resources via OfficeRnD.

## Description
Connect your **OfficeRnD Hybrid** account to empower your AI agents with office management capabilities. This server allows for seamless scheduling and resource coordination.

### What you can do

- **Desk & Room Booking** — Instantly create or cancel bookings for desks and meeting rooms
- **Resource Discovery** — List all available office resources, locations, and floors
- **Team Coordination** — View organization teams and employee directories
- **Event Monitoring** — Keep track of upcoming office events and community activities

### How it works

1. Subscribe to this server
2. Enter your **Client ID**, **Client Secret**, and **Org Slug**
3. Start managing your hybrid workspace from Claude, Cursor, or any MCP client


## Available Tools
- **cancel_booking**: Cancel an existing booking
- **create_booking**: Create a new booking
- **get_booking**: Get a specific booking
- **get_my_profile**: Get current user profile
- **list_bookings**: List all bookings
- **list_employees**: List all employees
- **list_events**: List organization events
- **list_locations**: List organization locations
- **list_resources**: List all resources (desks, rooms, etc.)
- **list_teams**: List organization teams


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OfficeRnD Hybrid** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available desks for today."

**🤖 AI Agent:**
> Fetching resources... I've found 12 available desks in the Main Office. Would you like to book one?

---

**👤 You:**
> "Book meeting room 'Zenith' for 2 PM today."

**🤖 AI Agent:**
> Creating booking for 'Zenith'... Success! Your reservation is confirmed from 2:00 PM to 3:00 PM.

---

**👤 You:**
> "Show my upcoming bookings."

**🤖 AI Agent:**
> Retrieving your bookings... You have a desk reserved for tomorrow at 9:00 AM and a meeting at 4:00 PM.


## Installation & Usage

To install and use the **OfficeRnD Hybrid** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/officernd-hybrid](https://vinkius.com/mcp/officernd-hybrid)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

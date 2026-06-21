# Condeco (Eptura Engage) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/condeco-eptura-engage)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/condeco-eptura-engage-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/condeco-eptura-engage-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage workspace bookings via Condeco — book meeting rooms, reserve hot desks, track availability, and handle office check-ins directly from any AI agent.

## Description
Connect your **Condeco** (now Eptura Engage) account to any AI agent and take full control of your enterprise workspace and desk booking workflows through natural conversation.

### What you can do

- **Office Location Navigation** — Identify bounded office capacities and geographic groupings mapping explicitly tracked buildings and campuses
- **Room Management** — Enumerate available meeting spaces, filtering by capacity and AV features, and check real-time usage states
- **Desk & Hot Desking** — Claim exclusive usage of hot desks within specific neighborhoods and zones, including equipment filters
- **Live Reservations** — Mutate active scheduling endpoints to book or cancel rooms and desks with instant sync to O365/Exchange
- **Check-in Automation** — Trigger physical presence capabilities to confirm your arrival at a location and satisfy local access controls
- **Booking History** — Extract chronological logs of user reservations to audit space utilization across your organization

### How it works

1. Subscribe to this server
2. Enter your Condeco/Eptura API Key (obtained from the Azure API Management Developer Portal)
3. Start managing your office space from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Enterprise Employees** — book desks and meeting rooms quickly without navigating complex web interfaces
- **Office Managers** — monitor space utilization and audit current check-ins through natural language
- **Operations Teams** — manage office locations and neighborhood boundaries across global campuses
- **DevOps/IT** — integrate workspace booking status into internal tools and dashboards


## Available Tools
- **list_locations**: Identify bounded office capacities discovering standard enterprise real estate limits
- **list_rooms**: Enumerate explicitly mapped meeting spaces filtering capacity and feature sets
- **get_room_availability**: Determine real-time usage states extracting explicit chronological meeting blocks
- **book_room**: Claim exclusive scheduling capabilities tracing synchronization triggers upon physical spaces
- **cancel_room_booking**: Revoke exact chronological reservations matching O365 sync boundaries
- **list_desks**: Identify specific bounding capacities covering mapped hot desks
- **book_desk**: Claim exclusive usage targeting specific hot desking bounds
- **cancel_desk_booking**: Revoke claimed exclusive desk reservations natively
- **list_bookings**: Extract chronological logs resolving explicit user booking reservations
- **check_in_to_location**: Trigger physical presence capabilities executing explicit local access controls


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Condeco (Eptura Engage)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all meeting rooms in the 'New York HQ' location"

**🤖 AI Agent:**
> I found 8 rooms in New York HQ. Available spaces include 'Manhattan Boardroom' (Cap: 20, AV: Yes) and 'Brooklyn Suite' (Cap: 6, AV: No). Would you like to check availability for any of these?

---

**👤 You:**
> "Book room 101 for tomorrow from 2:00 PM to 3:00 PM with title 'Weekly Sync'"

**🤖 AI Agent:**
> Room 101 booked successfully! Your reservation 'Weekly Sync' is confirmed for tomorrow. The booking has been synced to your calendar.

---

**👤 You:**
> "I've arrived at the office. Check me in to location 50"

**🤖 AI Agent:**
> Check-in complete! Your arrival at location 50 has been recorded. Your pending reservations for today are now auto-confirmed.


## Installation & Usage

To install and use the **Condeco (Eptura Engage)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/condeco-eptura-engage](https://vinkius.com/mcp/condeco-eptura-engage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

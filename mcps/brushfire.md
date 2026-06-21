# Brushfire MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/brushfire)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/brushfire-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/brushfire-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage events and attendees via Brushfire — track registrations, check-in guests, and monitor orders directly from any AI agent.

## Description
Connect your **Brushfire** account to any AI agent and orchestrate your event management, ticketing, and attendee synchronization through natural conversation.

### What you can do

- **Event Oversight** — List all your managed events, retrieve detailed metadata, and monitor ticket types.
- **Attendee Management** — List all registered guests for specific events, retrieve detailed profiles, and update information.
- **Real-time Check-in** — Mark attendees as checked-in directly from your workspace to track attendance.
- **Order Tracking** — List and inspect all event orders and transaction histories.
- **Registration Coordination** — Access and verify ticket/registration types to ensure your event setup is correct.
- **Account Insights** — Retrieve core account and site information straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your Brushfire API Key and Client Version
3. Start managing your events from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Event Organizers** — quickly check registration counts or attendee details without manual dashboard work.
- **On-site Staff** — perform check-ins and verify guest information straight from their mobile agent.
- **Finance Teams** — monitor event orders and transaction statuses using natural language.


## Available Tools
- **check_in_attendee**: Mark an attendee as checked-in
- **get_account_info**: Retrieve core account information
- **get_attendee**: Get details of a specific attendee
- **get_event**: Get details of a specific event
- **get_order**: Get details of a specific order
- **list_attendees**: List all attendees for a specific event
- **list_events**: List all managed events
- **list_orders**: List all event orders
- **list_ticket_types**: List ticket/registration types for an event
- **update_attendee**: Update attendee information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Brushfire** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my upcoming events in Brushfire."

**🤖 AI Agent:**
> I've retrieved your events. You have 3 upcoming conferences: 'Summer Summit 2026' (ID: ev_1), 'Tech Workshop' (ID: ev_2), and 'Global Gala' (ID: ev_3).

---

**👤 You:**
> "Show the attendee list for 'Summer Summit 2026'."

**🤖 AI Agent:**
> Retrieving attendees for Summer Summit... I found 150 registered guests, including Alice Johnson (Checked-in) and Bob Smith (Pending). Would you like to find someone specific?

---

**👤 You:**
> "Check-in attendee with ID att_99283."

**🤖 AI Agent:**
> Attendee att_99283 has been successfully checked-in for the event. Their status is now marked as present in Brushfire.


## Installation & Usage

To install and use the **Brushfire** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/brushfire](https://vinkius.com/mcp/brushfire)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Skedda MCP Server

Manage your workspace scheduling — create, update, and track bookings for desks, meeting rooms, and special venues directly through AI agents.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/skedda)

## Overview
**Category:** operations-management
**Tools Count:** 9

## Description
Connect your **Skedda** workspace to any AI agent to completely fully automate facility management and space scheduling. Handle your entire booking lifecycle through natural language conversations.

### What you can do

- **Space & Venue Discovery** — List all available physical spaces, venues, and their categorized groups (e.g., Office Hot Desks, Boardrooms)
- **Booking Operations** — Retrieve your current schedule, or instantly create, update, and delete reservations natively
- **User Management** — Look up fellow employees, customers, or members in the directory to assign them to bookings
- **Availability Tracking** — Filter your list of reservations by specific timeframes (ISO 8601) to identify empty slots

### How it works

1. Subscribe to this server
2. Provide your Skedda API Key from your venue settings
3. Start managing your workspace logistics straight from Claude, Cursor, or any MCP-compatible client

No more manually clicking through grid calendars to secure a hot desk for tomorrow or a boardroom for an upcoming client visit. Tell your AI pilot what you need, and it confirms the booking instantly.

### Who is this for?

- **Office Managers & Admins** — easily bulk-manage or delete bookings and quickly check occupancy levels without exporting data
- **Employees** — immediately reserve a meeting room on-the-go by chatting with your agent and assigning co-workers
- **Event Planners** — discover available spaces and categories to configure multi-day events efficiently


## Available Tools
- **create_booking**: Requires space ID, user ID, and start/end times.

Creates a new booking
- **delete_booking**: This action is irreversible.

Permanently deletes a booking
- **get_booking_details**: Retrieves details for a specific booking
- **list_bookings**: You can filter by date range.

Lists all bookings in Skedda
- **list_space_categories**: g., "Meeting Rooms", "Desks").

Lists space categories
- **list_spaces**: Lists all available spaces
- **list_users**: Lists all users in the Skedda account
- **list_venues**: Lists all venues
- **update_booking**: Updates an existing booking


## Installation & Usage

To install and use the **Skedda** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/skedda](https://vinkius.com/mcp/skedda)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

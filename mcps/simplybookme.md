# SimplyBook.me MCP Server

Enable your AI agent to manage appointments, browse staff calendars, and handle client records via the SimplyBook.me scheduling platform.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/simplybookme)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your AI to **SimplyBook.me**, the online appointment scheduling platform for service-based businesses.

### What you can do

- **Booking Management** — Create, update, and cancel appointments directly from chat using `create_booking`, `update_booking`, and `cancel_booking`.
- **Calendar Browsing** — View staff work calendars and available time slots with `get_work_calendar`.
- **Client Records** — List and inspect client profiles to check booking history and contact details.
- **Service Catalog** — Browse all services and events offered by the company, including pricing and duration.

### How it works

1. Add the SimplyBook.me integration to your AI toolset.
2. Provide your API Key, API Secret, and Company Login.
3. Manage your booking operations via natural language.

### Who is this for?

- **Salon & Spa Owners** — Schedule client appointments and check staff availability from chat.
- **Clinic Administrators** — Monitor upcoming consultations and manage patient bookings without opening the dashboard.
- **Service Teams** — Track group classes, events, and provider calendars in real time.


## Available Tools
- **create_booking**: Requires service ID, unit ID, and start time.

Creates a new booking
- **cancel_booking**: This action is irreversible.

Cancels a scheduled booking
- **update_booking**: Updates an existing booking
- **get_booking_details**: Retrieves details for a specific booking
- **get_work_calendar**: Retrieves the work calendar for a unit
- **list_bookings**: Lists all scheduled bookings
- **list_clients**: Lists company clients
- **list_events**: Lists specific calendar events or classes
- **list_services**: Lists all available services offered by the company
- **list_units**: Lists all service units (providers or locations)


## Installation & Usage

To install and use the **SimplyBook.me** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/simplybookme](https://vinkius.com/mcp/simplybookme)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

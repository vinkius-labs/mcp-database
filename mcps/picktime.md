# Picktime MCP Server

Equip your AI agent to manage scheduling operations. Fetch global availabilities, list locations, and manage business bookings via chat natively.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/picktime)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **Picktime** organization account to your AI agent and turn complex scheduling and availability management into a simple chat conversation.

### What you can do

- **Space & Resources** — Easily retrieve structural logistics utilizing `list_locations` and inspect the service portfolio actively using `list_services`.
- **Staff Management** — Gather team rosters through `list_staff` to orchestrate proper assignment mappings for upcoming reservations.
- **Booking Operations** — Execute deep audits with `list_bookings`, review detailed entries (`get_booking_details`), and cleanly back out utilizing `cancel_booking`.
- **Availability Mapping** — Audit live calendar empty spots using `get_availability` or check structured slots via `list_classes` for seamless planning.

### How it works

1. Subscribe to this server
2. Enter your Enterprise Picktime API Key
3. Start fetching availability windows or querying the status of corporate locations natively through Claude, Cursor, or any configured AI

### Who is this for?

- **Client Relations & Receptionists** — check if the stylist or doctor is free this afternoon without clicking through the calendar interface.
- **Business Directors** — extract all reservations of the day into a bulleted list to organize daily briefings and forecast team loads.
- **Tech Teams** — test availability integrations structurally from your terminal building enterprise webhook handlers.


## Available Tools
- **list_locations**: List all business locations configured in Picktime. Each location operates independently with its own services, staff, working hours, and booking pages. Multi-location businesses manage branches separately
- **get_location**: Used to resolve workspace boundaries before hitting schedules.

Get detailed configuration for a specific Picktime location by ID. Returns location name, address, timezone, working hours, booking URL, and linked calendar/payment integrations
- **list_services**: List all bookable services for a Picktime location. Returns service names, durations, prices, descriptions, assigned staff, and buffer times. Services define what customers can book
- **get_service_details**: Get detailed configuration for a specific Picktime service. Returns name, duration, price, description, staff assignments, booking limits, and cancellation policy
- **list_staff**: List all staff members at a Picktime location. Returns staff names, emails, roles, assigned services, working hours, and active status. Staff availability determines bookable time slots
- **list_bookings**: List all bookings for a Picktime location with optional date filter. Returns customer names, booked services, staff assignments, times, statuses, and payment info. Essential for schedule management
- **get_booking_details**: Get full details of a specific Picktime booking including customer contact info, service booked, staff assigned, start/end times, payment status, and any customer notes
- **cancel_booking**: Cancel a Picktime booking with a reason. The customer receives a cancellation notification and the time slot becomes available again for new bookings
- **list_classes**: List all group classes configured for a Picktime location. Classes are multi-attendee bookings with capacity limits — yoga sessions, workshops, group trainings
- **get_availability**: Get available booking time slots for a specific Picktime service on a given date. Returns free windows considering staff schedules, existing bookings, and buffer times. Essential for building custom booking flows


## Installation & Usage

To install and use the **Picktime** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/picktime](https://vinkius.com/mcp/picktime)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

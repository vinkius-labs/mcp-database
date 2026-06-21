# Robin MCP Server

Connect your AI assistant to Robin to seamlessly manage office locations, book meeting rooms, reserve hot desks, and monitor workplace availability directly from chat.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/robin)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your conversational assistant directly to **Robin**, the leading workplace management platform. This integration transforms your AI into a virtual office manager, empowering you to explore office locations, check room availability, and book desks directly from a seamless chat interface.

### What you can do

- **Manage Office Logistics** — Ask your assistant to map out your global organizational offices (`list_locations`) and review deep details like capacity or address for a specific hub (`get_location`).
- **Book Meeting Rooms** — See all bookable spaces (`list_spaces`) to find the perfect room for your meeting. Command the AI to check schedules (`list_space_events`, `get_free_busy`) and immediately book a room (`book_space`) for your team.
- **Reserve Hot Desks** — Explore the floor plan to find available seats (`list_desks`) and immediately secure a hot desk for a specific date (`reserve_desk`). If plans change, simply tell the AI to cancel your booking (`cancel_desk_reservation`).

### How it works

1. Install the Robin extension module in your MCP environment.
2. Obtain your `Robin Access Token` from your official dashboard and securely enter it in the authentication parameter below.
3. Converse naturally: "Check room availability in our main office tomorrow at 2 PM and book a desk for me."

### Who is this for?

- **Employees & Teams** — Quickly find available meeting rooms or hot desks without opening the web portal. Just ask the AI while planning your workday.
- **Office Managers** — Monitor space utilization and review upcoming events across different locations effortlessly.
- **Executive Assistants** — Manage aggressive scheduling by asking the AI to find free slots in multiple rooms and booking them instantly.


## Available Tools
- **book_space**: Specify space ID, title, and start/end times.

Books a meeting room by creating an event
- **cancel_desk_reservation**: You must provide the unique reservation ID.

Cancels an existing desk reservation
- **get_free_busy**: Provide a JSON array of space IDs.

Checks availability for multiple spaces within a time range
- **get_location**: Retrieves details for a specific office location
- **get_space**: Retrieves detailed information for a specific meeting space
- **list_desks**: Lists all hot desks and assigned seats at a location
- **list_locations**: Lists all office locations in Robin
- **list_space_events**: Lists all events booked in a specific meeting space
- **list_spaces**: Lists all bookable meeting rooms at a location
- **reserve_desk**: Reserves a hot desk for a specific date


## Installation & Usage

To install and use the **Robin** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/robin](https://vinkius.com/mcp/robin)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

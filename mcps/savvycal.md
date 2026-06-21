# SavvyCal MCP Server

Manage your SavvyCal scheduling links, check real-time availability, and coordinate automated bookings via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/savvycal)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **SavvyCal** account to any AI agent to streamline your meeting coordination. Let your AI agent act as your personal scheduling assistant without having to constantly switch tabs.

### What you can do

- **Scheduling Links** — View your active booking links, create new customized links dynamically, and manage URL slugs on the fly
- **Availability Constraints** — Query specific date ranges to find exactly when you are bookable across your various scheduling setups
- **Events Management** — List all upcoming scheduled meetings, get precise attendee details, and programmatically cancel appointments if needed
- **Account Settings** — Retrieve your base account profile and verify automated timezone settings

### How it works

1. Subscribe to this server
2. Enter your secure SavvyCal API Token
3. Start managing your calendar links from Claude, Cursor, or any MCP-compatible environment

Replace manual link juggling by having your agent fetch the right booking URL or calculate your free windows conversationally.

### Who is this for?

- **Founders & Executives** — ask your agent 'when am I free next week for a 45min chat?' and get the direct answer instantly
- **Sales & Consultants** — quickly generate a new, uniquely-named booking link for a specific client directly from your chat
- **Customer Success** — list upcoming client check-ins and cancel unconfirmed events with a single prompt


## Available Tools
- **cancel_event**: Specify the event ID and a cancellation reason.

Cancels a scheduled appointment
- **create_link**: Specify name, slug, and duration in minutes.

Creates a new scheduling link
- **delete_link**: This action is irreversible.

Permanently deletes a scheduling link
- **get_account**: Retrieves authenticated account information
- **get_event**: Retrieves details for a specific scheduled event
- **get_link**: Retrieves details for a specific scheduling link
- **list_availability**: Retrieves available time slots for a link within a date range
- **list_events**: Lists all scheduled booking events
- **list_links**: Lists all scheduling links in the SavvyCal account
- **update_link**: Updates an existing scheduling link


## Installation & Usage

To install and use the **SavvyCal** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/savvycal](https://vinkius.com/mcp/savvycal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

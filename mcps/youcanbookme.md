# YouCanBook.me MCP Server

Automate scheduling workflows via YouCanBook.me — manage booking pages, appointments, and availability directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/youcanbookme)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Connect your **YouCanBook.me** account to any AI agent and take full control of your scheduling infrastructure through natural conversation.

### What you can do

- **Booking Page Management** — List all shareable scheduling pages (profiles) and retrieve detailed configurations including timezones and linked calendars
- **Appointment Monitoring** — List and query bookings across your profiles, filtered by status (tentative, upcoming, finished, cancelled)
- **Deep Booking Audit** — Retrieve full details for any specific appointment, including attendee info and custom form responses
- **Programmatic Booking** — Initiate the scheduling flow by creating booking intents and retrieving available time slots for user confirmation
- **Cancellation Control** — Instantly revoke appointments and automatically notify attendees through simple chat commands
- **Team Coordination** — List all staff members assigned to a booking page to see which technicians or consultants are available
- **Account Insights** — Verify your account standing, base timezone, and active calendar integrations directly from your agent

### How it works

1. Subscribe to this server
2. Enter your YouCanBook.me API Key and Account ID
3. Start managing your appointments through Claude, Cursor, or any MCP-compatible client

No more manual filtering through booking dashboards to find an attendee's email. Your AI agent becomes your personal scheduling coordinator.

### Who is this for?

- **Sales & Success Teams** — monitor upcoming customer calls and verify attendee information before meetings
- **Small Business Owners** — manage booking page availability and cancel appointments on the go via chat
- **Executive Assistants** — coordinate schedules across multiple profiles and team members without manual navigation
- **Product Teams** — implement programmatic booking flows and verify availability slots through simple conversation


## Available Tools
- **list_profiles**: Lists all booking pages (profiles) in the YouCanBook.me account
- **get_profile**: Retrieves detailed configuration for a specific booking page
- **list_bookings**: Status options: tentative, upcoming, finished, cancelled.

Queries bookings for a specific profile with optional status filtering
- **get_booking**: Retrieves full details for a specific YouCanBook.me booking
- **cancel_booking**: This action removes the calendar event and is irreversible.

Permanently cancels a booking and notifies the attendee
- **create_intent**: Provide the profile subdomain (e.g. "mycompany"). Returns an intent ID.

Creates a booking intent to initiate the programmatic scheduling process
- **get_availability**: Retrieves bookable time slots for an active booking intent
- **confirm_intent**: Finalizes a booking intent, creating the official appointment
- **get_account**: Retrieves details about the YouCanBook.me account and plan
- **list_team_members**: Lists all team members assigned to a specific booking page


## Installation & Usage

To install and use the **YouCanBook.me** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/youcanbookme](https://vinkius.com/mcp/youcanbookme)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

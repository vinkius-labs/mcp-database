# Corsizio MCP Server

Equip your AI agent to manage event registrations, attendees, and payments through the Corsizio API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/corsizio)

## Overview
**Category:** productivity
**Tools Count:** 10

## Description
Integrate **Corsizio**, the streamlined event registration platform, directly into your AI workflow. Manage your classes, workshops, and seminars, track attendee lists, and monitor revenue using natural language.

### What you can do

- **Event Management** — List and retrieve details for all your upcoming and past events.
- **Attendee Tracking** — Quickly access registration lists and individual attendee profiles.
- **Financial Monitoring** — Track payments, refunds, and coupon usage across your events.
- **Account Statistics** — Get real-time insights into your total registrations and account growth.

### How it works

1. Connect the Corsizio integration to your AI assistant.
2. Authorize using your Corsizio Secret API Key (found in Account Settings > Developer API).
3. Manage your event lifecycle through intuitive conversation.

### Who is this for?

- **Event Organizers** — Quickly check registration counts and attendee details on the go.
- **Instructors & Teachers** — Access class lists and student information directly via chat.
- **Business Admins** — Monitor event revenue and financial transactions efficiently.


## Available Tools
- **get_account_stats**: Resolves total revenue, registration counts, and event performance metrics.

Retrieve high-level statistics for your Corsizio account
- **get_attendee_details**: Touches personal details, payment history, and event enrollment boundaries.

Get full registration profile for an attendee
- **get_event_details**: Touches event configuration, pricing, and registration boundary.

Get detailed information for a specific event
- **list_attendees**: Resolves attendee name, email, registration date, and payment status.

List all registered attendees for a specific event
- **list_coupons**: Resolves code names, discount amounts (percentage or fixed), and expiration constraints.

List all discount codes and coupons
- **list_events**: Resolves properties such as event ID, name, date, time, and current registration status.

List all events in your Corsizio account
- **list_instructors**: Resolves instructor names, contact info, and associated specialties.

List all instructors or teachers
- **list_locations**: Resolves location names, addresses, and capacity limits.

List physical or online locations for events
- **list_payments**: Resolves payment IDs, amounts, currencies, and associated event/attendee references.

List all payment transactions
- **list_refunds**: Resolves refund amount, original transaction reference, and processing date.

List all processed refunds


## Installation & Usage

To install and use the **Corsizio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/corsizio](https://vinkius.com/mcp/corsizio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

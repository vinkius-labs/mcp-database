# Restful Booker MCP Server

Manage hotel bookings via the Restful Booker API—create, retrieve, update, and delete reservations directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/restful-booker)

## Overview
**Category:** developer-tools
**Tools Count:** 8

## Description
Connect to the **Restful Booker** API to manage hotel reservations. This server allows your AI agent to handle the full lifecycle of bookings, from initial creation to final deletion.

### What you can do

- **Booking Discovery** — List all booking IDs or filter by guest names and dates using `get_booking_ids`
- **Detailed Inspection** — Retrieve full metadata, pricing, and dates for any specific reservation with `get_booking`
- **Reservation Creation** — Instantly create new entries in the system using `create_booking`
- **Flexible Updates** — Modify existing bookings entirely with `update_booking` or change specific fields with `partial_update_booking`
- **Secure Access** — Generate authentication tokens via `create_token` to authorize sensitive write and delete operations

### How it works

1. Subscribe to this server
2. Use the `create_token` tool with your credentials to get an access token
3. Start managing hotel data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — testing API integrations and CRUD workflows in a reliable sandbox environment
- **QA Engineers** — automating reservation scenarios and data validation through natural language
- **Hospitality Tech Teams** — prototyping AI-driven booking assistants and management tools


## Available Tools
- **create_booking**: Create a new booking
- **create_token**: Create a new auth token
- **delete_booking**: Requires auth token.

Delete a booking
- **get_booking_ids**: Can take optional query strings to search.

Get all booking IDs
- **get_booking**: Get a specific booking
- **health_check**: API health check
- **partial_update_booking**: Requires auth token.

Partially update a booking
- **update_booking**: Requires auth token.

Update a current booking


## Installation & Usage

To install and use the **Restful Booker** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/restful-booker](https://vinkius.com/mcp/restful-booker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

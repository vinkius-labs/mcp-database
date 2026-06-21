# Restful Booker MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/restful-booker)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/restful-booker-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/restful-booker-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage hotel bookings via the Restful Booker API—create, retrieve, update, and delete reservations directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Restful Booker** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all booking IDs for guests with the last name 'Smith'."

**🤖 AI Agent:**
> I found 3 booking IDs for 'Smith': 45, 102, and 215. Would you like me to fetch the full details for any of these?

---

**👤 You:**
> "Create a new booking for John Doe, price 150, deposit paid, from 2024-12-01 to 2024-12-05."

**🤖 AI Agent:**
> Booking successfully created! The new booking ID is 882. The guest is John Doe with a check-in on Dec 1st and check-out on Dec 5th.

---

**👤 You:**
> "Update booking 882 to change the total price to 200."

**🤖 AI Agent:**
> I've updated the total price for booking 882 to 200 using a partial update. All other details remain the same.


## Installation & Usage

To install and use the **Restful Booker** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/restful-booker](https://vinkius.com/mcp/restful-booker)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

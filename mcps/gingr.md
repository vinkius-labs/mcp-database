# Gingr MCP Server

Retrieve pet owner profiles, track reservations, and oversee check-ins via AI agents with Gingr.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gingr)

## Overview
**Category:** customer-support
**Tools Count:** 10

## Description
Connect your **Gingr** pet care management account to any AI agent to automate your data extraction and customer support workflows through the Model Context Protocol (MCP). Gingr is the leading platform for kennel, daycare, and grooming businesses. This MCP server enables you to retrieve detailed pet owner profiles, track upcoming and past reservations, and monitor real-time facility check-ins directly through natural conversation.

### Key Features

- **Owner & Pet Insights** — Retrieve complete profile metadata for pet owners using IDs, email addresses, or phone numbers.
- **Reservation Tracking** — List all boarding, daycare, and grooming reservations for any owner, filtered by status (future or currently checked-in).
- **Digital Whiteboard Oversight** — Access 'Back of House' data to see real-time facility activity and room assignments for any location.
- **Custom Data Discovery** — Search across custom metadata fields for both owners and animals to find specific regional or internal attributes.
- **Facility Transparency** — List all business locations and facilities configured in your Gingr app.
- **Read-only Security** — Safely query your pet care database with a secure, read-only integration designed for data visibility.
- **Real-time Synchronization** — Keep your facility operations data accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Gingr Subdomain and API Key (found in User Settings)
3. Start querying your pet care data from Claude, Cursor, or any MCP client

### Who is this for?

- **Pet Care Facility Managers** — quickly check check-in statuses or room assignments without manual dashboard navigation.
- **Customer Support Teams** — get a real-time overview of an owner's reservation history via simple AI commands.
- **Operations Leads** — automate the retrieval of facility activity data for daily reporting.


## Available Tools
- **verify_api_connection**: Check connection
- **list_active_checkins**: List currently checked-in
- **find_owner_by_email**: Search owner by email
- **get_pet_owner_details**: Get owner profile
- **find_owner_by_phone**: Search owner by phone
- **get_digital_whiteboard**: View active whiteboard
- **list_business_locations**: List pet care facilities
- **list_owner_reservations**: ) for a specific owner.

List past/future bookings
- **search_pet_custom_fields**: Search custom pet data
- **search_owner_custom_fields**: Search custom owner data


## Installation & Usage

To install and use the **Gingr** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gingr](https://vinkius.com/mcp/gingr)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

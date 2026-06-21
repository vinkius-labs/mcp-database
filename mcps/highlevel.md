# HighLevel MCP Server

Automate CRM and marketing via HighLevel — manage contacts, opportunities, and calendars directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/highlevel)

## Overview
**Category:** growth-engine
**Tools Count:** 11

## Description
Connect your **HighLevel** (GoHighLevel) account to any AI agent and take full control of your sales pipeline, contact management, and scheduling through natural conversation.

### What you can do

- **Contact Oversight** — Perform advanced searches for leads, retrieve full profiles, and create new contact records effortlessly.
- **Sales Pipelines** — List pipelines and search for opportunities to monitor your deals and revenue flow.
- **Appointment Management** — Access your calendars, check for free slots in real-time, and book appointments directly from the chat.
- **Task Coordination** — List and create tasks for specific contacts to ensure follow-ups are never missed.
- **Location Tracking** — Retrieve location-specific tags to categorize and filter your data accurately.
- **Unified CRM** — Bridge the gap between your marketing and sales activities using the powerful API v2.

### How it works

1. Subscribe to this server
2. Enter your HighLevel API v2 Access Token
3. Start managing your CRM from Claude, Cursor, or any MCP-compatible client

No more jumping between complex dashboard views. Your AI assistant acts as a dedicated Sales Assistant or Marketing Operations Lead.

### Who is this for?

- **Marketing Agencies** — instantly retrieve lead details and opportunity statuses for multiple clients.
- **Sales Reps** — automate the process of logging follow-up tasks and booking meetings.
- **Business Owners** — maintain a real-time overview of their sales funnel and appointments.


## Available Tools
- **create_appointment**: Book a new appointment on a calendar
- **create_contact**: Pass payload as JSON string in "body_json" (requires firstName, email, or phone).

Add a new contact/lead to HighLevel
- **create_contact_task**: Assign a new task to a specific contact
- **get_contact_details**: Get detailed information for a specific contact
- **get_calendar_free_slots**: Check availability for a specific calendar
- **list_calendars**: List all calendars available for a location
- **list_contact_tasks**: List all tasks assigned to a specific contact
- **list_pipelines**: List sales pipelines for a specific location
- **list_location_tags**: List all custom tags for a location
- **search_contacts**: Pass search criteria as a JSON string in "search_json".

Search for contacts in HighLevel
- **search_opportunities**: Search for opportunities within a pipeline


## Installation & Usage

To install and use the **HighLevel** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/highlevel](https://vinkius.com/mcp/highlevel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

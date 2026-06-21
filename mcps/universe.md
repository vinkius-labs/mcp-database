# Universe MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/universe)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/universe-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/universe-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage events, ticketing, and guestlists via Universe — list events, check in attendees, and handle access keys directly from your AI agent.

## Description
Connect your **Universe** host account to any AI agent to streamline event operations and attendee management through natural conversation.

### What you can do

- **Event Discovery** — List all events and listings for specific hosts or users to get a bird's-eye view of your schedule
- **Attendee Management** — Retrieve detailed guestlists, order information, and custom form answers for any event
- **Check-in Operations** — Mark tickets as checked-in instantly using ticket IDs, perfect for front-of-house automation
- **Ticketing & Tokens** — Fetch QR code tokens for attendees and manage private access keys for exclusive ticket types
- **Data Analysis** — Query orders and rates to understand sales performance and attendee demographics

### How it works

1. Subscribe to this server
2. Enter your Universe Personal Access Token
3. Start managing your events from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Event Organizers** — quickly check guest counts and event statuses without digging through the Universe dashboard
- **On-site Staff** — automate check-in verification and attendee lookups via voice or chat
- **Marketing Teams** — analyze attendee data and order history to optimize future event listings


## Available Tools
- **create_access_key**: Manage access keys for private tickets
- **check_in**: Mark a ticket as checked-in
- **get_events**: Get list of events for a host
- **list_guestlists**: Can be filtered by event or listing.

Retrieve attendee information for events or listings
- **list_listings**: Retrieve a list of event listings
- **get_event_orders**: Get orders and attendees for an event
- **get_event_tokens**: Get attendee QR code tokens


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Universe** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active events for host ID 98765."

**🤖 AI Agent:**
> I've retrieved the events for host 98765 using `get_events`. You have 'Tech Summit 2024' (ID: 112233) and 'AI Workshop' (ID: 445566) currently active. Which one would you like to manage?

---

**👤 You:**
> "Show me the guestlist for event 112233."

**🤖 AI Agent:**
> Fetching the guestlist for event 112233 via `list_guestlists`... I found 150 attendees. Recent registrations include Alice Smith and Bob Jones. Would you like to see the custom form answers for these guests?

---

**👤 You:**
> "Check in ticket ID 556677."

**🤖 AI Agent:**
> Processing check-in for ticket 556677 using `check_in`... Success! The attendee has been marked as checked-in for the event in Universe.


## Installation & Usage

To install and use the **Universe** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/universe](https://vinkius.com/mcp/universe)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

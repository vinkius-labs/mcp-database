# Ticket Tailor MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ticket-tailor)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ticket-tailor-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ticket-tailor-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Sell event tickets with low fees, custom branding, and seating charts that give you full control over the ticketing experience.

## Description
Connect your **Ticket Tailor** account to any AI agent and simplify how you manage your event registrations, ticket sales, and attendee data through natural conversation.

### What you can do

- **Event Oversight** — List all active and past events and retrieve detailed metadata and configuration settings.
- **Order Tracking** — List and query sales orders, optionally filtered by event, to monitor your revenue and sales velocity.
- **Ticket Inventory** — List different ticket types and tiers for any event to manage your pricing strategy.
- **Attendee Management** — List individual issued tickets to verify participants and check-in statuses.
- **Commercial Insights** — Fetch detailed metadata for specific orders and events directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your Ticket Tailor API Key (found in your account settings)
3. Start managing your event ticketing from Claude, Cursor, or any MCP client

### Who is this for?

- **Event Organizers** — quickly retrieve attendee counts and event metadata via simple AI commands.
- **Customer Support Teams** — verify ticket orders and check issued ticket details directly from the workspace.
- **Marketing Managers** — monitor sales progress and ticket tier availability via the AI assistant.


## Available Tools
- **get_event_details**: Get details for a specific event
- **list_events**: List Ticket Tailor events
- **list_issued_tickets**: List individual issued tickets
- **list_event_orders**: Optionally filter by event ID.

List orders
- **list_ticket_types**: List ticket types for an event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ticket Tailor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active events in my Ticket Tailor account."

**🤖 AI Agent:**
> I've retrieved your events. You have 3 upcoming events: 'Tech Conference 2024', 'Summer Music Festival', and 'AI Workshop Series'. Which one would you like to see sales data for?

---

**👤 You:**
> "Show me the ticket tiers for 'Tech Conference 2024' (ID: ev_10293)."

**🤖 AI Agent:**
> I've fetched the ticket types for ev_10293. You have: 'Early Bird' ($150), 'Standard Entry' ($250), and 'VIP All-Access' ($500). 'Early Bird' is currently sold out.

---

**👤 You:**
> "How many tickets were issued for the 'Summer Music Festival'?"

**🤖 AI Agent:**
> Retrieving data... For the 'Summer Music Festival' (ID: ev_88231), a total of 450 tickets have been issued so far. Shall I list the most recent orders?


## Installation & Usage

To install and use the **Ticket Tailor** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ticket-tailor](https://vinkius.com/mcp/ticket-tailor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

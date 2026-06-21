# Eventbrite MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eventbrite-extended)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eventbrite-extended-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eventbrite-extended-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Create events, sell tickets, and manage attendees with the world largest self-service ticketing platform for any occasion.

## Description
Connect your **Eventbrite** organizational account to any AI agent and take full control of your event planning and ticketing workflows through natural conversation.

### What you can do

- **Event Orchestration** — List and manage events across multiple organizations and retrieve detailed metadata including descriptions and status programmatically
- **Ticketing Control** — Access and monitor ticket classes for any event to track availability and sales performance in real-time
- **Attendee Management** — Retrieve complete directories of registered attendees and monitor individual orders to coordinate entry and engagement
- **Venue & Logistics** — Create and manage physical event locations (venues) programmatically to streamline your event logistics
- **Organizational Visibility** — Access your complete organization directory and user profile information to maintain high-fidelity oversight

### How it works

1. Subscribe to this server
2. Retrieve your **Private Token** from the Eventbrite App Management page
3. Start managing your events and registrations from Claude, Cursor, or any MCP client

No more manual status checking or complex navigation through fragmented event dashboards. Your AI acts as your dedicated event operations and ticketing coordinator.

### Who is this for?

- **Event Organizers** — instantly retrieve registration counts and update event details using natural language commands
- **Marketing Teams** — monitor ticket sales and attendee growth without leaving your communication tools
- **Operations Leads** — automate the creation of venues and manage event logistics through simple AI queries


## Available Tools
- **list_event_attendees**: List attendees for an event
- **create_event**: Requires event name, start and end dates, and currency.

Create a new Eventbrite event
- **create_organization_venue**: Requires venue name and address.

Create a new venue for an organization
- **get_event**: Get details for a specific Eventbrite event
- **get_order**: Get details for a specific Eventbrite order
- **get_me**: Get current Eventbrite user details
- **list_event_orders**: List orders for an event
- **list_organization_events**: List events for an organization
- **list_organizations**: Most operations require an Organization ID.

List Eventbrite organizations
- **list_event_ticket_classes**: List ticket classes for an event
- **update_event**: Update an existing Eventbrite event
- **list_organization_venues**: List venues for an organization


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eventbrite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active organizations on Eventbrite."

**🤖 AI Agent:**
> I've retrieved your organizations. You currently have access to: 'Tech Events Global' (ID: 123) and 'Internal Workshops' (ID: 456). Which one should we explore for events?

---

**👤 You:**
> "Show me the last 5 events for organization ID '123'."

**🤖 AI Agent:**
> Scanning events for organization 123... I found 5 recent entries, including 'AI Summit 2026' and 'Product Launch Party'. Would you like the registration counts for any of these?

---

**👤 You:**
> "Get attendee details for event ID '67890'."

**🤖 AI Agent:**
> Fetching attendee list... There are 150 participants registered for event 67890. Notable attendees include 'John Doe' and 'Sarah Smith'. I can provide individual registration metadata if needed.


## Installation & Usage

To install and use the **Eventbrite** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eventbrite-extended](https://vinkius.com/mcp/eventbrite-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

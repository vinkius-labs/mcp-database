# Eventzilla MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/eventzilla)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/eventzilla-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/eventzilla-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to manage event registrations, track ticket orders, and monitor discount codes via the Eventzilla API.

## Description
Integrate **Eventzilla**, the leading event registration and marketing platform, directly into your AI workflow. Manage your upcoming events and classes, track registered attendees and ticket transactions, monitor performance metrics and discount code usage, and oversee your entire event operation using natural language.

### What you can do

- **Event Oversight** — List and retrieve detailed information, dates, and status for all your Eventzilla events and webinars.
- **Registration Intelligence** — Monitor registered attendees, resolving names, emails, and ticket types across your events.
- **Financial Management** — Access and monitor ticket orders and transactions, tracking gross sales and payment statuses in real-time.
- **Event Auditing** — Retrieve high-level summaries of registration volume, check-in rates, and organizational event health instantly.

### How it works

1. Connect the Eventzilla integration to your AI assistant.
2. Authorize using your Eventzilla API Key (found in your account settings).
3. Orchestrate your event marketing and registration strategy through intuitive conversation.

### Who is this for?

- **Event Organizers** — Quickly check attendee counts and ticket sales on the go.
- **Marketing Teams** — Research discount code performance and sales telemetry via chat during campaign planning.
- **Operations Teams** — Monitor registration progress and organizational event metadata instantly.


## Available Tools
- **get_eventzilla_account_metadata**: Retrieve metadata and limits for your Eventzilla account
- **get_event_performance_summary**: Get a summary of performance metrics for a specific event
- **get_event_detailed_data**: Get detailed settings and information for a specific event
- **quick_event_volume_audit**: Retrieve a high-level summary of attendees and orders
- **list_event_attendees**: List all registered attendees for a specific event
- **list_event_discount_codes**: List all active and inactive discount codes for a specific event
- **list_all_events**: List all events managed in your Eventzilla account
- **list_currently_live_events**: Identify events that are currently taking place or open for registration
- **list_event_ticket_orders**: List all ticket orders and transactions for a specific event
- **list_future_scheduled_events**: Identify events that are scheduled for a future date


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Eventzilla** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active event registrations."

**🤖 AI Agent:**
> I've found 5 active events, including 'Annual Industry Gala' and 'Advanced Python Workshop'. The Industry Gala currently has 150 registrations. Would you like to see the ticket sales summary for the workshop?

---

**👤 You:**
> "Show me the attendee list for 'Python Workshop'."

**🤖 AI Agent:**
> For 'Advanced Python Workshop', I've retrieved the list of 45 attendees, including 'Jane Smith' and 'John Doe'. All attendees have 'Paid' status. Should I pull the discount codes used for these registrations?

---

**👤 You:**
> "Check active discount codes for event ID '12345'."

**🤖 AI Agent:**
> For event ID '12345', you have 3 active discount codes: 'EARLYBIRD' (20% off), 'VIPACCESS' (Free), and 'GROUP10'. EARLYBIRD has been used 45 times out of 50. Would you like to see the usage for VIPACCESS?


## Installation & Usage

To install and use the **Eventzilla** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/eventzilla](https://vinkius.com/mcp/eventzilla)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

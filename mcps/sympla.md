# Sympla MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sympla)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/sympla-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/sympla-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Orchestrate Sympla events — manage ticket orders, handle check-ins, and track event statistics directly from any AI agent.

## Description
Connect your AI agents to **Sympla**, the leading event management and ticketing platform in Brazil. This MCP provides 10 tools to manage the full lifecycle of your events, from attendee list orchestration and ticket order retrieval to real-time check-in processing and event performance analytics.

### What you can do

- **Event Orchestration** — List and inspect your published events and retrieve granular metadata for each session
- **Attendee Management** — Retrieve detailed participant lists and filter by ticket status or registration date
- **Ticket Lifecycle** — Manage individual ticket orders, retrieve QR codes, and monitor payment statuses
- **Check-in Automation** — Process attendee check-ins programmatically based on ticket IDs or QR data
- **Performance Insights** — Access real-time statistics on ticket sales, revenue, and attendance rates directly through natural conversation

### How it works

1. Subscribe to this server
2. Log in to your [**Sympla account**](https://www.sympla.com.br/)
3. Navigate to **Integrations > API** to generate your **Personal Access Token** (s_token)
4. Identify your **Event IDs** from the event management dashboard
5. Insert your token into the fields below to start managing your events.

### Who is this for?

- **Event Organizers** — automate the retrieval of daily attendee lists and check-in reports via natural language
- **Marketing Teams** — monitor real-time ticket sales performance and revenue trends smoothly
- **AEC & Venue Managers** — integrate event data into broader physical facility management systems


## Available Tools
- **checkin_participant_by_id**: Validate event entry using participant ID
- **checkin_participant_by_ticket**: Validate event entry using ticket number
- **get_event_details**: Get detailed information for a specific event
- **get_order_details**: Get detailed info for a specific order
- **get_participant_details**: Get detailed profile for a participant by ID
- **list_events**: List all events owned by your Sympla account
- **list_event_orders**: List all orders (purchases) for a specific event
- **list_event_participants**: List all participants (attendees) for an event
- **list_event_presentations**: List multi-date event presentations
- **search_participant_by_ticket**: Find a participant using their ticket number


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sympla** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all participants registered for my event 'Tech Conf 2024' (ID: 123456)."

**🤖 AI Agent:**
> Retrieving attendee list for 'Tech Conf 2024'... I've found 45 registered participants. Key attendees include John Doe (Premium Ticket), Jane Smith (General Admission), and Robert Brown (VIP). Would you like the full export?

---

**👤 You:**
> "Show me the sales performance summary for event ID 'ev_999'."

**🤖 AI Agent:**
> Connecting to Sympla stats engine... For event 'Summer Festival' (ID: ev_999): 150/200 tickets sold (75% occupancy). Total revenue: R$ 7,500.00. Sales peaked yesterday between 6 PM and 9 PM.

---

**👤 You:**
> "Perform check-in for ticket ID 'tkt_abc123'."

**🤖 AI Agent:**
> Requesting check-in from Sympla server... Success! Ticket 'tkt_abc123' has been checked in. Participant: Alice White. Attendance count for your event has been updated.


## Installation & Usage

To install and use the **Sympla** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sympla](https://vinkius.com/mcp/sympla)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

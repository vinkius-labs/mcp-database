# Hipsy MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hipsy)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hipsy-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hipsy-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Sell event tickets, manage registrations, and promote parties and festivals with a ticketing platform made for nightlife and entertainment.

## Description
Connect your **Hipsy** account to any AI agent and manage your event ticketing operations through natural conversation.

### What you can do

- **Organisation Management** — List all event organisations and inspect individual profiles
- **Event Browsing** — List all events, filter upcoming or past events, and inspect full event details with ticket types and sales data
- **Order Tracking** — Browse all ticket orders, filter by event, and inspect individual order details with buyer info and payment status
- **Ticket Configuration** — View all ticket types for an event with pricing and availability
- **Attendee Management** — List all attendees for an event with check-in status
- **Scan Analytics** — Review ticket scan entries and aggregate check-in statistics (total scanned, scan rate)
- **Revenue Reporting** — Retrieve total revenue, ticket sales breakdown, and payment data per event
- **Webhooks** — List all configured webhook endpoints

### How it works

1. Subscribe to this server
2. Enter your Hipsy API Key from your account settings
3. Start managing events from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Event Organisers** — track ticket sales, monitor check-ins in real time, and review post-event revenue without opening the dashboard
- **Venue Managers** — monitor attendee flow, scan rates, and capacity utilization
- **Finance Teams** — audit revenue reports, payment breakdowns, and order histories through AI


## Available Tools
- **check_hipsy_status**: Verify connectivity
- **get_event_revenue**: Get event revenue
- **get_event**: Get event details
- **get_order**: Get order details
- **get_organisation**: Get organisation details
- **get_scan_stats**: Get scan statistics
- **list_attendees**: List attendees
- **list_events**: List all events
- **list_orders_by_event**: List orders by event
- **list_orders**: List all orders
- **list_organisations**: List organisations
- **list_past_events**: List past events
- **list_scans**: List scan entries
- **list_ticket_types**: List ticket types
- **list_upcoming_events**: List upcoming events
- **list_webhooks**: List webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hipsy** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all upcoming events and the ticket sales for the next one."

**🤖 AI Agent:**
> 4 upcoming events: 1) 'Summer Music Festival' — Jul 15, 2025 (event_301, Venue: Park Stage). 2) 'Tech Meetup Amsterdam' — Jul 22 (event_302). 3) 'Outdoor Cinema Night' — Aug 5 (event_303). 4) 'Food & Wine Fest' — Aug 18 (event_304). Ticket sales for 'Summer Music Festival': 3 ticket types: Early Bird (€25, 200/200 sold — SOLD OUT), Regular (€40, 142/300 sold), VIP (€85, 28/50 sold). Total orders: 370. Revenue: €18,430. Would you like to see attendee check-in stats or order details?

---

**👤 You:**
> "Show the check-in stats for last Saturday's event and any attendees who haven't checked in."

**🤖 AI Agent:**
> Check-in stats for 'Jazz Night' (event_298, Apr 19): Total tickets sold: 185. Checked in: 162 (87.6% scan rate). Unique scans: 162. Not checked in: 23 attendees. No-show highlights: 5 VIP tickets (€85 each = €425 unredeemed), 18 Regular tickets. Peak check-in window: 7:00-7:30 PM (68 scans). Last scan: 9:15 PM. Would you like to see the revenue report or export the attendee list?

---

**👤 You:**
> "Show the revenue report for all past events this month."

**🤖 AI Agent:**
> 3 past events this month. Total revenue: €32,780. Breakdown: 1) 'Jazz Night' (Apr 19) — €12,450 (185 tickets). Payment: 82% card, 18% iDEAL. 2) 'Art Exhibition Opening' (Apr 12) — €8,330 (92 tickets). Payment: 75% card, 25% iDEAL. 3) 'Comedy Show' (Apr 5) — €12,000 (240 tickets). Payment: 90% card, 10% iDEAL. Average ticket price: €63.40. Average attendance rate: 89.2%. Would you like to compare with last month or check webhook configurations?


## Installation & Usage

To install and use the **Hipsy** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hipsy](https://vinkius.com/mcp/hipsy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

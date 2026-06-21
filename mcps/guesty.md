# Guesty MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/guesty)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/guesty-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/guesty-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Automate vacation rental management via Guesty — manage reservations, listings, guests, and calendars directly from any AI agent.

## Description
Connect your **Guesty** property management platform to any AI agent and take full control of your vacation rental operations through natural conversation.

### What you can do

- **Reservation Management** — List all reservations, retrieve detailed booking information, and monitor check-in schedules.
- **Listing Oversight** — Access details for all your property listings across platforms like Airbnb, Booking.com, and VRBO.
- **Guest Communication** — Search for guest profiles and retrieve communication history to ensure high-quality service.
- **Calendar & Pricing** — Check availability and pricing for specific dates and listings to optimize occupancy.
- **Operational Tasks** — Monitor cleaning and maintenance tasks to keep your properties in top condition.
- **Financial Reporting** — Retrieve owner statements, revenue data, and business accounting statistics.

### How it works

1. Subscribe to this server
2. Enter your Guesty Client ID and Client Secret
3. Start managing your rental business from Claude, Cursor, or any MCP-compatible client

No more manual exporting of booking data. Your AI assistant acts as a dedicated reservation manager or operations coordinator.

### Who is this for?

- **Property Managers** — instantly retrieve reservation details and listing statuses during busy check-in periods.
- **Operations Teams** — automate the process of checking task completion and calendar availability.
- **Short-term Rental Owners** — monitor revenue performance and guest satisfaction trends from a single interface.


## Available Tools
- **get_accounting_stats**: Retrieve business-level accounting summary and statistics
- **get_calendar**: Get availability and pricing calendar for a listing
- **get_listing_stats**: Retrieve performance statistics for a specific property listing
- **get_listing**: Get detailed information for a specific property listing
- **get_owner_revenue**: Returns owner statements: gross revenue, expenses, commissions, net payout
- **get_reservation**: Get details for a specific reservation
- **list_guests**: List guests or search by name/email
- **list_listings**: List all property listings managed in Guesty
- **list_messages**: List communication messages/chats. Optionally filter by guest ID
- **list_reservations**: List reservations. Filter by status (confirmed, stayed, cancelled)
- **list_tasks**: List cleaning and operational tasks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Guesty** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all confirmed reservations for next week."

**🤖 AI Agent:**
> I've retrieved your reservations. You have 8 confirmed bookings for next week, including 'Beachfront Villa' (ID: 7701) and 'City Loft' (ID: 7705). Would you like to see the guest details for any of these?

---

**👤 You:**
> "Check availability for listing ID 5520 from April 10th to 15th."

**🤖 AI Agent:**
> Checking calendar... Listing 5520 is AVAILABLE from April 10th to 15th. The average nightly rate for this period is $185.00. Should I check the guest history for this property?

---

**👤 You:**
> "Show me the accounting stats for this month."

**🤖 AI Agent:**
> Accessing accounting data... For this month, your gross revenue is $12,450.00 across 15 properties. Total commissions are $1,867.50 and net payout is $10,582.50. Would you like a breakdown by property?


## Installation & Usage

To install and use the **Guesty** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/guesty](https://vinkius.com/mcp/guesty)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# HQBeds MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hqbeds)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hqbeds-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hqbeds-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage hostel and accommodation bookings with channel distribution, guest communication, and occupancy tracking in one system.

## Description
Connect your **HQBeds** account to any AI agent and take full control of your property management system (PMS) and automated hostel/hotel operations through natural conversation.

### What you can do

- **Reservation Portfolio Orchestration** â€” List and manage all property reservations programmatically, retrieving detailed stay metadata and payment statuses
- **Guest & Customer Intelligence** â€” Programmatically retrieve directories of guests and access complete profiles and check-in history in real-time
- **Room & Inventory Architecture** â€” Access your complete directory of rooms and availability to coordinate your organizational resource allocation
- **Operational Monitoring** â€” Access real-time status updates for check-ins/outs and track property performance directly through your agent for instant reporting
- **Infrastructure Verification** â€” Verify account-level API connectivity and monitor booking volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Token** from your HQBeds dashboard (Settings > Integrations)
3. Start orchestrating your hospitality growth from Claude, Cursor, or any MCP client

No more manual checking of availability calendars or missing guest check-in times. Your AI acts as your dedicated front-desk coordinator and PMS architect.

### Who is this for?

- **Hostel & Hotel Managers** â€” instantly retrieve booking summaries and monitor occupancy using natural language commands
- **Reception Leads** â€” verify individual guest metadata and track payment history without leaving your creative workspace
- **Developers** â€” integrate high-speed HQBeds data into custom hospitality apps through simple AI queries


## Available Tools
- **check_hqbeds_status**: Verify HQBeds API connectivity
- **create_reservation**: Create a reservation
- **get_account**: Get account info
- **get_guest**: Get guest details
- **get_reservation**: Get reservation details
- **get_room**: Get room details
- **list_availability**: Use ISO 8601 dates.

Check room availability
- **list_guests**: List all guests
- **list_reservations**: List all reservations
- **list_rooms**: List all rooms


## 💬 Prompt Examples

Here are some examples of how you can interact with the **HQBeds** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all reservations checking in today."

**🤖 AI Agent:**
> You have 5 arrivals today. The first is John Smith in Room 101 (2 nights, paid). Would you like to see guest details or payment status for any of them?

---

**👤 You:**
> "Show room availability for this weekend."

**🤖 AI Agent:**
> This weekend you have 85% occupancy. 3 rooms are still available: Room 205 (double), Room 308 (single), and Room 412 (suite). Would you like to create a reservation?

---

**👤 You:**
> "Create a reservation for Maria Silva, Room 205, checking in May 10 and out May 12."

**🤖 AI Agent:**
> Done! Reservation created for Maria Silva in Room 205, May 10-12 (2 nights). Confirmation ID: RSV-4821. Would you like to send a confirmation email to the guest?


## Installation & Usage

To install and use the **HQBeds** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hqbeds](https://vinkius.com/mcp/hqbeds)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

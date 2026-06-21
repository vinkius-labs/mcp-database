# Preno MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/preno)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/preno-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/preno-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Run your hotel or accommodation with property management that handles bookings, channel distribution, and guest communication.

## Description
Connect your **Preno** account to any AI agent and take full control of your property management and high-fidelity hospitality orchestration through natural conversation.

### What you can do

- **Booking Portfolio Orchestration** — List all active and upcoming reservations, retrieve detailed high-fidelity status metadata, and monitor occupancy programmatically
- **Guest Intelligence Architecture** — Access complete high-fidelity guest profiles and stay history to personalize every interaction directly through your agent
- **Reservation Orchestration** — Programmatically generate new bookings and update existing high-fidelity reservation records for perfectly coordinated check-ins
- **Room & Rate Monitoring** — Access your complete directory of high-fidelity room types and rates to optimize property utilization and revenue management
- **Financial Transaction Discovery** — Access recorded technical payment entries to understand revenue streams and maintain perfect financial alignment
- **Operational Monitoring** — Verify account-level API connectivity and monitor booking orchestration volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Preno account (Settings > API Access)
3. Start managing your hospitality growth from Claude, Cursor, or any MCP client

No more manual occupancy checks or missing guest details. Your AI acts as your dedicated property coordinator and hospitality architect.

### Who is this for?

- **Hotel Managers** — instantly retrieve booking lists and guest profiles using natural language commands without leaving your creative workspace
- **Front Desk Leads** — trigger high-fidelity check-in preparations and monitor room availability to ensure healthy guest relations
- **Revenue Managers** — analyze high-fidelity rate metadata and payment logs to optimize pricing through simple AI queries


## Available Tools
- **list_preno_agents**: List OTAs and agents
- **list_preno_bookings**: List property bookings
- **create_preno_booking**: Create a new booking
- **create_preno_guest**: Create a new guest
- **get_preno_booking**: Get booking details
- **get_preno_guest**: Get guest details
- **get_preno_room_type**: Get room type details
- **list_preno_guests**: Optionally search by name or email.

List property guests
- **list_preno_payments**: List financial payments
- **list_preno_room_types**: List room categories
- **check_preno_status**: Check API Status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Preno** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active bookings and show their arrival status."

**🤖 AI Agent:**
> I've retrieved your bookings. You currently have 15 active high-fidelity reservations, including 'John Doe' (Checked In) and 'Sarah Smith' (Expected). Would you like to see the detailed guest metadata for any of them?

---

**👤 You:**
> "Create a new booking for guest 'John Doe' arriving tomorrow for 3 nights."

**🤖 AI Agent:**
> Reservation orchestrated! I've successfully generated a new high-fidelity booking for 'John Doe' (ID: res_456) for 3 nights. This record is now live in Preno. Shall I verify the available room technical types for assignment?

---

**👤 You:**
> "Check the last 5 payments recorded today."

**🤖 AI Agent:**
> Transaction directory orchestrated! I've identified 5 recent high-fidelity payment profiles, including one for 'Deluxe Suite' ($450). Your API connection is healthy. Shall I retrieve the detailed financial alignment metadata for today's transactions?


## Installation & Usage

To install and use the **Preno** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/preno](https://vinkius.com/mcp/preno)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

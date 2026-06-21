# SavvyCal MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/savvycal)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/savvycal-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/savvycal-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your SavvyCal scheduling links, check real-time availability, and coordinate automated bookings via AI.

## Description
Connect your **SavvyCal** account to any AI agent to streamline your meeting coordination. Let your AI agent act as your personal scheduling assistant without having to constantly switch tabs.

### What you can do

- **Scheduling Links** — View your active booking links, create new customized links dynamically, and manage URL slugs on the fly
- **Availability Constraints** — Query specific date ranges to find exactly when you are bookable across your various scheduling setups
- **Events Management** — List all upcoming scheduled meetings, get precise attendee details, and programmatically cancel appointments if needed
- **Account Settings** — Retrieve your base account profile and verify automated timezone settings

### How it works

1. Subscribe to this server
2. Enter your secure SavvyCal API Token
3. Start managing your calendar links from Claude, Cursor, or any MCP-compatible environment

Replace manual link juggling by having your agent fetch the right booking URL or calculate your free windows conversationally.

### Who is this for?

- **Founders & Executives** — ask your agent 'when am I free next week for a 45min chat?' and get the direct answer instantly
- **Sales & Consultants** — quickly generate a new, uniquely-named booking link for a specific client directly from your chat
- **Customer Success** — list upcoming client check-ins and cancel unconfirmed events with a single prompt


## Available Tools
- **cancel_event**: Specify the event ID and a cancellation reason.

Cancels a scheduled appointment
- **create_link**: Specify name, slug, and duration in minutes.

Creates a new scheduling link
- **delete_link**: This action is irreversible.

Permanently deletes a scheduling link
- **get_account**: Retrieves authenticated account information
- **get_event**: Retrieves details for a specific scheduled event
- **get_link**: Retrieves details for a specific scheduling link
- **list_availability**: Retrieves available time slots for a link within a date range
- **list_events**: Lists all scheduled booking events
- **list_links**: Lists all scheduling links in the SavvyCal account
- **update_link**: Updates an existing scheduling link


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SavvyCal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "When am I available next Wednesday for my 'Consultation' link?"

**🤖 AI Agent:**
> Looking at your 'Consultation' scheduling rules, next Wednesday you have bookable slots at 10:00 AM, 11:30 AM, and 2:00 PM (EST). Should I create a quick email snippet for you to send these options?

---

**👤 You:**
> "Create a new 30-minute link named Q3 Sync."

**🤖 AI Agent:**
> Done. I created the 30-minute link named 'Q3 Sync'. Your shareable URL slug is `q3-sync-abc12`. You can share `savvycal.com/your-username/q3-sync-abc12` immediately.

---

**👤 You:**
> "Who am I meeting with tomorrow?"

**🤖 AI Agent:**
> You have 2 events scheduled tomorrow via SavvyCal. 1. Product Onboarding with John Doe at 9 AM. 2. Interview with Jane Smith at 2 PM. I can provide their contact email or cancel either meeting if necessary.


## Installation & Usage

To install and use the **SavvyCal** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/savvycal](https://vinkius.com/mcp/savvycal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

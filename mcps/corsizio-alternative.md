# Corsizio MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/corsizio-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/corsizio-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/corsizio-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Sell event tickets and manage class registrations with a lightweight booking platform that handles payments and attendees.

## Description
Connect your **Corsizio** account to any AI agent and take full control of your event registration and participant engagement workflows through natural conversation.

### What you can do

- **Event Orchestration** — List and manage all active and past events programmatically, retrieving detailed metadata about schedules, locations, and pricing
- **Attendee Lifecycle** — Access complete participant profiles and registration details to maintain high-fidelity records of your event audience
- **Operational Intelligence** — Retrieve directories of instructors, locations, and categories to understand your event ecosystem directly through your agent
- **Feedback & Payout Tracking** — Access participant reviews and monitor account payouts programmatically to coordinate your event's financial and quality oversight
- **Activity Monitoring** — Retrieve account activity logs and manage discount coupons directly from your agent for perfectly coordinated event operations

### How it works

1. Subscribe to this server
2. Retrieve your **Secret API Key** from your Corsizio settings (Settings > API & Integrations)
3. Start managing your event registrations from Claude, Cursor, or any MCP client

No more manual scrubbing through attendee exports or complex navigation in the portal. Your AI acts as your dedicated event operations and participant coordinator.

### Who is this for?

- **Event Organizers** — instantly retrieve attendee counts and check event statuses using natural language commands
- **Course Instructors** — access participant details and feedback scores without leaving your communication tools
- **Business Administrators** — monitor payouts and manage discount coupons through simple AI queries


## Available Tools
- **get_account_info**: Get Corsizio account details
- **get_attendee_details**: Get details for a specific attendee
- **get_event_details**: Get details for a specific event
- **list_attendees**: List all event attendees
- **list_event_categories**: List all event categories
- **list_discount_coupons**: List all discount coupons
- **list_events**: Supports optional query parameters for filtering.

List all events
- **list_event_feedback**: List participant feedback
- **list_instructors**: List all instructors
- **list_event_locations**: List all event locations
- **list_activity_logs**: List account activity logs
- **list_payouts**: List account payouts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Corsizio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active events in my Corsizio account."

**🤖 AI Agent:**
> I've retrieved your active events. You currently have 3 sessions: 'AI Workshop 2026' (ID: ev_123), 'Design Sprint', and 'Coding Bootcamp'. Which one would you like the attendee list for?

---

**👤 You:**
> "Show the attendee details for event ID 'ev_123'."

**🤖 AI Agent:**
> Fetching attendee list... Event ev_123 has 15 participants registered, including 'John Doe' and 'Jane Smith'. I can provide individual profile metadata for any of them if needed.

---

**👤 You:**
> "Get the latest feedback for 'AI Workshop 2026'."

**🤖 AI Agent:**
> Scanning feedback... For 'AI Workshop 2026', I found 5 recent reviews with an average score of 4.8. Highlights include praise for the hands-on sessions. Would you like to see the detailed comments?


## Installation & Usage

To install and use the **Corsizio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/corsizio-alternative](https://vinkius.com/mcp/corsizio-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

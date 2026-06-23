# SuperSaaS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/supersaas)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate online scheduling and bookings via SuperSaaS — manage schedules, appointments, and users directly from any AI agent.

## Description
Connect your **SuperSaaS** account to any AI agent and simplify your online appointment scheduling, booking management, and user database through natural conversation.

### What you can do

- **Schedule Management** — List all online appointment schedules, retrieve detailed metadata and availability settings
- **Appointment Control** — Query bookings and appointments for any schedule, and retrieve detailed attendee info
- **Direct Execution** — Create new appointments and bookings programmatically directly from your agent with names and times
- **User Coordination** — List registered users and team members to understand your institution's occupancy
- **Account Tracking** — Access your real-time account balance and usage metrics directly from your agent

### How it works

1. Subscribe to this server
2. Enter your SuperSaaS Account Name and API Key from your account settings
3. Start managing your online bookings from Claude, Cursor, or any MCP-compatible client


## Available Tools (11)
- **delete_appointment**: Delete an appointment
- **get_schedule**: Get details for a specific schedule
- **get_user**: Get details for a specific user
- **list_changes**: List recent changes to a schedule
- **create_appointment**: Create a new booking
- **get_appointment_details**: Get details for a specific booking
- **get_account_balance**: Check account credit balance
- **list_appointments**: List appointments for a schedule
- **list_schedules**: List SuperSaaS schedules
- **list_account_users**: List registered users
- **update_appointment**: Update an existing appointment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SuperSaaS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active schedules in my SuperSaaS account."

**🤖 AI Agent:**
> I've retrieved your schedules. You have 3 active calendars, including 'Consultations' and 'Workshop Rooms'.

---

**👤 You:**
> "Show me all appointments for this week across all schedules with availability gaps."

**🤖 AI Agent:**
> 89 appointments this week across 4 schedules. "Consultation Room A" (34 bookings): Monday 92% booked, Tuesday 85%, Wednesday 78%, Thursday 90%, Friday 67%. Gaps: Wednesday 2-4 PM, Friday after 3 PM. "Training Room" (23 bookings): 3 full-day bookings, 4 half-day. "Equipment Rental" (18 reservations): excavator fully booked, crane available Thursday-Friday. "Virtual Meetings" (14 slots): 6 available slots remaining. Total revenue from bookings: $4,560. No-show rate: 3.4% (3 no-shows). Cancellations: 5 (4 rescheduled).

---

**👤 You:**
> "Create a recurring weekly appointment for team standup meetings every Monday at 9 AM."

**🤖 AI Agent:**
> Recurring appointment created. Name: "Team Standup". Schedule: Virtual Meetings. Day: every Monday at 9:00 AM. Duration: 30 minutes. Recurrence: weekly, no end date. Room: Virtual Meeting Room 1. Attendees: 8 team members notified. Calendar invites: sent via email and iCal. Reminders: 15 minutes before (push notification). Buffer: 10 minutes after. Conflict check: no conflicts detected for next 12 weeks. First occurrence: Monday, May 19 at 9:00 AM. Cancellation policy: 24-hour notice required.


## ❓ FAQ

**Q: Can I list all my appointments using my AI agent?**
Yes! Use the `list_appointments` tool and provide the Schedule ID. Your agent will retrieve all bookings for that specific calendar.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/supersaas](https://vinkius.com/mcp/supersaas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SuperSaaS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `supersaas` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SuperSaaS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "supersaas": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

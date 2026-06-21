# YouCanBook.me MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/youcanbookme)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate scheduling workflows via YouCanBook.me — manage booking pages, appointments, and availability directly from any AI agent.

## Description
Connect your **YouCanBook.me** account to any AI agent and take full control of your scheduling infrastructure through natural conversation.

### What you can do

- **Booking Page Management** — List all shareable scheduling pages (profiles) and retrieve detailed configurations including timezones and linked calendars
- **Appointment Monitoring** — List and query bookings across your profiles, filtered by status (tentative, upcoming, finished, cancelled)
- **Deep Booking Audit** — Retrieve full details for any specific appointment, including attendee info and custom form responses
- **Programmatic Booking** — Initiate the scheduling flow by creating booking intents and retrieving available time slots for user confirmation
- **Cancellation Control** — Instantly revoke appointments and automatically notify attendees through simple chat commands
- **Team Coordination** — List all staff members assigned to a booking page to see which technicians or consultants are available
- **Account Insights** — Verify your account standing, base timezone, and active calendar integrations directly from your agent

### How it works

1. Subscribe to this server
2. Enter your YouCanBook.me API Key and Account ID
3. Start managing your appointments through Claude, Cursor, or any MCP-compatible client

No more manual filtering through booking dashboards to find an attendee's email. Your AI agent becomes your personal scheduling coordinator.

### Who is this for?

- **Sales & Success Teams** — monitor upcoming customer calls and verify attendee information before meetings
- **Small Business Owners** — manage booking page availability and cancel appointments on the go via chat
- **Executive Assistants** — coordinate schedules across multiple profiles and team members without manual navigation
- **Product Teams** — implement programmatic booking flows and verify availability slots through simple conversation


## Available Tools
- **list_profiles**: Lists all booking pages (profiles) in the YouCanBook.me account
- **get_profile**: Retrieves detailed configuration for a specific booking page
- **list_bookings**: Status options: tentative, upcoming, finished, cancelled.

Queries bookings for a specific profile with optional status filtering
- **get_booking**: Retrieves full details for a specific YouCanBook.me booking
- **cancel_booking**: This action removes the calendar event and is irreversible.

Permanently cancels a booking and notifies the attendee
- **create_intent**: Provide the profile subdomain (e.g. "mycompany"). Returns an intent ID.

Creates a booking intent to initiate the programmatic scheduling process
- **get_availability**: Retrieves bookable time slots for an active booking intent
- **confirm_intent**: Finalizes a booking intent, creating the official appointment
- **get_account**: Retrieves details about the YouCanBook.me account and plan
- **list_team_members**: Lists all team members assigned to a specific booking page


## 💬 Prompt Examples

Here are some examples of how you can interact with the **YouCanBook.me** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my YouCanBook.me booking pages."

**🤖 AI Agent:**
> I found 3 booking pages: 1. 'Product Demo' (ID: prof-123), 2. 'Customer Support' (ID: prof-456), and 3. 'Recruitment Intro' (ID: prof-789). Which one would you like to see bookings for?

---

**👤 You:**
> "Show me upcoming bookings for the 'Product Demo' profile."

**🤖 AI Agent:**
> You have 2 upcoming bookings for 'Product Demo': 1. John Doe (2026-04-01 at 10:00 AM) and 2. Jane Smith (2026-04-02 at 02:00 PM). Would you like to see the full details for either of these?

---

**👤 You:**
> "Cancel the booking with ID 'book-999'."

**🤖 AI Agent:**
> Success! I've cancelled the booking 'book-999'. The attendee has been notified and the time slot is now open on your calendar again. Is there anything else you need to reschedule?


## ❓ FAQ

**Q: Can I cancel a specific booking and notify the attendee via chat?**
Yes. The `cancel_booking` tool allows your AI agent to permanently revoke an appointment using its booking ID. This action automatically removes the event from your calendar and sends a cancellation notice to the attendee.

**Q: How do I check my upcoming appointments for a specific booking page?**
Use the `list_bookings` tool. Provide the unique `profile_id` and set the status to 'upcoming'. Your agent will return a list of all confirmed future appointments for that scheduling page.

**Q: Is it possible to see which staff members are assigned to a booking profile?**
Absolutely. Using the `list_team_members` tool, you can retrieve a list of all staff members linked to a specific profile, showing you who is available to take appointments on that page.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/youcanbookme](https://vinkius.com/mcp/youcanbookme)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **YouCanBook.me** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `youcanbookme` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **YouCanBook.me** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "youcanbookme": {
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

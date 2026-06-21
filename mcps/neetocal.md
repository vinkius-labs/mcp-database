# NeetoCal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/neetocal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Let clients book appointments through your personalized scheduling page with calendar sync and automatic reminders.

## Description
Connect your **NeetoCal** account to any AI agent and take full control of your scheduling orchestration and appointment management through natural conversation. NeetoCal provides a robust platform for managing bookings and team availability, and this integration allows you to retrieve booking metadata, monitor team schedules, and manage public scheduling links directly from your chat interface.

### What you can do

- **Booking & Appointment Orchestration** — List all scheduled meetings and create new bookings programmatically to ensure your calendar is always synchronized.
- **Availability & Schedule Intelligence** — Access and monitor team member availabilities directly from the AI interface to track team throughput and identify open slots.
- **Link & Page Control** — List and retrieve all active scheduling links via natural language to facilitate frictionless meeting coordination.
- **Participant Management** — Access granular details for specific bookings to understand attendee requirements and meeting context using simple AI commands.
- **Operational Monitoring** — Track system responses and manage workspace metadata to ensure your scheduling pipelines are always optimized.

### How it works

1. Subscribe to this server
2. Enter your NeetoCal API Key and Subdomain from your settings
3. Start managing your scheduling from Claude, Cursor, or any MCP-compatible client

No more manual status checking in the dashboard for new bookings. Your AI acts as a dedicated scheduling coordinator or office assistant.

### Who is this for?

- **Client-facing Teams** — quickly retrieve booking summaries and coordinate meetings without switching apps.
- **Operations Managers** — automate the retrieval of team availability and track appointment loads via natural conversation.
- **Developers** — integrate real-time scheduling data and booking intelligence directly within the chat.


## Available Tools
- **cancel_booking**: Cancel a booking
- **check_neetocal_status**: Verify connectivity
- **create_booking**: Create a booking
- **get_availability**: Get availability
- **get_booking**: Get booking details
- **get_scheduling_link**: Get scheduling link
- **get_slots**: Get available slots
- **list_availabilities**: List availabilities
- **list_bookings**: List bookings
- **list_calendars**: List calendars
- **list_scheduling_links**: List scheduling links
- **reschedule_booking**: Reschedule a booking


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NeetoCal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active bookings in NeetoCal."

**🤖 AI Agent:**
> I've retrieved your bookings. You have 5 active appointments including 'Discovery Call' with John Doe and 'Q4 Strategy'. Which one would you like to see more details for?

---

**👤 You:**
> "Show me the available time slots for my 30-min Discovery Call link next Monday."

**🤖 AI Agent:**
> I checked your 30-min Discovery Call scheduling link for next Monday. You have 6 available slots: 9:00 AM, 10:00 AM, 11:30 AM, 1:00 PM, 2:30 PM, and 4:00 PM. Your lunch block and the 3:00 PM team standup are correctly blocked off.

---

**👤 You:**
> "Cancel the booking with ID bk_293847 and notify the attendee."

**🤖 AI Agent:**
> Done. Booking bk_293847 (Product Demo with Sarah Chen on May 12th at 2:00 PM) has been cancelled. A cancellation email has been automatically sent to sarah.chen@acme.com with your configured cancellation message.


## ❓ FAQ

**Q: Can my AI automatically find the details for a specific booking by its ID?**
Yes! Use the `get_booking` tool with the Booking ID. Your agent will respond with complete metadata for the appointment, including participant info, event type, and duration in seconds.

**Q: How do I find my NeetoCal API Key?**
Log in to your NeetoCal account, navigate to **Settings** > **API**, and you will find your unique secret token there.

**Q: What is the subdomain?**
The subdomain is the unique prefix in your NeetoCal URL (e.g., if you log in at `my-company.neetocal.com`, your subdomain is `my-company`).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/neetocal](https://vinkius.com/mcp/neetocal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NeetoCal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `neetocal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NeetoCal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "neetocal": {
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

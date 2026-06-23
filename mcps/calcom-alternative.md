# Cal.com MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/calcom-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Let anyone book time with you through customizable scheduling pages that sync with your calendar and eliminate back-and-forth.

## Description
Connect your **Cal.com** account to any AI agent and take full control of your professional scheduling infrastructure and meeting lifecycle through natural conversation.

### What you can do

- **Meeting Orchestration** — List and manage your meeting lifecycle programmatically, including creating new bookings and cancelling or rescheduling existing ones in real-time
- **Availability Intelligence** — Programmatically find free time slots for specific event types and date ranges to coordinate perfectly timed meetings
- **Template Management** — Access and monitor your complete directory of event types (templates) to ensure your high-fidelity scheduling options are always current
- **Rule & Schedule Monitoring** — Access your directory of availability schedules and working hours to oversee your time management programmatically
- **Operational Visibility** — Access high-fidelity metadata for your user profile and active webhooks directly through your agent for instant reporting

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Cal.com dashboard (Settings > Developer > API Keys)
3. Start managing your productivity schedule from Claude, Cursor, or any MCP client

No more manual toggling between calendars or sending back-and-forth availability emails. Your AI acts as your dedicated scheduling coordinator and time architect.

### Who is this for?

- **Busy Professionals** — instantly retrieve upcoming meetings and find free slots using natural language commands
- **Sales & Support Teams** — automate the scheduling of discovery calls and monitor event type performance without leaving your workspace
- **Executive Assistants** — orchestrate complex scheduling flows and manage user availability through simple AI queries


## Available Tools (12)
- **cancel_booking**: Remove meeting
- **create_new_booking**: Schedule a meeting
- **get_booking_details**: Get meeting info
- **get_event_type_details**: Get template info
- **get_my_profile**: Get user settings
- **get_available_slots**: Find free times
- **list_bookings**: List scheduled meetings
- **list_event_types**: List booking templates
- **list_availability_schedules**: List working hours
- **list_active_webhooks**: Get event configs
- **reschedule_meeting**: Update booking time
- **test_cal_auth**: Check connection


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cal.com** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my upcoming bookings for the next 7 days."

**🤖 AI Agent:**
> I've retrieved your schedule. You have 4 upcoming bookings, including a 'Strategy Session' tomorrow at 2 PM and 3 other meetings. Would you like the detailed attendee metadata for any of these?

---

**👤 You:**
> "Find available slots for a 'Discovery Call' tomorrow between 9 AM and 12 PM."

**🤖 AI Agent:**
> Scanning availability... I found 3 open slots for your 'Discovery Call' template: 9:30 AM, 10:30 AM, and 11:15 AM. Shall I book one of these for you?

---

**👤 You:**
> "Cancel my booking ID '12345' because of a conflict."

**🤖 AI Agent:**
> Booking cancelled! I've successfully removed meeting 12345 from your schedule. A notification has been sent to the attendees. Need help finding a new time slot?


## ❓ FAQ

**Q: How do I find my Cal.com API Key?**
Log in to your account, navigate to **Settings** > **Developer** > **API Keys**, and create a new key for your integration.

**Q: Can I check for available slots via AI?**
Yes! The `get_available_slots` tool allows your agent to find open times for specific event types and date ranges programmatically.

**Q: How do I reschedule a booking?**
Use the `reschedule_meeting` tool and provide the booking ID along with the new start and end times in JSON format.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calcom-alternative](https://vinkius.com/mcp/calcom-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cal.com** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `calcom-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cal.com** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "calcom-alternative": {
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

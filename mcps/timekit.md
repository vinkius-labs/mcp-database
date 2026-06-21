# Timekit MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/timekit)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Embed scheduling into your product with a white-label booking API that handles availability, time zones, and calendar sync.

## Description
Connect your **Timekit** account to any AI agent and simplify how you manage resource availability, booking workflows, and customer appointments through natural conversation.

### What you can do

- **Resource Management** — List all resources (people, rooms, equipment) and create new profiles to manage scheduling capacity.
- **Booking Lifecycle** — Create new bookings, confirm tentative requests, or decline/cancel existing appointments via AI.
- **Availability Checking** — Programmatically find available time slots for one or more resources based on specific date ranges and durations.
- **Rescheduling** — Easily move existing bookings to new time slots without manual dashboard entry.
- **Workflow Control** — Manage complex booking 'graphs' (instant, confirm_decline) directly from your workspace.
- **Account Visibility** — Retrieve detailed metadata for specific bookings and resources to stay on top of your schedule.

### How it works

1. Subscribe to this server
2. Enter your Timekit API Key (found in your developer settings)
3. Start managing your scheduling infrastructure from Claude, Cursor, or any MCP client

### Who is this for?

- **Service Providers** — quickly book client consultations and check availability via simple AI commands.
- **Office Managers** — manage room bookings and equipment scheduling across the organization directly from the workspace.
- **Product Teams** — automate the creation of resources and monitor booking flows via the AI assistant.


## Available Tools
- **cancel_booking**: Cancel a confirmed booking
- **check_availability**: Check availability for resources
- **confirm_booking**: Confirm a pending booking
- **create_booking**: Create a new booking
- **create_resource**: Create a new resource
- **decline_booking**: Decline a pending booking
- **get_booking**: Get details for a specific booking
- **get_resource**: Get details for a specific resource
- **list_bookings**: List all bookings
- **list_resources**: List all resources (people, rooms, etc.)
- **reschedule_booking**: Reschedule an existing booking


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Timekit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all resources available in my account."

**🤖 AI Agent:**
> I've retrieved your resources. You have: 'Main Office' (Room), 'Projector A' (Equipment), 'Alex Rivera' (Person), and 'Sarah Chen' (Person). Which one would you like to check availability for?

---

**👤 You:**
> "Find 30-minute slots for 'Alex Rivera' (ID: res_10293) for tomorrow afternoon."

**🤖 AI Agent:**
> I've checked Alex's availability. There are 3 available 30-minute slots tomorrow afternoon: 2:00 PM, 3:30 PM, and 4:00 PM UTC. Shall I book one of these for you?

---

**👤 You:**
> "Confirm the tentative booking #88231."

**🤖 AI Agent:**
> Success! I've confirmed booking 88231. The resource and the customer have been notified. Your schedule is now up-to-date.


## ❓ FAQ

**Q: Can I check availability for multiple resources at once?**
Yes! Use the `check_availability` tool and provide a JSON array of Resource IDs. The agent will return time slots where all specified resources are available.

**Q: How do I confirm a tentative booking request?**
Use the `confirm_booking` action and provide the unique Booking ID. This will transition the request from 'tentative' to 'confirmed' in your Timekit account.

**Q: Is it possible to reschedule an existing appointment via AI?**
Absolutely. Use the `reschedule_booking` tool. Provide the Booking ID and the new start and end times to update the appointment instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/timekit](https://vinkius.com/mcp/timekit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Timekit** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `timekit` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Timekit** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "timekit": {
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

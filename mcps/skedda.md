# Skedda MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/skedda)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [operations-management](../categories/operations-management.md)

Manage your workspace scheduling — create, update, and track bookings for desks, meeting rooms, and special venues directly through AI agents.

## Description
Connect your **Skedda** workspace to any AI agent to completely fully automate facility management and space scheduling. Handle your entire booking lifecycle through natural language conversations.

### What you can do

- **Space & Venue Discovery** — List all available physical spaces, venues, and their categorized groups (e.g., Office Hot Desks, Boardrooms)
- **Booking Operations** — Retrieve your current schedule, or instantly create, update, and delete reservations natively
- **User Management** — Look up fellow employees, customers, or members in the directory to assign them to bookings
- **Availability Tracking** — Filter your list of reservations by specific timeframes (ISO 8601) to identify empty slots

### How it works

1. Subscribe to this server
2. Provide your Skedda API Key from your venue settings
3. Start managing your workspace logistics straight from Claude, Cursor, or any MCP-compatible client

No more manually clicking through grid calendars to secure a hot desk for tomorrow or a boardroom for an upcoming client visit. Tell your AI pilot what you need, and it confirms the booking instantly.

### Who is this for?

- **Office Managers & Admins** — easily bulk-manage or delete bookings and quickly check occupancy levels without exporting data
- **Employees** — immediately reserve a meeting room on-the-go by chatting with your agent and assigning co-workers
- **Event Planners** — discover available spaces and categories to configure multi-day events efficiently


## Available Tools
- **create_booking**: Requires space ID, user ID, and start/end times.

Creates a new booking
- **delete_booking**: This action is irreversible.

Permanently deletes a booking
- **get_booking_details**: Retrieves details for a specific booking
- **list_bookings**: You can filter by date range.

Lists all bookings in Skedda
- **list_space_categories**: g., "Meeting Rooms", "Desks").

Lists space categories
- **list_spaces**: Lists all available spaces
- **list_users**: Lists all users in the Skedda account
- **list_venues**: Lists all venues
- **update_booking**: Updates an existing booking


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Skedda** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all meeting room zones and internal spaces we have available."

**🤖 AI Agent:**
> I've pulled the facility details. You currently have 4 spaces available:
1. Main Boardroom (ID: 151A, Category: Meeting Rooms)
2. Focus Pod 1 (ID: 21B, Category: Private Desks)
3. Hot Desk A (ID: 9X, Category: Open Floor)
4. Training Center (ID: 41C, Category: Event Venus)
Do you want me to list active bookings for any of these spaces?

---

**👤 You:**
> "Can you book 'Focus Pod 1' for tomorrow from 10:00 AM to 12:00 PM for user Marc Smith?"

**🤖 AI Agent:**
> Successfully booked Focus Pod 1 for tomorrow (10:00 AM - 12:00 PM UTC) for Marc Smith. 
Booking ID: `185011XX`.
Let me know if you need to adjust or update the allocated timeframe.

---

**👤 You:**
> "Cancel all bookings scheduled for the 'Training Center' on Friday."

**🤖 AI Agent:**
> I've checked the bookings for Friday at the Training Center. There were 2 active events: 
1 - 09:00 AM (Booking ID `88V1`)
2 - 02:00 PM (Booking ID `91B3`)
Both have been successfully deleted from the platform.


## ❓ FAQ

**Q: Can my AI automatically find an available room for tomorrow and book it?**
Yes. While your agent can list existing schedules across specific dates using ISO 8601 timeframes, it can dynamically cross-reference that with your list of available spaces. Once a gap is confirmed, the agent will prompt the booking creation tool linking your user ID to instantly reserve the room.

**Q: How will my AI know which space ID to book if I only know its name?**
You can simply mention the plain name (e.g., 'Book the Innovation Boardroom'). The agent will intelligently call the 'list_spaces' tool in the background first, match your requested string to the correct internal resource ID, and generate the final reservation seamlessly.

**Q: Can I bulk cancel multiple reservations if an event reschedules?**
Absolutely. You can request your AI to 'list all bookings for Monday', ask it to filter down to specific ones based on timeframe or assignee, and instruct it to execute a deletion for each matching reservation sequentially.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/skedda](https://vinkius.com/mcp/skedda)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Skedda** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `skedda` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Skedda** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "skedda": {
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

# SimplyBook.me MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/simplybookme)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Enable your AI agent to manage appointments, browse staff calendars, and handle client records via the SimplyBook.me scheduling platform.

## Description
Connect your AI to **SimplyBook.me**, the online appointment scheduling platform for service-based businesses.

### What you can do

- **Booking Management** — Create, update, and cancel appointments directly from chat using `create_booking`, `update_booking`, and `cancel_booking`.
- **Calendar Browsing** — View staff work calendars and available time slots with `get_work_calendar`.
- **Client Records** — List and inspect client profiles to check booking history and contact details.
- **Service Catalog** — Browse all services and events offered by the company, including pricing and duration.

### How it works

1. Add the SimplyBook.me integration to your AI toolset.
2. Provide your API Key, API Secret, and Company Login.
3. Manage your booking operations via natural language.

### Who is this for?

- **Salon & Spa Owners** — Schedule client appointments and check staff availability from chat.
- **Clinic Administrators** — Monitor upcoming consultations and manage patient bookings without opening the dashboard.
- **Service Teams** — Track group classes, events, and provider calendars in real time.


## Available Tools (10)
- **create_booking**: Requires service ID, unit ID, and start time.

Creates a new booking
- **cancel_booking**: This action is irreversible.

Cancels a scheduled booking
- **update_booking**: Updates an existing booking
- **get_booking_details**: Retrieves details for a specific booking
- **get_work_calendar**: Retrieves the work calendar for a unit
- **list_bookings**: Lists all scheduled bookings
- **list_clients**: Lists company clients
- **list_events**: Lists specific calendar events or classes
- **list_services**: Lists all available services offered by the company
- **list_units**: Lists all service units (providers or locations)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SimplyBook.me** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available services offered by my company."

**🤖 AI Agent:**
> Here are the 5 services currently offered:
1. Haircut (30 min) — $25
2. Full Color (90 min) — $120
3. Manicure (45 min) — $35
4. Facial Treatment (60 min) — $80
5. Consultation (15 min) — Free

Would you like to book an appointment for any of these?

---

**👤 You:**
> "Show me all bookings for next week."

**🤖 AI Agent:**
> Found 8 bookings for April 7–11:
- Mon 10:00 — Maria S. (Haircut)
- Mon 14:30 — João P. (Full Color)
- Tue 09:00 — Ana L. (Facial Treatment)
- Wed 11:00 — Carlos M. (Consultation)
- Thu 15:00 — Laura R. (Manicure)
- Fri 10:00 — Pedro G. (Haircut)
- Fri 13:00 — Sofia T. (Full Color)
- Fri 16:00 — Diego A. (Facial Treatment)

Would you like details on any specific booking?


## ❓ FAQ

**Q: Can the AI accidentally delete all my bookings?**
No. The cancel_booking tool only cancels a single specific booking by its ID. It cannot perform bulk deletions or affect account settings. Each cancellation requires an explicit booking ID.

**Q: How does authentication work?**
You provide your API Key, API Secret, and Company Login. The integration automatically exchanges them for a session token (X-Token) on each request — no manual OAuth setup required.

**Q: Can the AI create new bookings or only manage existing ones?**
The AI can both create new bookings and manage existing ones. Use create_booking to schedule appointments and cancel_booking to cancel specific reservations by their ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/simplybookme](https://vinkius.com/mcp/simplybookme)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SimplyBook.me** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `simplybookme` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SimplyBook.me** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "simplybookme": {
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

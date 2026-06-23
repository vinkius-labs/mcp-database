# Picktime MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/picktime)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Equip your AI agent to manage scheduling operations. Fetch global availabilities, list locations, and manage business bookings via chat natively.

## Description
Connect your **Picktime** organization account to your AI agent and turn complex scheduling and availability management into a simple chat conversation.

### What you can do

- **Space & Resources** — Easily retrieve structural logistics utilizing `list_locations` and inspect the service portfolio actively using `list_services`.
- **Staff Management** — Gather team rosters through `list_staff` to orchestrate proper assignment mappings for upcoming reservations.
- **Booking Operations** — Execute deep audits with `list_bookings`, review detailed entries (`get_booking_details`), and cleanly back out utilizing `cancel_booking`.
- **Availability Mapping** — Audit live calendar empty spots using `get_availability` or check structured slots via `list_classes` for seamless planning.

### How it works

1. Subscribe to this server
2. Enter your Enterprise Picktime API Key
3. Start fetching availability windows or querying the status of corporate locations natively through Claude, Cursor, or any configured AI

### Who is this for?

- **Client Relations & Receptionists** — check if the stylist or doctor is free this afternoon without clicking through the calendar interface.
- **Business Directors** — extract all reservations of the day into a bulleted list to organize daily briefings and forecast team loads.
- **Tech Teams** — test availability integrations structurally from your terminal building enterprise webhook handlers.


## Available Tools (10)
- **list_locations**: List all business locations configured in Picktime. Each location operates independently with its own services, staff, working hours, and booking pages. Multi-location businesses manage branches separately
- **get_location**: Used to resolve workspace boundaries before hitting schedules.

Get detailed configuration for a specific Picktime location by ID. Returns location name, address, timezone, working hours, booking URL, and linked calendar/payment integrations
- **list_services**: List all bookable services for a Picktime location. Returns service names, durations, prices, descriptions, assigned staff, and buffer times. Services define what customers can book
- **get_service_details**: Get detailed configuration for a specific Picktime service. Returns name, duration, price, description, staff assignments, booking limits, and cancellation policy
- **list_staff**: List all staff members at a Picktime location. Returns staff names, emails, roles, assigned services, working hours, and active status. Staff availability determines bookable time slots
- **list_bookings**: List all bookings for a Picktime location with optional date filter. Returns customer names, booked services, staff assignments, times, statuses, and payment info. Essential for schedule management
- **get_booking_details**: Get full details of a specific Picktime booking including customer contact info, service booked, staff assigned, start/end times, payment status, and any customer notes
- **cancel_booking**: Cancel a Picktime booking with a reason. The customer receives a cancellation notification and the time slot becomes available again for new bookings
- **list_classes**: List all group classes configured for a Picktime location. Classes are multi-attendee bookings with capacity limits — yoga sessions, workshops, group trainings
- **get_availability**: Get available booking time slots for a specific Picktime service on a given date. Returns free windows considering staff schedules, existing bookings, and buffer times. Essential for building custom booking flows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Picktime** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all of our active clinic locations in the Picktime registry."

**🤖 AI Agent:**
> Based on the MCP query, you have 3 configured locations. The primary location is 'Central Manhattan Office' with the designated ID location_12345.

---

**👤 You:**
> "Cancel the booking record identified as BK123456."

**🤖 AI Agent:**
> Confirmed. I executed `cancel_booking` using ID BK123456. The status is now nullified and the slot returned to the public pool.

---

**👤 You:**
> "Can you check the availability data for 'Hair Styling' next Monday?"

**🤖 AI Agent:**
> I queried `get_availability`. There are plenty of openings next Monday for 'Hair Styling', notably 10:00 AM, 11:30 AM, and 2:00 PM.


## ❓ FAQ

**Q: Can the AI find an available slot for a specific service next Friday?**
Yes. Upon providing the location and service ID along with the desired date, your agent invokes `get_availability`. The connector reads Picktime's master block array, isolating the open time windows seamlessly against existing rules (like business hours and buffers).

**Q: If a customer cancels on the phone, can the AI remove their booking?**
Absolutely. Just provide the booking ID to the agent and it will utilize the `cancel_booking` function. Picktime will release the blocked slot immediately back to the customer-facing booking page.

**Q: Can I grab all upcoming appointments for a specific staff member?**
Yes, by matching the staff member's ID from `list_staff` with the broader fetch generated by `list_bookings`. Alternatively, your agent can sort and filter the returned array natively in its reasoning stream, showing you only Dr. Silva's schedule.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/picktime](https://vinkius.com/mcp/picktime)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Picktime** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `picktime` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Picktime** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "picktime": {
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

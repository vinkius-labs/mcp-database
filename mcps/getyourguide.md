# GetYourGuide MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/getyourguide)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Search and book tours, activities, and travel experiences via AI agents with GetYourGuide.

## Description
Connect your AI agent to the **GetYourGuide** global marketplace to automate travel activity discovery and booking through the Model Context Protocol (MCP). GetYourGuide is the leading platform for finding and booking unforgettable travel experiences, from guided tours to skip-the-line tickets. This MCP server enables you to search for activities in any destination, check real-time availability, and manage travel bookings directly through natural conversation.

### Key Features

- **Activity Discovery** — Search for tours and experiences by keyword, location, or coordinates, and fetch detailed metadata for each activity.
- **Real-time Availability** — Check open time slots and vacancies for specific tours to find the perfect time for your trip.
- **Travel Booking** — Programmatically create new bookings for activities and retrieve confirmation details instantly.
- **Booking Management** — Fetch the status of existing reservations or cancel confirmed bookings using their unique hash.
- **Shopping Cart Tracking** — List and retrieve detailed information for active or pending shopping carts.
- **Global Destinations** — List supported cities and destinations to discover the best activities GetYourGuide has to offer globally.
- **Partner Insights** — Access metadata for the authenticated partner account to verify connectivity and settings.
- **Real-time Synchronization** — Keep your travel operations accessible to your AI assistant without leaving your primary workspace.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your GetYourGuide Partner Access Token (found in the Integrator Portal)
3. Start managing your travel activities from Claude, Cursor, or any MCP client

### Who is this for?

- **Travel Agencies & Distributors** — quickly check activity availability or manage client bookings without manual portal navigation.
- **Travel Concierges** — get a real-time overview of the best activities in any destination via simple AI commands.
- **Logistics Ops** — automate the retrieval of tour details and booking statuses for travel itineraries.


## Available Tools (12)
- **get_booking_status**: Check booking details
- **get_cart_details**: Get cart metadata
- **check_activity_availability**: Check open slots
- **get_activity_details**: Get tour metadata
- **list_active_carts**: List shopping carts
- **list_travel_destinations**: List supported cities
- **search_by_destination**: Filter by city
- **search_travel_activities**: Search tours/activities
- **cancel_travel_booking**: Cancel a booking
- **verify_api_connection**: Check connection
- **create_travel_booking**: Book an activity
- **get_partner_details**: Get account identity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GetYourGuide** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for guided tours of the Eiffel Tower in Paris."

**🤖 AI Agent:**
> Searching activities... I found several options for the Eiffel Tower, including 'Priority Access Tour' (ID: 123) and 'Summit Guided Tour'. Which one would you like to check availability for?

---

**👤 You:**
> "Is the 'Louvre Museum Skip-the-Line Ticket' available for October 10th?"

**🤖 AI Agent:**
> Checking availability... Yes, there are 15 slots available for October 10th at various times starting from 09:00 AM. Prices start at $22.00.

---

**👤 You:**
> "Show me the status of my booking 'GYG-ABC-123-XYZ'."

**🤖 AI Agent:**
> Fetching booking... Your reservation for the 'Venice Gondola Ride' is 'Confirmed'. The meeting point is San Marco Square at 10:30 AM tomorrow. Would you like the meeting point coordinates?


## ❓ FAQ

**Q: How do I get an Access Token for GetYourGuide?**
You must register as a Partner or Distributor. Once approved, you can find your Access Token in the GetYourGuide Integrator Portal.

**Q: Can I search for activities using coordinates?**
Yes! The 'search_travel_activities' tool accepts location strings which can include latitude/longitude coordinates to find tours near a specific point.

**Q: How do I check if a tour is available on a specific date?**
Use the 'check_activity_availability' tool. Provide the Tour ID and an ISO date (YYYY-MM-DD) to see all open slots and vacancies for that day.

**Q: What is a 'Booking Hash'?**
The Booking Hash is a unique alphanumeric identifier for a reservation. You need it to retrieve booking details or to cancel a reservation via the agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/getyourguide](https://vinkius.com/mcp/getyourguide)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GetYourGuide** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `getyourguide` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GetYourGuide** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "getyourguide": {
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

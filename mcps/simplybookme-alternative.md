# SimplyBook.me MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/simplybookme-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage services, providers, and bookings on SimplyBook.me with AI agents.

## Description
Connect your **SimplyBook.me** account to any AI agent to automate your online booking system and resource orchestration. SimplyBook.me provides a powerful platform for managing appointment schedules, and this integration allows you to browse service lists, check provider availability, and handle full booking lifecycles through natural conversation.

### What you can do

- **Resource & Service Orchestration** — List all managed services, categories, and providers to maintain a clear overview of your booking assets programmatically.
- **Availability Intelligence** — Check real-time availability for specific services and providers to find the perfect appointment slot via natural language.
- **Booking Lifecycle Management** — Create, retrieve, and monitor bookings directly from the AI interface to ensure your schedule is always synchronized.
- **Client Management** — Access and monitor your client database to keep respondent metadata updated during the booking process.
- **Operational Monitoring** — Track appointment statuses and monitor provider assignments using simple AI commands.

### How it works

1. Subscribe to this server
2. Enter your SimplyBook.me Company Login and User API Token
3. Start managing your appointment schedules from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Service Business Owners** — quickly check upcoming appointments and provider schedules without switching apps.
- **Operations Managers** — automate the process of checking real-time availability and managing client data via natural conversation.
- **Customer Success Teams** — streamline the retrieval of booking details and coordinate service assignments directly within the chat.


## Available Tools (11)
- **cancel_booking**: Cancel an existing booking
- **get_client**: Get details for a specific client
- **list_promotions**: List all active promotions and discounts
- **create_booking**: Create a new appointment
- **check_availability**: Check available time slots
- **get_booking_details**: Get details for a specific booking
- **list_all_bookings**: List recent appointments
- **list_categories**: List service categories
- **list_clients**: me account.

List registered clients
- **list_providers**: List service providers (staff)
- **list_services**: List all bookable services


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SimplyBook.me** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all available services in my SimplyBook.me account."

**🤖 AI Agent:**
> I've retrieved your services. You have 5 active offerings including 'Consultation', 'Training Session', and 'Support Call'. Which one would you like to check availability for?

---

**👤 You:**
> "Show me all bookings for this week with available time slots and staff schedules."

**🤖 AI Agent:**
> 78 bookings this week across 5 services. Monday: 18 bookings (92% capacity). Tuesday: 16 (85% capacity). Wednesday: 14 (74%). Thursday: 15 (79%). Friday: 12 (63%). Saturday: 3 (25%). "Consultation" leads with 28 bookings (avg duration: 45 min). "Haircut" has 22. "Massage" has 15. "Facial" has 8. "Manicure" has 5. Available slots today: 6 (2 PM, 2:30, 3 PM, 3:30, 4 PM, 4:30). Staff: Sarah booked 89%, James 76%, Lisa 92% (highest utilization). No-show rate: 4.2%.

---

**👤 You:**
> "Book a 60-minute consultation appointment for a new client next Thursday at 2 PM."

**🤖 AI Agent:**
> Booking confirmed. Service: Consultation (60 min). Date: Thursday, May 22, 2025 at 2:00 PM. Provider: Lisa (specialist, highest rated). Client: New client profile created. Confirmation email sent to client with booking details, location map, and cancellation policy. Reminder SMS scheduled: 24 hours before and 2 hours before. Google Calendar sync: event created. Buffer time: 15 min after appointment. Payment: deposit of $25 charged, remaining $75 due at appointment.


## ❓ FAQ

**Q: How do I find my SimplyBook.me User API Token?**
Log in to your SimplyBook.me admin panel, enable the **API Custom Feature**, and navigate to **Settings** under that feature to find your User API Key.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/simplybookme-alternative](https://vinkius.com/mcp/simplybookme-alternative)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `simplybookme-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SimplyBook.me** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "simplybookme-alternative": {
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

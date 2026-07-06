# Zoho Bookings MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-bookings)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate appointment scheduling via Zoho Bookings — manage appointments, services, and staff with AI.

## Description
Connect your **Zoho Bookings** account to any AI agent to streamline your appointment management through natural conversation. Zoho Bookings provides a comprehensive platform for scheduling and managing services, staff availability, and workspaces.

### What you can do

- **Appointment Management** — List all booked appointments and handle new bookings or cancellations directly from your AI agent.
- **Service Catalog** — Retrieve your complete list of services and appointment types to build dynamic booking flows.
- **Staff Coordination** — List staff members and fetch their available time slots for any specific date to ensure efficient scheduling.
- **Workspace Organization** — Manage multiple workspaces and their associated booking settings programmatically.
- **Real-time Availability** — Get instant data on staff slots to avoid conflicts and optimize your team's calendar.

### How it works

1. Subscribe to this server
2. Enter your Zoho Authtoken (API Key) from your account settings
3. Start managing your appointments from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Service Providers** — automate your scheduling and manage staff availability more efficiently.
- **Receptionists & VAs** — quickly check and book appointments for clients using natural language.
- **Business Owners** — get a real-time overview of services and bookings across all business locations.


## Available Tools (7)
- **list_services**: List all services offered
- **list_staff**: List all staff members
- **list_workspaces**: List all workspaces
- **book_appointment**: Pass booking data as a JSON string.

Book a new appointment
- **cancel_appointment**: Cancel an existing appointment
- **get_staff_slots**: Get available slots for a staff member
- **list_appointments**: List all booked appointments


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho Bookings** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my upcoming appointments and check the available slots for Dr. Smith on May 15th."

**🤖 AI Agent:**
> You have 3 upcoming appointments this week. For Dr. Smith (Staff ID: 8901), there are 4 available slots on May 15th: 09:00 AM, 11:30 AM, 02:00 PM, and 04:30 PM. Would you like to book one of these slots?

---

**👤 You:**
> "Cancel my existing appointment with ID 'AP-2045' and book a new 'Technical Audit' session for tomorrow at 10 AM."

**🤖 AI Agent:**
> I have successfully canceled appointment AP-2045. A new 'Technical Audit' session has been booked for tomorrow at 10:00 AM. Your confirmation number is AP-2099.

---

**👤 You:**
> "Retrieve the full list of services we offer in the 'Downtown Clinic' workspace."

**🤖 AI Agent:**
> In the 'Downtown Clinic' workspace, you currently offer 5 services: 'General Consultation' (30 mins), 'Specialist Review' (60 mins), 'Follow-up' (15 mins), 'Annual Checkup' (45 mins), and 'Vaccination' (10 mins).


## ❓ FAQ

**Q: How do I find my Zoho Bookings Authtoken?**
Log in to your Zoho Bookings account, navigate to the API section in your settings, or use the Zoho Accounts portal to generate a permanent authtoken for API access.

**Q: Can the AI agent check staff availability for a specific day?**
Yes! Use the `get_staff_slots` tool with the Staff ID, Service ID, and the target Date to see all available time slots for that day.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-bookings](https://vinkius.com/mcp/zoho-bookings)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Zoho Bookings** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `zoho-bookings` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Zoho Bookings** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "zoho-bookings": {
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

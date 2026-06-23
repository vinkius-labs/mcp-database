# MakePlans MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/makeplans)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage appointments, services, and customers via the MakePlans REST API.

## Description
Connect your **MakePlans** account to any AI agent to automate your scheduling and appointment management. This MCP server enables your agent to list bookings, find available time slots, manage services and resources, and create customer records directly from natural language interfaces.

### What you can do

- **Appointment Control** — List all scheduled bookings and retrieve detailed metadata and status updates
- **Availability Check** — Query specific services to find available time slots within defined date ranges
- **Resource Oversight** — Manage bookable resources such as staff members, rooms, or specialized equipment
- **Service Catalog** — List all service definitions and appointment types configured in your account
- **Customer CRM** — Create new customer profiles and manage the 'people' database for your business
- **Real-time Scheduling** — Programmatically create new appointments by linking people, services, and time slots

### How it works

1. Subscribe to this server
2. Enter your MakePlans API Key and your Account Name (subdomain)
3. Start managing your calendar from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Service-Based Businesses** — Monitor your appointment calendar and manage availability via simple natural language commands
- **Operations Teams** — Quickly retrieve customer booking histories and update resource assignments without opening the portal
- **Developers** — Integrate scheduling logic and slot availability into your custom internal dashboards


## Available Tools (8)
- **list_appointments**: Use optional params for filtering.

List all bookings/appointments
- **create_new_appointment**: Requires person_id, service_id, and start_at.

Schedule a new booking
- **create_new_customer**: Requires name.

Add a new customer profile
- **get_appointment_details**: Get details for a specific booking
- **list_customers**: List all registered customers
- **list_booking_resources**: List booking resources (staff, rooms, etc.)
- **list_available_services**: List all offered services (appointment types)
- **find_available_slots**: Requires service_id and date parameters.

Find available time slots for a service


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MakePlans** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all appointments scheduled for next week in MakePlans."

**🤖 AI Agent:**
> I've retrieved your bookings for next week. You have 8 appointments scheduled, including 'Consultation with John Smith' and 'Yoga Class'. Would you like the full details for any of them?

---

**👤 You:**
> "Find available slots for service ID '123' between tomorrow and Friday."

**🤖 AI Agent:**
> I've checked the availability for service 123. There are 5 open slots available tomorrow morning and 3 slots available on Thursday afternoon.

---

**👤 You:**
> "Create a new customer profile for 'Alice Doe' with email 'alice@example.com'."

**🤖 AI Agent:**
> Successfully created the profile for Alice Doe in MakePlans. The new person ID is 'pers-987'. You can now use this ID to schedule bookings for her.


## ❓ FAQ

**Q: How do I find my MakePlans API Key?**
Log in to your MakePlans admin dashboard, navigate to Settings > API to find or generate your Private API Key. Your token is encrypted at rest and injected securely at runtime.

**Q: What is the Account Name?**
The account name is the subdomain used in your MakePlans URL, for example: `mycompany.makeplans.com`. Enter only `mycompany`.

**Q: Can I search for available slots for a specific date range?**
Yes, use the `find_available_slots` tool and provide `params` such as `from=2024-01-01&to=2024-01-07` along with the service ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/makeplans](https://vinkius.com/mcp/makeplans)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MakePlans** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `makeplans` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MakePlans** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "makeplans": {
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

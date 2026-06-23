# Vagaro MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vagaro)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage appointments, clients, staff, services, and retail for your Vagaro-powered salon, spa, or fitness business through natural conversation.

## Description
Connect your **Vagaro** business to any AI agent and manage your salon, spa, or fitness studio through natural conversation.

### What you can do

- **Appointments** — View booked appointments, check availability, and manage daily schedule
- **Clients** — Search customers, view profiles, visit history, and preferences
- **Staff** — List providers, check individual schedules, and manage availability
- **Services** — Browse all services offered with pricing and duration
- **Classes** — View group fitness classes, capacity, and enrollment
- **Products** — Manage retail inventory: hair care, skincare, supplements
- **Business** — Access business profile, hours, and online booking settings

### Who is this for?

- **Salon Owners** — Instant access to daily bookings, revenue, and client insights
- **Spa Managers** — Track therapist schedules and service utilization
- **Fitness Studios** — Monitor class enrollment and member engagement
- **Front Desk** — Quick client lookup, appointment details, and scheduling assistance


## Available Tools (10)
- **list_appointments**: Filter by date to see a specific day.

List salon/spa/fitness appointments
- **get_business_info**: Get business profile
- **get_appointment**: Get appointment details
- **search_clients**: Returns contact info, visit history, and preferences.

Search clients/customers
- **get_client**: Get client profile
- **list_services**: Includes pricing, duration, and category.

List all services offered
- **list_staff**: Includes name, role, specialties, and availability.

List all staff/providers
- **get_staff_schedule**: Shows booked and available time slots.

Get staff member schedule
- **list_classes**: Includes schedule, instructor, capacity, and enrolled count.

List fitness/wellness classes
- **list_products**: Includes name, price, brand, and stock level.

List retail products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vagaro** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me today's appointments."

**🤖 AI Agent:**
> Today's schedule:

9:00 AM — **Jessica R.** Balayage + Cut with Sarah ($185)
10:30 AM — **Mark T.** Men's Haircut with Mike ($35)
11:00 AM — **Amanda L.** Deep Tissue Massage with Ana ($120)
1:00 PM — **Sarah K.** Gel Manicure + Pedicure with Lisa ($75)

4 appointments, $415 projected revenue. You have a 2-hour gap from 2:00-4:00 PM.

---

**👤 You:**
> "Find Elena Gomez's profile and check her last booked service."

**🤖 AI Agent:**
> Accessing Vagaro client records ('get_client_details')...
Elena Gomez (ID: 8841-A):
- Status: Active VIP
- Last Service: 'Signature Facial' on Oct 5th
- Preferred Staff: Anna M.
- Notes: Allergic to lavender extract.

---

**👤 You:**
> "Book a 60-minute deep tissue massage for Mark Smith with John next Friday at 2 PM."

**🤖 AI Agent:**
> Executing `create_appointment` action...
Appointment confirmed!
- Client: Mark Smith
- Service: Deep Tissue Massage (60 min)
- Staff: John
- Date: Next Friday, 2:00 PM
- Price: $110.00
A confirmation SMS has been sent to the client.


## ❓ FAQ

**Q: How do I get Vagaro API access?**
Go to your Vagaro dashboard → Settings → Developer Features → API Settings. You'll need Admin or Owner permissions and active payment processing to generate API credentials.

**Q: Does it support multi-location businesses?**
Yes. Each location has its own Business ID. Configure the server with the specific Business ID for the location you want to manage, or set up multiple instances for multi-location oversight.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vagaro](https://vinkius.com/mcp/vagaro)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vagaro** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vagaro` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vagaro** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vagaro": {
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

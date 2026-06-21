# Acuity Scheduling MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/acuity-scheduling-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Acuity appointments and calendars — audit availability and bookings via AI.

## Description
Empower your AI agent to orchestrate your entire scheduling ecosystem with **Acuity Scheduling**, the online appointment scheduling software. By connecting Acuity to your agent, you transform complex calendar management into a natural conversation. Your agent can instantly list upcoming appointments, audit availability for specific types, and manage client bookings without you ever touching a dashboard. Whether you are a solo practitioner or managing a large team, your agent acts as a real-time scheduling coordinator, ensuring your time is always efficiently allocated.

### What you can do

- **Appointment Auditing** — List all upcoming and historical appointments, and retrieve detailed metadata for each client booking.
- **Availability Management** — Query real-time availability for specific appointment types and calendars instantly.
- **Booking Lifecycle** — Create, reschedule, and cancel appointments through natural language to keep your schedule accurate.
- **Resource Oversight** — List all your calendars, appointment types, and categories to maintain a structured service offering.
- **Account Auditing** — Quickly retrieve account-wide information to maintain strict organizational control.

### How it works

1. Subscribe to this server
2. Enter your Acuity User ID and API Key
3. Start managing your schedule through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Service Providers** — monitor your daily schedule and client details straight from your workflow.
- **Operations Managers** — verify if appointment slots are being correctly booked and managed by the team.
- **Customer Support** — perform rapid appointment audits and reschedule client meetings without manual dashboard logins.
- **Business Owners** — automate availability querying to orchestrate your time-driven growth smoothly.


## Available Tools
- **cancel_appointment**: Cancel an appointment
- **create_appointment**: Create a new appointment
- **get_appointment**: Get details for a specific appointment
- **get_availability**: Check available times
- **get_me**: Get Acuity account details
- **list_appointment_types**: List available appointment types
- **list_appointments**: List Acuity appointments
- **list_calendars**: List all calendars
- **list_categories**: List appointment categories
- **reschedule_appointment**: Reschedule an appointment


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Acuity Scheduling** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show my upcoming appointments for this week."

**🤖 AI Agent:**
> I've retrieved your schedule. You have 3 appointments this week, including a 'Strategy Session' with John Doe on Wednesday. Would you like the details for any of them?

---

**👤 You:**
> "Check if there are any slots for 'New Patient Consultation' tomorrow."

**🤖 AI Agent:**
> Checking tomorrow's availability... I've found 2 available slots for that consultation: 10:00 AM and 14:30 PM. Would you like me to book one for you?

---

**👤 You:**
> "Cancel my appointment with ID 987654321."

**🤖 AI Agent:**
> I've successfully cancelled appointment 987654321. I've also verified that the slot is now back in your availability for other clients.


## ❓ FAQ

**Q: Where do I find my Acuity User ID and API Key?**
Log in to your Acuity Scheduling account, go to **Settings** > **Integrations** > **API**, and you will find both there. Copy and paste them into the fields below.

**Q: Can the agent check real-time availability?**
Yes. Use the `get_availability` tool providing the Appointment Type ID and the target month. Your agent will return all open slots instantly.

**Q: Is it possible to reschedule an existing appointment?**
Yes. The `reschedule_appointment` tool allows your agent to move an existing booking to a new datetime using the original Appointment ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/acuity-scheduling-alternative](https://vinkius.com/mcp/acuity-scheduling-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Acuity Scheduling** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `acuity-scheduling-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Acuity Scheduling** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "acuity-scheduling-alternative": {
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

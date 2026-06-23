# Phorest MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/phorest-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Manage salon and spa operations—clients, appointments, and staff schedules—directly through your AI agent.

## Description
Connect your **Phorest** account to any AI agent to streamline your salon or spa management. Take full control of your business operations through natural conversation.

### What you can do

- **Client Management** — List, create, and update client records including contact details and course history.
- **Appointment Control** — List branch appointments, get specific details, update bookings, and perform client check-ins.
- **Staff & Timetables** — Retrieve branch or staff-specific timetables and manage staff breaks efficiently.
- **Course Tracking** — Monitor and update client courses and treatment packages.
- **Data Export** — Generate and retrieve CSV export jobs for business reporting and analysis.

### How it works

1. Subscribe to this server
2. Enter your Phorest API credentials (Username and Password)
3. Start managing your salon operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Salon Owners** — quickly check daily schedules and client check-in statuses without opening the Phorest desktop app.
- **Receptionists** — update client details and manage appointments via voice or quick text commands.
- **Business Analysts** — trigger CSV exports and gather staff performance data for reporting.


## Available Tools (17)
- **checkin_appointment**: Check-in a client for an appointment
- **confirm_appointments**: Confirm one or more appointments
- **create_break**: Create a staff break
- **create_client**: Create a new client
- **create_csv_export_job**: Create a CSV export job
- **get_appointment**: Get specific appointment details
- **get_branch_timetable**: Get the branch work timetable
- **get_client_course**: Get details of a specific client course
- **get_csv_export_job**: Retrieve the status and download URL of a CSV export job
- **get_staff_timetable**: Get timetables for all staff in a branch
- **list_appointments**: List appointments for a branch
- **list_breaks**: List staff breaks
- **list_client_courses**: List client courses (packages)
- **list_clients**: List clients for a business
- **update_appointment**: Update an appointment
- **update_client_course**: Update a client course (e.g., expiry date)
- **update_client**: The version field is required for optimistic locking.

Update an existing client


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Phorest** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all clients for business ID 12345."

**🤖 AI Agent:**
> I've retrieved the client list for business 12345. I found 50 clients on the first page, including 'Jane Doe' and 'John Smith'. Would you like to see more details for a specific client?

---

**👤 You:**
> "Show me the appointments for branch 678 today."

**🤖 AI Agent:**
> Fetching appointments for branch 678... There are 12 appointments scheduled for today. The next one is a 'Full Hair Color' at 2:00 PM for client ID 9988.

---

**👤 You:**
> "Get the timetable for staff member 5544 in branch 678."

**🤖 AI Agent:**
> Accessing staff timetable... Staff member 5544 is working from 9:00 AM to 6:00 PM today with a break scheduled at 1:00 PM. They have 3 available slots remaining.


## ❓ FAQ

**Q: Can I check in a client for their appointment using the AI?**
Yes! Use the `checkin_appointment` tool with the Business ID, Branch ID, and Appointment ID. The agent will process the check-in immediately.

**Q: How do I see a specific staff member's schedule?**
You can use the `get_staff_timetable` tool. Just provide the Business ID, Branch ID, and Staff ID to see their working hours and availability.

**Q: Is it possible to export client data to CSV?**
Yes, you can initiate an export using `create_csv_export_job` and then retrieve the status or file using `get_csv_export_job`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/phorest-alternative](https://vinkius.com/mcp/phorest-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Phorest** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `phorest-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Phorest** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "phorest-alternative": {
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

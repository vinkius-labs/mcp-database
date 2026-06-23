# vCita MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vcita)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Run your small business with online scheduling, payment collection, and client management that keeps everything in one place.

## Description
Connect your **vCita** business management account to any AI agent and simplify how you coordinate your schedule, client records, and billing through natural conversation.

### What you can do

- **Client Management** — List, search, and create new client records in your CRM with full metadata support.
- **Appointment Scheduling** — Book new services, list upcoming appointments, and cancel existing bookings instantly via AI.
- **Service Catalog** — Query your offered services and prices to understand your bookable offering.
- **Financial Tracking** — Monitor your cash flow by listing invoices, payments, and price estimates sent to clients.
- **Team Coordination** — List staff members and their roles to manage your business directory.
- **Operational Visibility** — Check account status and connection health to ensure your business engine is running smoothly.

### How it works

1. Subscribe to this server
2. Enter your vCita API Token (found in your developer portal or settings)
3. Start managing your business operations from Claude, Cursor, or any MCP client

### Who is this for?

- **Service Providers & Freelancers** — quickly book appointments and check client payment statuses via simple AI commands.
- **Small Business Owners** — monitor invoices and manage the client directory directly from the workspace.
- **Operations Managers** — coordinate staff availability and track billing history via the AI assistant.


## Available Tools (12)
- **cancel_appointment**: Cancel booking
- **create_new_booking**: Schedule a service
- **create_crm_client**: Add new customer
- **get_api_status**: Get account status
- **get_client_details**: Get client info
- **list_staff_members**: List team users
- **list_scheduled_appointments**: List bookings
- **list_crm_clients**: List CRM customers
- **list_price_estimates**: List client estimates
- **list_client_invoices**: List all invoices
- **list_recorded_payments**: List transactions
- **list_offered_services**: List bookable services


## 💬 Prompt Examples

Here are some examples of how you can interact with the **vCita** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me my upcoming appointments for this week."

**🤖 AI Agent:**
> I've retrieved your schedule. You have 3 appointments: 'Consultation' with John Doe (Tue, 10 AM), 'Strategy Session' with Jane Smith (Wed, 2 PM), and 'Follow-up' with Mike Ross (Fri, 9 AM). Which one would you like more details on?

---

**👤 You:**
> "Search for a client with the email 'jane.doe@example.com'."

**🤖 AI Agent:**
> I've found the record. Jane Doe (ID: cl_10293) is a registered client. She has one outstanding invoice for $150 and an upcoming appointment on Wednesday. Shall I retrieve her full contact history?

---

**👤 You:**
> "Book a 'New Consultation' for client 'cl_10293' on Dec 1st at 10 AM."

**🤖 AI Agent:**
> Booking successful! I've scheduled the 'New Consultation' (Service ID: svc_552) for client cl_10293 on 2024-12-01 at 10:00 AM UTC. A confirmation has been sent to the client.


## ❓ FAQ

**Q: Can I search for a client by their email address?**
Yes! Use the `list_crm_clients` tool and provide the optional email parameter. The agent will return the specific record for that client if it exists in your CRM.

**Q: How do I book a new service for an existing client?**
Use the `create_new_booking` action. You'll need to provide the Client ID, the Service ID, and the start time in ISO 8601 format (e.g., 2024-12-01T10:00:00Z).

**Q: Is it possible to list all unpaid invoices via AI?**
Absolutely. Use the `list_client_invoices` query. The agent will retrieve all your billing documents, and you can then ask the AI to filter or identify those with a 'pending' or 'overdue' status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vcita](https://vinkius.com/mcp/vcita)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **vCita** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vcita` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **vCita** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vcita": {
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

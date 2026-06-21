# EasyPractice MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/easypractice)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Equip your AI agent to manage clinic appointments, track clients, and monitor invoices via the EasyPractice API.

## Description
Integrate **EasyPractice**, the leading clinic management platform for therapists and practitioners, directly into your AI workflow. Manage your appointments and session schedules, track client profiles and interaction history, monitor clinic invoices and payment statuses, and oversee your services and pricing using natural language.

### What you can do

- **Appointment Oversight** — List and retrieve detailed information and start times for all your clinic sessions.
- **Client Intelligence** — Monitor client profiles, contact details, and appointment history across your practice.
- **Financial Monitoring** — Track clinic invoices, total amounts, and payment statuses to ensure efficient billing.
- **Service Management** — Access the service catalog to retrieve structural metadata, resolving session types and pricing tiers.

### How it works

1. Connect the EasyPractice integration to your AI assistant.
2. Authorize using your EasyPractice API Key (found in your account settings).
3. Orchestrate your clinic management and practitioner operations through intuitive conversation.

### Who is this for?

- **Clinic Managers** — Quickly check daily appointment volumes and client activity on the go.
- **Practitioners** — Research client history and upcoming schedules via chat during sessions.
- **Operations Teams** — Monitor billing statuses and organizational metadata across the clinic instantly.


## Available Tools
- **get_easypractice_account_metadata**: Retrieve metadata and usage limits for your EasyPractice account
- **get_appointment_details**: Get detailed information for a specific appointment
- **get_client_details**: Get detailed profile and appointment history for a specific client
- **quick_clinic_volume_audit**: Retrieve a high-level summary of client and appointment activity
- **list_clinic_appointments**: List all scheduled appointments in your clinic
- **list_clinic_clients**: List all clients registered in your EasyPractice clinic
- **list_clinic_invoices**: List all invoices issued by your clinic
- **list_latest_appointments**: Identify the most recently updated or scheduled appointments
- **list_clinic_services**: List all services and session types offered by your clinic
- **search_clinic_clients**: Search for clients using a name or email keyword


## 💬 Prompt Examples

Here are some examples of how you can interact with the **EasyPractice** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all appointments for tomorrow."

**🤖 AI Agent:**
> I've found 5 appointments for tomorrow, including sessions with 'John Doe' (9:00 AM) and 'Alice Miller' (11:00 AM). Would you like to see the service type for any of these appointments?

---

**👤 You:**
> "Show me the details for client 'John Doe'."

**🤖 AI Agent:**
> John Doe has 12 total appointments in your clinic. Their last session was on March 15th and they have no outstanding invoices. Should I pull their contact information for you?

---

**👤 You:**
> "Are there any unpaid invoices in the system?"

**🤖 AI Agent:**
> I've identified 3 unpaid invoices, including INV-101 ($150.00) and INV-105 ($200.00). 2 of these are past their due date. Would you like me to pull the associated client names for these invoices?


## ❓ FAQ

**Q: How do I get an EasyPractice API Key?**
Log in to your EasyPractice account, navigate to **Settings > API**, and you can generate or retrieve your unique API Key from there. API access is typically enabled for pro plans.

**Q: Can the agent book new appointments?**
This integration currently focuses on listing and auditing clinic data. Booking new appointments or sessions should be managed via your EasyPractice online booking page or calendar app.

**Q: Does the integration show client contact info?**
Yes, you can use the list_clinic_clients or search_clinic_clients tools to retrieve client profile details, including their registered email addresses and phone numbers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/easypractice](https://vinkius.com/mcp/easypractice)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **EasyPractice** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `easypractice` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **EasyPractice** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "easypractice": {
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

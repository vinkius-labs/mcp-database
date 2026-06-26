# Cliniko MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cliniko)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Manage your healthcare practice via Cliniko — handle appointments, patient records, practitioners, and treatment notes directly from any AI agent.

## Description
Connect your **Cliniko** account to any AI agent to streamline your healthcare practice management through natural conversation.

### What you can do

- **Appointment Scheduling** — List, create, retrieve, update, or cancel appointments to keep your clinic's calendar organized.
- **Patient Records** — Search for patients, create new profiles, and update existing medical records with ease.
- **Practitioner Management** — Retrieve lists and details of healthcare providers and practitioners within your account.
- **Business Locations** — Access information about your different business locations and clinics.
- **Clinical Documentation** — Create and list treatment notes to maintain accurate patient care history.

### How it works

1. Subscribe to this server
2. Enter your Cliniko API Key and User Agent
3. Start managing your clinic operations from Claude, Cursor, or any MCP-compatible client

Stop switching between tabs to check patient details or practitioner availability. Your AI acts as a dedicated medical receptionist and administrative assistant.

### Who is this for?

- **Clinic Administrators** — quickly check daily schedules and manage patient flow without manual searching.
- **Healthcare Practitioners** — retrieve patient history and treatment notes directly while preparing for consultations.
- **Medical Support Staff** — automate the process of finding practitioner IDs and business location details.


## Available Tools (14)
- **update_appointment**: Update an appointment
- **list_appointments**: Supports filtering via query parameters.

List all appointments
- **list_businesses**: List all business locations
- **list_patients**: Supports filtering via query parameters.

List all patients
- **list_practitioners**: List all practitioners
- **list_treatment_notes**: List treatment notes for a patient
- **update_patient**: Update patient details
- **create_appointment**: Create a new appointment
- **create_patient**: Create a new patient
- **create_treatment_note**: Create a treatment note
- **delete_appointment**: Cancel or delete an appointment
- **get_appointment**: Retrieve a specific appointment
- **get_patient**: Retrieve a specific patient
- **get_practitioner**: Retrieve a specific practitioner


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cliniko** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all appointments scheduled for today."

**🤖 AI Agent:**
> I've retrieved today's schedule. You have 5 appointments, including an 'Initial Consultation' with John Doe at 9:00 AM and a 'Follow-up' with Sarah Smith at 11:30 AM.

---

**👤 You:**
> "Get the details for patient ID 12345."

**🤖 AI Agent:**
> Fetching patient data... Patient ID 12345 is Robert Brown. His records show he is 42 years old and his last visit was on October 12th. Would you like to see his recent treatment notes?

---

**👤 You:**
> "Show me all business locations registered in Cliniko."

**🤖 AI Agent:**
> I found 2 business locations: 'City Health Center' (ID: 101) and 'Riverside Clinic' (ID: 102). Which one would you like to explore further?


## ❓ FAQ

**Q: Can I search for a specific patient by name using the AI?**
Yes! You can use the `list_patients` tool with a query parameter `q` to filter patients by name or other identifiers.

**Q: Is it possible to cancel an appointment through the agent?**
Absolutely. Use the `delete_appointment` tool with the specific Appointment ID to cancel or remove a booking from your Cliniko calendar.

**Q: How do I see all the practitioners registered in my account?**
Simply ask the agent to run the `list_practitioners` tool. It will return a list of all healthcare providers associated with your Cliniko account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cliniko](https://vinkius.com/mcp/cliniko)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cliniko** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cliniko` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cliniko** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cliniko": {
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

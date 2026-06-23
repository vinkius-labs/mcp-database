# Calenso MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/calenso)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage appointments, customers, and bookings online via AI.

## Description
Connect your AI agent to **Calenso** to natively manage appointment scheduling, track customer bookings, and query staff availability via natural language.

### What you can do

- **Appointment Management** — List upcoming appointments, fetch specific details, or cancel bookings effortlessly.
- **Customer Directory** — Query existing customers or automatically add new customer profiles directly from a chat conversation.
- **Service & Staff Availability** — List available bookable services, branches, and staff members dynamically.

### How it works

1. Retrieve your API Key from the Calenso portal.
2. Provide the key to this integration.
3. Ask your AI agent to list all appointments for today or add a new customer.

### Who is this for?

- **Consultants & Clinics** — Manage your schedule and client list natively within your AI workflow.
- **Service Businesses** — Rapidly check branch availability or cancel an appointment via prompt.
- **Developers** — Hook native booking endpoints directly into external workflows.


## Available Tools (8)
- **cancel_calenso_appointment**: Cancel an appointment
- **create_calenso_customer**: Create a new customer
- **get_calenso_appointment**: Get appointment details
- **list_calenso_appointments**: List all appointments
- **list_calenso_branches**: List branches/locations
- **list_calenso_customers**: List all customers
- **list_calenso_services**: List available services
- **list_calenso_staff**: List staff members


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Calenso** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my upcoming Calenso appointments."

**🤖 AI Agent:**
> Here is the information you requested based on the execution of the tools.

---

**👤 You:**
> "Cancel appointment ID 88392."

**🤖 AI Agent:**
> Here is the information you requested based on the execution of the tools.

---

**👤 You:**
> "List the bookable services and staff members."

**🤖 AI Agent:**
> Here is the information you requested based on the execution of the tools.


## ❓ FAQ

**Q: Can I cancel a booking directly from the chat?**
Yes. Provide the Appointment ID to the 'cancel_calenso_appointment' tool, and the AI agent will remove it from your schedule.

**Q: How do I add a new customer profile?**
Invoke the 'create_calenso_customer' tool with a JSON object containing the customer's details (like name and email).

**Q: Is it possible to query available staff members?**
Yes, just use the 'list_calenso_staff' tool to pull the active roster of your bookable employees.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/calenso](https://vinkius.com/mcp/calenso)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Calenso** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `calenso` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Calenso** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "calenso": {
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

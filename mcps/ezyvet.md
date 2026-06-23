# ezyVet MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ezyvet)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage your veterinary practice via ezyVet — list patients, appointments, invoices, and consults directly through your AI agent.

## Description
Connect your **ezyVet** Practice Management account to any AI agent and take full control of your clinical workflows through natural conversation.

### What you can do

- **Animal & Patient Records** — List and fetch detailed records for animals (patients) including breed and status
- **Appointment Scheduling** — Query upcoming appointments and check schedule availability directly from the cloud
- **Clinical Consults** — Access and inspect clinical data and consult history for any patient
- **Financial Billing** — List and inspect invoices to track payments and practice revenue
- **Contact Management** — Manage details for clients (owners), suppliers, and staff contacts
- **Inventory & Products** — List products available in your practice's inventory catalog

### How it works

1. Subscribe to this server
2. Enter your ezyVet Client ID, Client Secret, and Partner ID
3. Start managing your veterinary practice from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Veterinarians** — quickly review patient history or appointment details during or between consults
- **Practice Managers** — monitor clinic flow and billing status through natural language queries
- **Vet Technicians** — access patient records and product info straight from your workflow


## Available Tools (12)
- **get_animal**: Get a specific ezyVet animal by ID
- **get_appointment**: Get a specific ezyVet appointment by ID
- **get_consult**: Get a specific ezyVet consult by ID
- **get_contact**: Get a specific ezyVet contact by ID
- **get_invoice**: Get a specific ezyVet invoice by ID
- **get_me**: Get current ezyVet user profile
- **list_animals**: List all ezyVet animals (patients)
- **list_appointments**: List all ezyVet appointments
- **list_consults**: List all ezyVet consults
- **list_contacts**: List all ezyVet contacts (clients/suppliers)
- **list_invoices**: List all ezyVet invoices
- **list_products**: List all ezyVet products


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ezyVet** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all patients (animals) registered in the system."

**🤖 AI Agent:**
> I've retrieved the animal records. You have 'Bella' (Labrador, ID: 101) and 'Luna' (Persian Cat, ID: 102) among others. Which patient would you like to drill into?

---

**👤 You:**
> "Check today's appointments."

**🤖 AI Agent:**
> Searching the schedule... You have 3 appointments booked for today: 'Annual Checkup' at 10:00 AM and 'Vaccination' at 2:00 PM. Would you like the details for any of these?

---

**👤 You:**
> "List the most recent invoices."

**🤖 AI Agent:**
> Fetching financial records... The most recent invoices are INV-001 ($150.00, Paid) and INV-002 ($85.00, Pending). Shall I show you the details for INV-002?


## ❓ FAQ

**Q: Where do I find my ezyVet API credentials?**
You can generate your Client ID and Client Secret in the ezyVet Developer Portal or request them from ezyVet support. Your Partner ID is typically provided during your integration onboarding.

**Q: Does this integration support multiple practice locations?**
Yes, as long as your API credentials have access to those locations. The results will reflect the data authorized for your Partner ID and Client credentials.

**Q: Can I access clinical consult history?**
Yes, the `list_consults` and `get_consult` tools allow you to retrieve and inspect past clinical sessions and their associated data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ezyvet](https://vinkius.com/mcp/ezyvet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ezyVet** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ezyvet` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ezyVet** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ezyvet": {
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

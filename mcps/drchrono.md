# DrChrono MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/drchrono)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/drchrono-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/drchrono-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [calendar-scheduling](../categories/calendar-scheduling.md)

Manage healthcare workflows via DrChrono — handle patient records, schedule appointments, and access clinical notes directly from your AI agent.

## Description
Connect your **DrChrono** EHR account to any AI agent to streamline medical practice management through natural conversation.

### What you can do

- **Patient Management** — List, create, and update patient profiles including demographics and contact info using `list_patients` and `update_patient`.
- **Appointment Scheduling** — Manage the practice calendar by listing, creating, or retrieving specific appointment details with `list_appointments` and `create_appointment`.
- **Clinical Documentation** — Access and create clinical notes for patient visits to maintain accurate medical records via `list_clinical_notes` and `create_clinical_note`.
- **Billing & Finance** — Monitor billing claims and financial transactions to keep track of practice revenue using `list_billing_claims` and `list_billing_transactions`.
- **Practice Infrastructure** — Retrieve information about doctors, offices, and authenticated users with `list_doctors` and `list_offices`.

### How it works

1. Subscribe to this server
2. Enter your DrChrono Access Token
3. Start managing your medical practice from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Medical Practitioners** — quickly check patient history and clinical notes without navigating complex EHR menus.
- **Practice Managers** — oversee appointment schedules and billing claims through simple queries.
- **Healthcare Developers** — interact with the DrChrono API directly from the code editor to verify data structures.


## Available Tools
- **create_appointment**: Schedule a new appointment
- **create_clinical_note**: Create a clinical note
- **create_patient**: Create a new patient
- **get_appointment**: Retrieve appointment details
- **get_patient**: Retrieve a specific patient
- **get_users**: Retrieve information about the authenticated user
- **list_appointments**: List appointments
- **list_billing_claims**: List billing claims
- **list_billing_transactions**: List financial transactions
- **list_clinical_notes**: Retrieve clinical notes for visits
- **list_doctors**: List doctors associated with the account
- **list_offices**: List practice locations
- **list_patients**: List all patients
- **update_patient**: Update a patient record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DrChrono** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all patients in my DrChrono account."

**🤖 AI Agent:**
> I've retrieved the patient list. You have 15 patients registered. Would you like to see the details for a specific patient like 'John Doe' (ID: 12345)?

---

**👤 You:**
> "Schedule an appointment for patient 12345 with doctor 67890 for tomorrow at 10 AM."

**🤖 AI Agent:**
> I've scheduled the appointment for tomorrow at 10:00 AM. The appointment ID is 998877. Is there anything else you need to add to the notes?

---

**👤 You:**
> "Show me the clinical notes for recent patient visits."

**🤖 AI Agent:**
> Fetching clinical notes... I found 3 recent notes. The most recent one is from today's visit for patient ID 12345 regarding a routine checkup.


## Installation & Usage

To install and use the **DrChrono** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/drchrono](https://vinkius.com/mcp/drchrono)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

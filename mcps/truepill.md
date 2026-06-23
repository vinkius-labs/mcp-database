# Truepill MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/truepill)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Manage pharmacy operations and patient records via Truepill — create patients, find records, and track prescriptions directly from any AI agent.

## Description
Connect your **Truepill** account to any AI agent to streamline pharmacy and patient management workflows through natural conversation.

### What you can do

- **Patient Management** — Create, update, and retrieve detailed patient records including demographics and contact information.
- **Search & Discovery** — Find patients using specific criteria like name, date of birth, or zip code without needing a token first.
- **Prescription Tracking** — Access full prescription histories, status updates, and fillable details for any patient in your system.
- **Detailed Inspection** — Fetch specific prescription metadata including prescriber details, NDC, and refill counts.
- **Event Monitoring** — Retrieve webhook events to stay updated on pharmacy lifecycle changes and order statuses.

### How it works

1. Subscribe to this server
2. Enter your Truepill API Key
3. Start managing healthcare records from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Healthcare Providers** — quickly look up patient history and prescription statuses during consultations.
- **Operations Teams** — monitor pharmacy events and patient record updates without manual dashboard navigation.
- **Developers** — test and interact with the Truepill API directly from the code editor to verify patient data structures.


## Available Tools (7)
- **create_patient**: Returns a patient_token.

Create a new patient record
- **find_patient**: Find patients by demographic details
- **get_patient_prescriptions**: Get all prescriptions for a patient
- **get_patient**: Get a specific patient by token
- **get_prescription**: Get details for a specific prescription
- **get_webhook_events**: g., NOTIFY_RX, ORDER, SHIPMENT, TRANSFER).

Retrieve webhook events
- **update_patient**: g., address, phone, email) for a patient. Required fields like dob or last_name cannot be updated via this endpoint.

Update an existing patient record


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Truepill** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find a patient named Alice Smith born on 19880425."

**🤖 AI Agent:**
> I've searched the records. I found one match for Alice Smith (DOB: 1988-04-25) with patient token 'pt_987654321'. Would you like to see her full profile?

---

**👤 You:**
> "Get all prescriptions for patient pt_987654321."

**🤖 AI Agent:**
> Retrieving prescription history... Alice has 2 active prescriptions: Amoxicillin (Status: Filled) and Lisinopril (Status: Pending). Do you need the details for either of these?

---

**👤 You:**
> "Create a new patient record for Bob Jones, male, born 19751212, living in New York 10001."

**🤖 AI Agent:**
> I've successfully created the record for Bob Jones. His new patient token is 'pt_112233445'. You can now add prescriptions to this profile.


## ❓ FAQ

**Q: Can I search for a patient without having their specific patient token?**
Yes. You can use the `find_patient` tool to search by first name, last name, date of birth, or zip code to locate the correct record.

**Q: How do I check the status of all medications assigned to a patient?**
Use the `get_patient_prescriptions` tool with the patient's token. It will return a list of all prescriptions, their current status, and whether they are fillable.

**Q: Is it possible to update a patient's date of birth if it was entered incorrectly?**
No. The `update_patient` tool only allows modifications to non-required fields like address, phone, and email. Required identity fields like DOB cannot be changed via this tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/truepill](https://vinkius.com/mcp/truepill)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Truepill** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `truepill` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Truepill** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "truepill": {
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

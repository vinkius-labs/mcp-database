# Accela MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/accela)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage civic services, permits, and inspections via Accela — search records, schedule inspections, and manage land parcels directly from any AI agent.

## Description
Connect your **Accela** civic platform to any AI agent to streamline government and public data workflows. Manage the entire lifecycle of permits, inspections, and land records through natural language.

### What you can do

- **Record Management** — Search for permits and applications, create new records, and update statuses or descriptions in real-time.
- **Inspections** — List associated inspections, schedule new site visits, and update results or statuses directly from your conversation.
- **Geospatial Data** — Search for valid addresses within the jurisdiction and retrieve detailed land parcel information.
- **Contact & Documents** — Manage applicants and contractors by searching or creating contacts, and list all documents attached to specific records.

### How it works

1. Subscribe to this server
2. Enter your Accela App ID, Agency name, and Access Token
3. Start managing civic records from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Government Officials** — quickly query permit statuses and inspection schedules without navigating complex legacy portals.
- **Contractors & Developers** — check the status of applications and schedule required inspections directly from your workflow tools.
- **Data Analysts** — retrieve parcel and address data for jurisdictional reporting and planning.


## Available Tools (13)
- **create_contact**: Add a new contact to the system
- **create_record**: Create a new record (e.g., a permit application)
- **get_parcels**: Retrieve land parcel information
- **get_record**: Retrieve detailed information about a specific record
- **list_documents**: List documents attached to a record
- **list_inspections**: List inspections associated with a record or inspector
- **schedule_inspection**: Schedule a new inspection
- **search_addresses**: Search for valid addresses within the jurisdiction
- **search_contacts**: Search for people or organizations (applicants, contractors)
- **search_records**: Search for records (permits, applications) based on criteria
- **update_inspection**: Update inspection results or status
- **update_record**: Update record details
- **upload_document**: Upload a new document (e.g., blueprints, photos)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accela** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for all building permits with a 'Pending' status."

**🤖 AI Agent:**
> I found 3 pending building permits. The most recent is REC-2024-001 for a residential renovation. Would you like the full details for any of these?

---

**👤 You:**
> "Schedule a 'Final Plumbing' inspection for record REC-9982 on 2024-12-15."

**🤖 AI Agent:**
> The 'Final Plumbing' inspection for record REC-9982 has been successfully scheduled for December 15, 2024. The confirmation ID is INSP-554.

---

**👤 You:**
> "Get the detailed information for record ID REC-10293."

**🤖 AI Agent:**
> Retrieving record REC-10293... This is a 'Commercial Electrical' permit issued to 'BuildIt Corp'. Current status is 'Active' and it was last updated on 2024-11-01.


## ❓ FAQ

**Q: Can I search for specific permits by their current status?**
Yes. Use the `search_records` tool and provide a status filter (e.g., 'Pending' or 'Approved') to find all matching applications within your agency.

**Q: How do I schedule a new inspection for an existing record?**
Simply use the `schedule_inspection` tool. You will need to provide the Record ID, the type of inspection, and the desired scheduled date.

**Q: Is it possible to retrieve land parcel details using a parcel number?**
Yes, the `get_parcels` tool allows you to query the system using a parcel number to retrieve specific land and property metadata.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/accela](https://vinkius.com/mcp/accela)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accela** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accela` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accela** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accela": {
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

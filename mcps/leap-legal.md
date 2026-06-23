# LEAP Legal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/leap-legal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Manage law practice via LEAP Legal Software — matters, contacts, time tracking, bills, payments, tasks, documents, and calendar.

## Description
Connect to **LEAP Legal Software** platform and manage your entire law practice from any AI agent. Access matters, contacts, documents, time entries, calendar events, bills, payments, and tasks—all through a unified REST API.

### What you can do

- **Matters/Cases** — List, search, create, and update legal matters with status, client, and practice area
- **Contacts/Clients** — Manage your client database including individuals, organizations, and opposing parties
- **Client Portfolio** — View all matters associated with a specific client
- **Time Tracking** — Log billable and non-billable time entries against any matter
- **Bills/Invoices** — List and review bills with amounts, status, and line items
- **Payments** — Track payments received from clients
- **Tasks** — View and manage tasks associated with matters and contacts
- **Documents** — Access matter documents, filings, correspondence, and evidence
- **Calendar** — View court dates, hearings, deadlines, and meetings
- **Custom Fields** — Access custom field schemas configured for matters

### How it works

1. Subscribe to this server
2. Enter your LEAP Legal OAuth 2 access token
3. Start managing your law practice from Claude, Cursor, or any MCP-compatible client

Your AI becomes a legal practice assistant, helping you track matters, log time, manage contacts, and handle billing.

### Who is this for?

- **Solo Practitioners** — manage your entire caseload and client relationships from AI assistants
- **Law Firms** — track matters across practice areas and monitor billable time across attorneys
- **Paralegals** — quickly find matter details, documents, and client information
- **Legal Assistants** — log time entries, manage calendars, and track bills and payments
- **Law Students** — practice case management and time tracking workflows


## Available Tools (18)
- **create_leap_contact**: USE WHEN:
- User wants to add a new client
- User needs to create a new contact record
- User asks to "add a new client" or "create a contact"

PARAMETERS:
- first_name (REQUIRED): Client's first name
- last_name (REQUIRED): Client's last name
- email (OPTIONAL): Client's email address
- phone (OPTIONAL): Client's phone number
- type (OPTIONAL): Contact type — "Client" (default), "Opposing Party", "Witness", "Other"

EXAMPLES:
- "Add a new client John Smith" → call with first_name="John", last_name="Smith"
- "Create contact for opposing party Jane Doe, jane@example.com" → call with first_name="Jane", last_name="Doe", email="jane@example.com", type="Opposing Party"

Create a new contact/client in LEAP Legal
- **create_leap_matter**: USE WHEN:
- User wants to open a new legal case
- User needs to create a new matter for a client
- User asks to "create a new case" or "open a matter"

PARAMETERS:
- name (REQUIRED): Matter/case name
- contact_id (OPTIONAL): ID of the client/contact this matter belongs to
- status (OPTIONAL): Initial status — "Open" (default), "Closed", "Pending"
- practice_area (OPTIONAL): Practice area (e.g. "Family Law", "Criminal Defense")
- description (OPTIONAL): Matter description/notes

EXAMPLES:
- "Create a new matter called 'Smith Divorce'" → call with name="Smith Divorce"
- "Open a new criminal defense matter for client 456" → call with name="State v. Johnson", contact_id="456", practice_area="Criminal Defense"

Create a new matter/case in LEAP Legal
- **create_leap_time_entry**: USE WHEN:
- User wants to log time spent on a matter
- User needs to record billable hours
- User asks to "add time entry" or "log hours"

PARAMETERS:
- matter_id (REQUIRED): Matter/case ID this time entry belongs to
- description (REQUIRED): Description of the work performed
- duration_minutes (REQUIRED): Duration in minutes
- billable (OPTIONAL): Whether this is billable — true (default) or false
- rate (OPTIONAL): Hourly rate for this entry

EXAMPLES:
- "Log 2 hours of legal research for matter 123" → call with matter_id="123", description="Legal research", duration_minutes=120
- "Add 30 minute phone call with client" → call with matter_id="123", description="Phone call with client", duration_minutes=30

Create a new time entry for billing
- **get_leap_bill**: Get detailed information for a specific bill/invoice
- **get_client_leap_matters**: Useful for understanding a client's full legal portfolio.

Get all matters/cases for a specific client/contact
- **get_leap_contact**: Get detailed information for a specific contact/client
- **get_leap_matter**: Get detailed information for a specific matter/case
- **list_leap_bills**: List bills/invoices in LEAP Legal
- **list_leap_calendar_events**: List calendar events in LEAP Legal
- **list_leap_contacts**: USE WHEN:
- User wants to see all their clients and contacts
- User needs to find a client by name or email
- User is exploring their contact database
- User asks "list my clients" or "show all contacts"

PARAMETERS:
- page (OPTIONAL): Page number for pagination
- page_size (OPTIONAL): Results per page (default: 25, max: 100)

EXAMPLES:
- "List all my clients" → call with no params
- "Show my contacts" → call with no params
- "List contacts page 2" → call with page="2"

List all contacts/clients in LEAP Legal
- **list_leap_custom_fields**: List custom field schemas in LEAP Legal
- **list_leap_documents**: List documents for a specific matter
- **list_leap_matters**: Supports filtering by status, client, practice area, and date range for flexible queries.

USE WHEN:
- User wants to see all their legal matters/cases
- User needs to find matters by status, client, or practice area
- User is exploring their law firm's caseload
- User asks "what matters do I have" or "list my open cases"

PARAMETERS:
- status (OPTIONAL): Filter by matter status (e.g. "Open", "Closed", "Pending")
- practice_area (OPTIONAL): Filter by practice area (e.g. "Family Law", "Criminal Defense")
- contact_id (OPTIONAL): Filter by specific client/contact ID
- page (OPTIONAL): Page number for pagination
- page_size (OPTIONAL): Results per page (default: 25, max: 100)

EXAMPLES:
- "List all my open matters" → call with status="Open"
- "Show my family law matters" → call with practice_area="Family Law"
- "List all matters" → call with no params

List all matters/cases in LEAP Legal Software
- **list_leap_payments**: List payments received in LEAP Legal
- **list_leap_tasks**: List tasks in LEAP Legal
- **list_leap_time_entries**: Supports filtering by matter, user, and date range.

USE WHEN:
- User wants to see all logged time entries
- User needs to review billable hours for a matter
- User is preparing invoices or reviewing time reports
- User asks "show my time entries" or "list billable hours"

PARAMETERS:
- matter_id (OPTIONAL): Filter by specific matter ID
- date_from (OPTIONAL): Start date filter (YYYY-MM-DD)
- date_to (OPTIONAL): End date filter (YYYY-MM-DD)
- page (OPTIONAL): Page number for pagination
- page_size (OPTIONAL): Results per page (default: 25, max: 100)

EXAMPLES:
- "List all time entries" → call with no params
- "Show time entries for matter 123" → call with matter_id="123"
- "List time entries from April 1-7" → call with date_from="2026-04-01", date_to="2026-04-07"

List time entries in LEAP Legal
- **search_leap_matters**: Search matters/cases by keyword query
- **update_leap_matter**: Update an existing matter/case in LEAP Legal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **LEAP Legal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my open matters in LEAP Legal."

**🤖 AI Agent:**
> I found 5 open matters in your LEAP Legal account: 1) Smith Divorce [Open] — John Smith, Family Law, 2) State v. Johnson [Open] — Robert Johnson, Criminal Defense, 3) Estate of Williams [Open] — Mary Williams, Estate Planning, 4) ABC Corp Contract Dispute [Open] — ABC Corporation, Business Litigation, 5) Jones Personal Injury [Open] — Sarah Jones, Personal Injury.

---

**👤 You:**
> "Create a new time entry for 2 hours of legal research on the Smith Divorce matter."

**🤖 AI Agent:**
> Time entry created successfully! Logged 120 minutes of 'Legal research' on matter 'Smith Divorce'. Entry is marked as billable. Running total for this matter: 8.5 hours this month.

---

**👤 You:**
> "Show me all contacts for client John Smith."

**🤖 AI Agent:**
> Found 3 contacts associated with John Smith: 1) John Smith (Client) — john.smith@email.com, 555-0123, 2) Jane Smith (Spouse) — jane.smith@email.com, 555-0124, 3) Robert Williams (Opposing Counsel) — robert@williamslaw.com, 555-0456.


## ❓ FAQ

**Q: What features of LEAP Legal are available through this API?**
The API provides access to: Matters/Cases (CRUD operations), Contacts/Clients (create and list), Time Entries (list and create), Bills/Invoices (list and get), Payments (list), Tasks (list), Documents (list by matter), Calendar Events (list), and Custom Fields (list schemas). You can search matters by keyword, filter by status and practice area, and view all matters for a specific client.

**Q: How do I get a LEAP Legal API access token?**
Visit the LEAP Developer Console at developer.leap.build and register your application. Use OAuth 2 authentication to obtain an access token. The token is used as a Bearer token in the Authorization header for all API requests. Contact LEAP support if you need help setting up API access for your firm.

**Q: Can I create new matters and contacts through the API?**
Yes! You can create new matters with name, client assignment, status, and practice area. You can also create new contacts with first name, last name, email, phone, and contact type (Client, Opposing Party, Witness, etc.). Use `create_leap_matter` and `create_leap_contact` tools for these operations.

**Q: How do I track billable time with LEAP Legal API?**
Use `create_leap_time_entry` to log time against any matter. Provide the matter ID, description of work, and duration in minutes. You can specify whether the entry is billable and set a custom hourly rate. Use `list_leap_time_entries` to view all time logged against a specific matter or across all matters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/leap-legal](https://vinkius.com/mcp/leap-legal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **LEAP Legal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `leap-legal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **LEAP Legal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "leap-legal": {
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

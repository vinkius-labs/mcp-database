# PracticePanther MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/practicepanther)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage law practice via PracticePanther — matters, contacts, time tracking, bills, payments, tasks, and calendar.

## Description
Connect to **PracticePanther legal practice management** platform and manage your entire law practice from any AI agent. Access matters, contacts, documents, time entries, calendar events, bills, payments, tasks, and expenses—all through a unified REST API with OData support.

### What you can do

- **Matters/Cases** — List, search, create, and update legal matters with status, client, and practice area
- **Contacts/Clients** — Manage your client database including individuals, organizations, and opposing parties
- **Time Tracking** — Log billable and non-billable time entries against any matter
- **Bills/Invoices** — List and review bills with amounts, status, and line items
- **Payments** — Track payments received from clients
- **Tasks** — View and manage tasks associated with matters and contacts
- **Calendar** — View court dates, hearings, deadlines, and meetings
- **Custom Fields** — Access custom fields configured for matters and contacts
- **Activities** — Track calls, emails, meetings, and notes
- **Expenses** — Log and review expenses associated with matters
- **OData Support** — Use powerful OData filtering, ordering, and pagination for flexible queries

### How it works

1. Subscribe to this server
2. Enter your PracticePanther OAuth 2 access token
3. Start managing your law practice from Claude, Cursor, or any MCP-compatible client

Your AI becomes a legal practice assistant, helping you track matters, log time, manage contacts, and handle billing.

### Who is this for?

- **Solo Practitioners** — manage your entire caseload and client relationships from AI assistants
- **Law Firms** — track matters across practice areas and monitor billable time across attorneys
- **Paralegals** — quickly find matter details, documents, and client information
- **Legal Assistants** — log time entries, manage calendars, and track bills and payments
- **Law Students** — practice case management and time tracking workflows


## Available Tools
- **create_practicepanther_contact**: USE WHEN:
- User wants to add a new client
- User needs to create a new contact record
- User asks to "add a new contact" or "create a client"

PARAMETERS:
- first_name (REQUIRED): Contact's first name
- last_name (REQUIRED): Contact's last name
- email (OPTIONAL): Contact's email address
- phone (OPTIONAL): Contact's phone number
- type (OPTIONAL): Contact type — "Client", "Opposing Party", "Witness", "Referral Source", etc.

EXAMPLES:
- "Add a new contact John Smith" → call with first_name="John", last_name="Smith"
- "Create client Jane Doe, jane@example.com, 555-0123" → call with first_name="Jane", last_name="Doe", email="jane@example.com", phone="555-0123", type="Client"

Create a new contact/client in PracticePanther
- **create_practicepanther_matter**: USE WHEN:
- User wants to open a new legal matter
- User needs to create a new case for a client
- User asks to "create a new matter" or "open a case"

PARAMETERS:
- name (REQUIRED): Matter/case name
- client_id (OPTIONAL): GUID of the contact/client this matter belongs to
- status (OPTIONAL): Matter status (e.g. "Open", "Closed", "Pending")
- description (OPTIONAL): Matter description
- practice_area (OPTIONAL): Practice area for this matter

EXAMPLES:
- "Create a new matter called 'Smith Divorce'" → call with name="Smith Divorce"
- "Open a new personal injury case for client John Smith" → call with name="Smith v. Johnson", client_id="client-guid"

Create a new matter/case in PracticePanther
- **create_practicepanther_time_entry**: USE WHEN:
- User wants to log time spent on a matter
- User needs to record billable hours
- User asks to "add time entry" or "log hours"

PARAMETERS:
- matter_id (REQUIRED): GUID of the matter this time entry belongs to
- description (REQUIRED): Description of the work performed
- duration_minutes (REQUIRED): Duration in minutes
- billable (OPTIONAL): Whether this is billable — true (default) or false
- rate (OPTIONAL): Hourly rate for this entry

EXAMPLES:
- "Log 2 hours of legal research for matter 123" → call with matter_id="123", description="Legal research", duration_minutes=120
- "Add 30 minute phone call with client" → call with matter_id="123", description="Phone call with client", duration_minutes=30

Create a new time entry for billing
- **get_practicepanther_bill**: Get detailed information for a specific bill/invoice
- **get_practicepanther_contact**: Get detailed information for a specific contact/client
- **get_practicepanther_matter**: Get detailed information for a specific matter/case
- **list_practicepanther_activities**: List activities in PracticePanther
- **list_practicepanther_bills**: List bills/invoices in PracticePanther
- **list_practicepanther_calendar_events**: List calendar events in PracticePanther
- **list_practicepanther_contacts**: USE WHEN:
- User wants to see all their contacts and clients
- User needs to find a contact by name or email
- User is exploring their contact database
- User asks "list my contacts" or "show all clients"

PARAMETERS:
- top (OPTIONAL): Number of results to return
- skip (OPTIONAL): Number of results to skip for pagination
- orderby (OPTIONAL): OData order expression (e.g. "LastName asc")
- filter (OPTIONAL): OData filter expression (e.g. "Email ne null")

EXAMPLES:
- "List all my contacts" → call with no params
- "Show my clients only" → call with filter="Type eq 'Client'"
- "List contacts ordered by last name" → call with orderby="LastName asc"

List all contacts/clients in PracticePanther
- **list_practicepanther_custom_fields**: List custom fields defined in PracticePanther
- **list_practicepanther_expenses**: List expenses in PracticePanther
- **list_practicepanther_matters**: Supports OData filtering, ordering, and pagination for flexible queries.

USE WHEN:
- User wants to see all their legal matters/cases
- User needs to find matters by status, client, or practice area
- User is exploring their law firm's caseload
- User asks "what matters do I have" or "list my open cases"

PARAMETERS:
- top (OPTIONAL): Number of results to return (e.g. "10", "50", "100")
- skip (OPTIONAL): Number of results to skip for pagination
- orderby (OPTIONAL): OData order expression (e.g. "CreatedDate desc", "Name asc")
- filter (OPTIONAL): OData filter expression (e.g. "Status eq 'Open'")

EXAMPLES:
- "List all my matters" → call with no params
- "Show my open cases" → call with filter="Status eq 'Open'"
- "List matters ordered by creation date" → call with orderby="CreatedDate desc"

List all matters/cases in PracticePanther
- **list_practicepanther_payments**: List payments received in PracticePanther
- **list_practicepanther_tasks**: List tasks in PracticePanther
- **list_practicepanther_time_entries**: Supports filtering by matter, user, and date range.

USE WHEN:
- User wants to see all logged time entries
- User needs to review billable hours for a matter
- User is preparing invoices or reviewing time reports
- User asks "show my time entries" or "list billable hours"

PARAMETERS:
- top (OPTIONAL): Number of results to return
- skip (OPTIONAL): Number of results to skip for pagination
- orderby (OPTIONAL): OData order expression (e.g. "Date desc")
- filter (OPTIONAL): OData filter expression (e.g. "Matter/Name eq 'Smith Divorce'")

EXAMPLES:
- "List all time entries" → call with no params
- "Show time entries for this matter" → call with filter="MatterId eq 'matter-guid'"
- "List time entries from newest to oldest" → call with orderby="Date desc"

List time entries logged in PracticePanther
- **search_practicepanther_matters**: USE WHEN:
- User wants to search for specific matters
- User needs to find matters by name, client, or status
- User asks to "find matters about X" or "search for open cases"

PARAMETERS:
- filter (REQUIRED): OData filter expression (e.g. "contains(Name, 'Smith')", "Status eq 'Open'")
- top (OPTIONAL): Number of results to return
- orderby (OPTIONAL): OData order expression

EXAMPLES:
- "Search for matters containing 'Smith'" → call with filter="contains(Name, 'Smith')"
- "Find all open personal injury cases" → call with filter="Status eq 'Open' and PracticeArea eq 'Personal Injury'"

Search matters/cases using OData filter
- **update_practicepanther_matter**: Update an existing matter/case in PracticePanther


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PracticePanther** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my open matters in PracticePanther."

**🤖 AI Agent:**
> I found 5 open matters in your PracticePanther account: 1) Smith Divorce [Open] — John Smith, Family Law, 2) State v. Johnson [Open] — Robert Johnson, Criminal Defense, 3) Estate of Williams [Open] — Mary Williams, Estate Planning, 4) ABC Corp Contract Dispute [Open] — ABC Corporation, Business Litigation, 5) Jones Personal Injury [Open] — Sarah Jones, Personal Injury.

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

**Q: What features of PracticePanther are available through this API?**
The API provides access to: Matters/Cases (CRUD operations), Contacts/Clients (create and list), Time Entries (list and create), Bills/Invoices (list and get), Payments (list), Tasks (list), Calendar Events (list), Custom Fields (list), Activities (list), and Expenses (list). The API supports OData filtering, ordering, and pagination for flexible queries across all resources.

**Q: How do I get a PracticePanther API access token?**
PracticePanther uses OAuth 2 authentication. Visit the PracticePanther OAuth authorization endpoint to authorize your application, then exchange the authorization code for an access token at the token endpoint. The access token is a Bearer token used in the Authorization header for all API requests. Contact PracticePanther support if you need help setting up API access for your firm.

**Q: Can I filter and order results using OData?**
Yes! PracticePanther's API supports full OData query options. Use $filter for filtering (e.g. "Status eq 'Open'"), $orderby for ordering (e.g. "CreatedDate desc"), $top for limiting results, and $skip for pagination. These parameters are available on all list tools. For example, to find open matters ordered by creation date: use filter="Status eq 'Open'" and orderby="CreatedDate desc".

**Q: How do I track billable time with PracticePanther API?**
Use `create_practicepanther_time_entry` to log time against any matter. Provide the matter GUID, description of work, and duration in minutes. You can specify whether the entry is billable and set a custom hourly rate. Use `list_practicepanther_time_entries` to view all time logged against a specific matter or across all matters.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/practicepanther](https://vinkius.com/mcp/practicepanther)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PracticePanther** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `practicepanther` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PracticePanther** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "practicepanther": {
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

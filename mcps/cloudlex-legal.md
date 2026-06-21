# CloudLex Legal MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cloudlex-legal)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [document-management](../categories/document-management.md)

Manage personal injury cases via CloudLex — cases, clients, documents, medical records, liens, tasks, and communications.

## Description
Connect to **CloudLex Legal** case management platform and manage your entire personal injury practice from any AI agent. Access cases, clients, documents, medical records, liens, tasks, communications, and expenses—all through a unified API designed for plaintiff personal injury law firms.

### What you can do

- **Cases/Matters** — List, search, create, and update personal injury cases with status, client, and practice area
- **Clients/Contacts** — Manage your client database including individuals, opposing parties, witnesses, medical providers, and experts
- **Client Portfolio** — View all cases associated with a specific client
- **Documents** — Access case documents including pleadings, correspondence, evidence, and settlement documents
- **Tasks** — View and manage tasks associated with cases including due dates and assigned attorneys
- **Medical Records** — Access medical treatment records, bills, provider information, and medical summaries
- **Liens** — Track medical liens, insurance liens, and other claims against settlements
- **Communications** — View emails, phone calls, letters, and notes with clients, opposing counsel, and other parties
- **Expenses** — Track case-related expenses including court costs, expert witness fees, and medical record retrieval costs

### How it works

1. Subscribe to this server
2. Enter your CloudLex API key (available in CloudLex account settings)
3. Start managing your personal injury practice from Claude, Cursor, or any MCP-compatible client

Your AI becomes a legal practice assistant, helping you track cases, manage clients, organize documents, and monitor case expenses.

### Who is this for?

- **Personal Injury Attorneys** — manage your entire caseload and client relationships from AI assistants
- **Law Firms** — track cases across practice areas and monitor case expenses and liens
- **Paralegals** — quickly find case details, documents, medical records, and client information
- **Legal Assistants** — manage tasks, communications, and track case expenses
- **Case Managers** — organize medical records, liens, and settlement documentation


## Available Tools (15)
- **create_cloudlex_case**: USE WHEN:
- User wants to open a new legal case
- User needs to create a new matter for a client
- User asks to "create a new case" or "open a matter"

PARAMETERS:
- case_name (REQUIRED): Case/matter name
- client_id (OPTIONAL): ID of the client this case belongs to
- status (OPTIONAL): Initial status — "Open" (default), "Closed", "Pending", "Settled"
- practice_area (OPTIONAL): Practice area (e.g. "Personal Injury", "Mass Tort", "Auto Accident")
- description (OPTIONAL): Case description/notes
- incident_date (OPTIONAL): Date of the incident (YYYY-MM-DD)

EXAMPLES:
- "Create a new case called 'Smith Auto Accident'" → call with case_name="Smith Auto Accident"
- "Open a new personal injury matter for client 456" → call with case_name="State v. Johnson", client_id="456", practice_area="Personal Injury"

Create a new case/matter in CloudLex Legal
- **create_cloudlex_client**: USE WHEN:
- User wants to add a new client
- User needs to create a new contact record
- User asks to "add a new client" or "create a contact"

PARAMETERS:
- first_name (REQUIRED): Client's first name
- last_name (REQUIRED): Client's last name
- email (OPTIONAL): Client's email address
- phone (OPTIONAL): Client's phone number
- type (OPTIONAL): Contact type — "Client" (default), "Opposing Party", "Witness", "Medical Provider", "Expert"

EXAMPLES:
- "Add a new client John Smith" → call with first_name="John", last_name="Smith"
- "Create contact for opposing party Jane Doe, jane@example.com" → call with first_name="Jane", last_name="Doe", email="jane@example.com", type="Opposing Party"

Create a new client/contact in CloudLex Legal
- **get_cloudlex_case**: Get detailed information for a specific case/matter
- **get_cloudlex_client**: Get detailed information for a specific client/contact
- **get_client_cloudlex_cases**: Useful for understanding a client's full legal portfolio and case history.

Get all cases/matters for a specific client/contact
- **list_cloudlex_cases**: Supports filtering by status, practice area, client, and date range for flexible queries.

USE WHEN:
- User wants to see all their legal cases/matters
- User needs to find cases by status, client, or practice area
- User is exploring their law firm's caseload
- User asks "what cases do I have" or "list my open cases"

PARAMETERS:
- status (OPTIONAL): Filter by case status (e.g. "Open", "Closed", "Pending", "Settled")
- practice_area (OPTIONAL): Filter by practice area (e.g. "Personal Injury", "Mass Tort", "Auto Accident")
- client_id (OPTIONAL): Filter by specific client ID
- page (OPTIONAL): Page number for pagination
- page_size (OPTIONAL): Results per page (default: 25, max: 100)

EXAMPLES:
- "List all my open cases" → call with status="Open"
- "Show my personal injury matters" → call with practice_area="Personal Injury"
- "List all cases" → call with no params

List all cases/matters in CloudLex Legal
- **list_cloudlex_clients**: USE WHEN:
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
- "List clients page 2" → call with page="2"

List all clients/contacts in CloudLex Legal
- **list_cloudlex_communications**: List communications for a specific case
- **list_cloudlex_documents**: List documents for a specific case/matter
- **list_cloudlex_expenses**: List expenses for a specific case
- **list_cloudlex_liens**: List liens for a specific case
- **list_cloudlex_medical_records**: List medical records for a specific case
- **list_cloudlex_tasks**: List tasks for a specific case/matter
- **search_cloudlex_cases**: Search cases/matters by keyword query
- **update_cloudlex_case**: Update an existing case/matter in CloudLex Legal


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CloudLex Legal** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my open personal injury cases in CloudLex."

**🤖 AI Agent:**
> I found 5 open personal injury cases in your CloudLex account: 1) Smith Auto Accident [Open] — John Smith, Auto Accident, 2) Jones Slip and Fall [Open] — Jane Jones, Premises Liability, 3) Williams Medical Malpractice [Open] — Robert Williams, Medical Malpractice, 4) Brown Workplace Injury [Open] — Sarah Brown, Workers' Compensation, 5) Davis Product Liability [Open] — Michael Davis, Product Liability.

---

**👤 You:**
> "Show me all medical records for the Smith Auto Accident case."

**🤖 AI Agent:**
> Found 8 medical records for Smith Auto Accident: 1) Emergency Room Visit — City Hospital, 04/15/2026, $2,500, 2) Orthopedic Consultation — Dr. Johnson, 04/20/2026, $450, 3) Physical Therapy Sessions (6) — Rehab Center, 04/25-06/15/2026, $1,800, 4) MRI Scan — Imaging Center, 04/22/2026, $1,200, 5) Follow-up Visit — Dr. Johnson, 05/15/2026, $350. Total medical expenses: $6,300.

---

**👤 You:**
> "Create a new case for client John Smith called 'Smith v. ABC Corporation - Workplace Injury'."

**🤖 AI Agent:**
> Case created successfully! 'Smith v. ABC Corporation - Workplace Injury' has been created and linked to client John Smith. Case status is set to Open, practice area is Workers' Compensation. You can now add documents, medical records, tasks, and track expenses for this case.


## ❓ FAQ

**Q: What features of CloudLex are available through this API?**
The API provides access to: Cases/Matters (CRUD operations), Contacts/Clients (create and list), Documents (list by case), Tasks (list by case), Medical Records (list by case), Liens (list by case), Communications (list by case), and Expenses (list by case). You can search cases by keyword, filter by status and practice area, and view all cases for a specific client.

**Q: How do I get a CloudLex API key?**
Log in to your CloudLex account at cloudlex.com, navigate to Settings → Integrations or API Settings, and generate an API key. The key gives you access to your firm's case data, client information, documents, medical records, and expenses. Contact CloudLex support if you don't see the API option in your account.

**Q: Can I create new cases and clients through the API?**
Yes! You can create new cases with case name, client assignment, status, practice area, and incident date. You can also create new contacts with first name, last name, email, phone, and contact type (Client, Opposing Party, Witness, Medical Provider, Expert). Use `create_cloudlex_case` and `create_cloudlex_client` tools for these operations.

**Q: What types of contacts can I manage in CloudLex?**
CloudLex supports multiple contact types essential for personal injury practice: Clients (injured parties), Opposing Parties (defendants, insurance adjusters), Witnesses (eyewitnesses, expert witnesses), Medical Providers (doctors, hospitals, physical therapists), and Experts (medical experts, accident reconstructionists, economists). Each contact type can be linked to specific cases and communications.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cloudlex-legal](https://vinkius.com/mcp/cloudlex-legal)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CloudLex Legal** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cloudlex-legal` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CloudLex Legal** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cloudlex-legal": {
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

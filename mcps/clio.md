# Clio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [project-management](../categories/project-management.md)

Manage legal practice and matters via Clio — track cases, monitor contacts, and manage firm tasks directly from any AI agent.

## Description
Connect your **Clio** account to any AI agent and take full control of your legal practice management through natural conversation. Streamline how you manage matters, contacts, and billing natively.

### What you can do

- **Matter Oversight** — List and retrieve details for all legal matters and cases under your administration natively
- **Contact Intelligence** — Access and monitor all contacts, including people and companies, flawlessly
- **Task Management** — List and review firm tasks and to-dos to keep your practice organized securely
- **Billing Logistics** — Access generated bills and monitor their payment status to manage cash flow flawlessly
- **Firm Management** — List all internal users and attorneys within your law firm flawlessly
- **Integrated Visibility** — Retrieve detailed matter metadata including status and responsible attorneys directly within your workspace flawlessly

### How it works

1. Subscribe to this server
2. Create a Developer Application in your Clio account (one-time setup, takes about 5 minutes)
3. Enter your Client ID and Client Secret, then click **Connect with Clio** to authorize access
4. Start managing your legal practice from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Attorneys** — monitor case status and review recent matter updates using natural language
- **Legal Assistants** — audit firm task lists and verify contact details without opening the dashboard
- **Practice Managers** — quickly look up billing history and attorney assignments straight from their chat interface
- **Law Firm Ops** — verify matter structures and monitor user roles


## Available Tools (23)
- **list_matters**: Filter by status: open, closed, pending. Includes case number, description, client, and dates.

List legal cases/matters
- **get_matter**: Includes client, practice area, responsible attorney, dates, and status.

Get case details
- **list_contacts**: List firm contacts
- **create_activity**: Provide date (YYYY-MM-DD), quantity in seconds, and the type (TimeEntry or ExpenseEntry).

Log a time entry or expense
- **list_tasks**: Filter by matter for case-specific tasks. Critical for tracking court deadlines and firm-wide to-dos.

List tasks and deadlines
- **list_notes**: Optionally filter by matter ID. Includes subject, detail, date, and linked matter.

List case notes
- **create_task**: Optionally link to a matter and set a due date. Use for court deadlines, filing reminders, and internal follow-ups.

Create a new task or deadline
- **create_note**: Use for documenting conversations, strategy decisions, or research findings.

Add a note to a matter
- **list_bills**: Use to monitor firm revenue and outstanding receivables.

List invoices
- **get_bill**: Returns line items, totals, balance, due date, and associated matter.

Get invoice details
- **list_calendar_entries**: Includes summary, start/end times, location, and linked matter.

List calendar events
- **list_documents**: Filter by matter. Includes filename, category, creation date, and linked matter.

List case documents
- **list_practice_areas**: g., Civil Litigation, Corporate, Family Law). Useful for matter categorization and firm structure overview.

List practice areas
- **search_matters**: Use for finding specific cases when the user provides a keyword or partial name.

Search legal matters by keyword
- **list_matter_stages**: g., Intake, Discovery, Trial, Closed). Used for understanding matter lifecycle.

List matter stages
- **list_communications**: Includes subject, body, type, date, and linked matter/contact.

List firm communications
- **get_user_profile**: Get current user profile
- **list_users**: Useful for team management and workload distribution.

List firm users and attorneys
- **create_matter**: Requires a display number (case reference), description, and client contact ID. The client must exist before creating a matter.

Create a new legal matter
- **search_contacts**: Use this tool when looking for a specific person or organization.

Search contacts by name or email
- **get_contact**: Returns name, type, email addresses, phone numbers, and physical addresses.

Get contact details
- **create_contact**: Provide first and last name for persons. For companies, set type to "Company" and use first_name as the company name.

Create a new contact
- **list_activities**: Optionally filter by matter. Includes date, hours, rate, notes, and billing status.

List time entries and expenses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my open matters in Clio."

**🤖 AI Agent:**
> Retrieving your open matters... I found 5 items: Case #2026-001 (Civil Litigation), #2026-002 (Corporate Setup), and 3 others. Which one would you like to see the details for?

---

**👤 You:**
> "Show me the tasks for the 'City Refurb' matter."

**🤖 AI Agent:**
> Checking tasks for City Refurb... I found 3 items: 'File Motion' (Due Today), 'Witness Deposition' (Completed), and 'Review Contract' (Pending). Would you like to update any of these?

---

**👤 You:**
> "Who is the contact for the 'Jones v. Smith' case?"

**🤖 AI Agent:**
> Retrieving contact for Jones v. Smith... The primary client is Alice Jones. I can provide her email or phone number if needed.


## ❓ FAQ

**Q: How do I connect my Clio account?**
After subscribing, the setup wizard will guide you through 3 simple steps: 1) Select your data region (US, Canada, EU, or Australia). 2) Enter the Client ID and Client Secret from your Clio Developer Application. 3) Click the **Connect with Clio** button — a popup will open where you approve access. That's it! No manual token exchange or curl commands required.

**Q: Where do I find the Redirect URI for my Clio Developer Application?**
When creating your Developer Application in Clio, set the **Redirect URI** to: `https://api.vinkius.com/marketplace/oauth/callback`. This is the platform's secure callback endpoint that completes the OAuth authorization automatically.

**Q: How do I get my Client ID and Client Secret?**
Sign in to Clio and go to **Settings → Developer Applications** (direct link: `https://app.clio.com/settings/developer_applications`). Click **New Application**, give it a name, and set the **Redirect URI** to `https://api.vinkius.com/marketplace/oauth/callback`. Save the app and copy the **Client ID** and **Client Secret** (the secret is shown only once — copy it immediately).

**Q: Can I see the status of a specific legal matter?**
Yes! Use the `get_matter` tool with the matter ID. The agent will return the current status (Open, Closed, etc.), the client name, and the responsible attorney.

**Q: How do I check if a bill has been paid?**
Use the `list_bills` tool. Your agent will fetch the list of generated bills, which includes their amounts and payment statuses, directly from Clio.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clio](https://vinkius.com/mcp/clio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clio": {
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

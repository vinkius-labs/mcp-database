# Clio MCP Server

Manage legal practice and matters via Clio — track cases, monitor contacts, and manage firm tasks directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/clio)

## Overview
**Category:** project-management
**Tools Count:** 23

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


## Available Tools
- **list_matters**: Filter by status: open, closed, pending. Includes case number, description, client, and dates.

List legal cases/matters
- **get_matter**: Includes client, practice area, responsible attorney, dates, and status.

Get case details
- **list_contacts**: List firm contacts
- **list_activities**: Optionally filter by matter. Includes date, hours, rate, notes, and billing status.

List time entries and expenses
- **list_tasks**: Filter by matter for case-specific tasks. Critical for tracking court deadlines and firm-wide to-dos.

List tasks and deadlines
- **list_bills**: Use to monitor firm revenue and outstanding receivables.

List invoices
- **list_calendar_entries**: Includes summary, start/end times, location, and linked matter.

List calendar events
- **list_documents**: Filter by matter. Includes filename, category, creation date, and linked matter.

List case documents
- **create_activity**: Provide date (YYYY-MM-DD), quantity in seconds, and the type (TimeEntry or ExpenseEntry).

Log a time entry or expense
- **create_task**: Optionally link to a matter and set a due date. Use for court deadlines, filing reminders, and internal follow-ups.

Create a new task or deadline
- **list_notes**: Optionally filter by matter ID. Includes subject, detail, date, and linked matter.

List case notes
- **create_note**: Use for documenting conversations, strategy decisions, or research findings.

Add a note to a matter
- **get_bill**: Returns line items, totals, balance, due date, and associated matter.

Get invoice details
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


## Installation & Usage

To install and use the **Clio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clio](https://vinkius.com/mcp/clio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

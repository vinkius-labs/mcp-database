# Clio MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clio-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/clio-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/clio-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Practice law more efficiently with legal case management, time tracking, billing, and document organization in one system.

## Description
Connect your **Clio** (v4) account to any AI agent and take full control of your legal practice management and firm operations through natural conversation.

### What you can do

- **Matter & Case Orchestration** — List and manage legal matters programmatically, monitoring their entire lifecycle from intake to resolution in real-time
- **Billing & Activity Intelligence** — Track billable time and expenses associated with specific matters and retrieve detailed high-fidelity invoice summaries
- **Relationship CRM** — Access complete profiles for individuals and company contacts (clients, counsel) to maintain a perfectly coordinated relationship ecosystem
- **Communication Architecture** — Access logged calls, emails, and firm-wide task lists to ensure high-fidelity oversight of all firm interactions
- **Regional Flexibility** — Connect across multiple data centers (US, CA, EU, AU) using secure OAuth and regional endpoint routing directly through your agent

### How it works

1. Subscribe to this server
2. Create a Developer Application in your Clio account (one-time setup, takes about 5 minutes)
3. Enter your Client ID and Client Secret, then click **Connect with Clio** to authorize access
4. Start managing your law firm's workload from Claude, Cursor, or any MCP client

No more manual deal logging or digging through complex matter tables in the portal. Your AI acts as your dedicated legal operations specialist and billing coordinator.

### Who is this for?

- **Attorneys & Partners** — instantly retrieve case summaries and check billable hour targets using natural language commands
- **Legal Administrators** — monitor firm-wide tasks and manage client contact directories without leaving your communication tools
- **Legal Tech Developers** — integrate automated matter tracking and expense reporting into custom workflows through simple AI queries


## Available Tools
- **create_contact**: Provide first and last name for persons. For companies, set type to "Company" and use first_name as the company name.

Create a new contact
- **create_matter**: Requires a display number (case reference), description, and client contact ID. The client must exist before creating a matter.

Create a new legal matter
- **get_contact**: Returns name, type, email addresses, phone numbers, and physical addresses.

Get contact details
- **get_matter**: Includes client, practice area, responsible attorney, dates, and status.

Get case details
- **get_user_profile**: Get current user profile
- **list_activities**: Optionally filter by matter. Includes date, hours, rate, notes, and billing status.

List time entries and expenses
- **list_bills**: Use to monitor firm revenue and outstanding receivables.

List invoices
- **list_communications**: Includes subject, body, type, date, and linked matter/contact.

List firm communications
- **list_contacts**: List firm contacts
- **list_matter_stages**: g., Intake, Discovery, Trial, Closed). Used for understanding matter lifecycle.

List matter stages
- **list_matters**: Filter by status: open, closed, pending. Includes case number, description, client, and dates.

List legal cases/matters
- **list_tasks**: Filter by matter for case-specific tasks. Critical for tracking court deadlines and firm-wide to-dos.

List tasks and deadlines
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
- **list_calendar_entries**: Includes summary, start/end times, location, and linked matter.

List calendar events
- **list_documents**: Filter by matter. Includes filename, category, creation date, and linked matter.

List case documents
- **list_practice_areas**: g., Civil Litigation, Corporate, Family Law). Useful for matter categorization and firm structure overview.

List practice areas
- **search_matters**: Use for finding specific cases when the user provides a keyword or partial name.

Search legal matters by keyword
- **list_users**: Useful for team management and workload distribution.

List firm users and attorneys
- **search_contacts**: Use this tool when looking for a specific person or organization.

Search contacts by name or email


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active legal matters in my Clio account."

**🤖 AI Agent:**
> I've retrieved your active matters. You currently have 4 ongoing cases, including 'Estate Planning - John Smith' (ID: m_123) and 'Corporate Acquisition'. Which one should we check activities for?

---

**👤 You:**
> "Create a new company contact 'Acme Legal' in Clio."

**🤖 AI Agent:**
> Contact created! Acme Legal has been successfully added to your Clio directory (ID: c_456). They are now available for matter association and billing. Shall I create a new legal case for them?

---

**👤 You:**
> "Show my billable activities and outstanding invoices."

**🤖 AI Agent:**
> Retrieving financial overview... You have 15 unbilled activities totaling $2,450.00 and 3 outstanding invoices. Your largest pending bill is for 'Global Tech' (ID: b_789). Would you like the detailed breakdown?


## Installation & Usage

To install and use the **Clio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clio-alternative](https://vinkius.com/mcp/clio-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Pipedrive CRM (Full) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pipedrive-crm-full)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-crm](../categories/sales-crm.md)

Manage deals, contacts, organizations, activities, notes, and pipelines — complete Pipedrive CRM access through natural conversation.

## Description
Connect **Pipedrive CRM** to any AI agent — manage your entire sales pipeline without switching tabs.

### What you can do
- **Deals** — Search, create, and update deals with pipeline tracking
- **Contacts** — Find and create persons with email, phone, and organization
- **Organizations** — Search companies linked to deals and contacts
- **Activities** — Create calls, meetings, tasks, and emails
- **Notes** — Attach notes to deals, persons, or organizations
- **Pipelines** — View all pipeline stages and deal flow

### Who is this for?
- **Sales Reps** — Manage your pipeline without leaving your AI assistant
- **SDRs** — Quickly create leads, contacts, and activities
- **Sales Managers** — Pipeline overview and deal insights through conversation
- **RevOps** — Full CRM visibility and reporting


## Available Tools (11)
- **pd_create_activity**: Subject and type are required. Type must be one of: call, meeting, email, task, lunch, deadline. Optionally set due_date (YYYY-MM-DD) and link to deal_id, person_id, or both. Add a note for context. Activities appear in the Pipedrive calendar and task queue.

Schedule a sales activity in Pipedrive — a call, meeting, email, task, lunch, or deadline linked to deals or contacts
- **pd_create_deal**: Title is required. Optionally specify monetary value, currency (USD/EUR/GBP/etc.), linked person_id and org_id (use search tools to find these), and pipeline/stage placement (use pd_list_pipelines and pd_list_stages to find IDs). If no pipeline is specified, the deal enters the default pipeline at its first stage.

Create a new deal in your Pipedrive sales pipeline with title, value, currency, and linked contact/organization
- **pd_create_note**: Notes appear in the timeline/history of the linked record. Link to exactly one of: deal_id, person_id, or org_id. Use to log meeting summaries, call notes, or internal context on any CRM record.

Create a note in Pipedrive attached to a deal, person, or organization for activity logging
- **pd_create_person**: Name is required. Email and phone are optional but recommended for contact management. Link to an existing organization using org_id (use pd_search_organizations to find). Returns the created person with their new Pipedrive ID.

Create a new contact (person) in Pipedrive with name, email, phone, and optional organization link
- **pd_list_activities**: Returns subject, type (call/meeting/email/task/lunch/deadline), due date, due time, completion status, and linked deal/person. Use when the user asks about upcoming tasks, scheduled meetings, overdue activities, or recent sales activity.

List recent Pipedrive activities (calls, meetings, tasks, emails) with due dates, types, and completion status
- **pd_list_pipelines**: Returns pipeline name, total deal count, and whether it is active. Most Pipedrive accounts have one default pipeline, but larger teams may have separate pipelines for different sales processes (e.g., New Business vs Renewals). Use to find pipeline IDs before creating deals or filtering by pipeline.

List all sales pipelines configured in Pipedrive with their names, deal counts, and order
- **pd_list_stages**: Returns stage name, display order, number of deals at each stage, and rotten days (warning threshold). Use to find stage IDs for creating or moving deals, or to understand the sales process flow.

List the stages within a Pipedrive pipeline showing stage names, order, deal counts, and win probability
- **pd_search_deals**: Returns deal title, monetary value, currency, pipeline stage, pipeline name, linked person (contact), and organization. Use when the user wants to find a specific deal, check pipeline status, look up deal values, or see which stage a deal is in.

Search Pipedrive deals by name or keyword to find opportunities in your sales pipeline with value, stage, and contact info
- **pd_search_organizations**: Returns org name, address, and associated data. Use when the user wants to find a company, needs org IDs for linking to deals or persons, or wants to look up account details.

Search Pipedrive organizations (companies) by name to find accounts in your CRM
- **pd_search_persons**: Returns person name, email addresses, phone numbers, and linked organization. Use when the user wants to find a contact, look up someone by email, or get person IDs for linking to deals or activities.

Search Pipedrive contacts (persons) by name, email, or phone to find people in your CRM
- **pd_update_deal**: Only specified fields are updated. Common use: advance stage_id when a deal progresses, update value after negotiation, or set status to "won"/"lost" to close a deal. Available statuses: open, won, lost, deleted.

Update an existing Pipedrive deal — change stage, value, title, or mark as won/lost to reflect pipeline progress


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pipedrive CRM (Full)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for deals with Acme Corp"

**🤖 AI Agent:**
> 📊 **Deals with Acme Corp**
| Title | Value | Stage | Pipeline |
|---|---|---|---|
| Acme Enterprise License | $45,000 | Proposal Made | Sales Pipeline |
| Acme Support Plan | $12,000 | Won | Renewals |

---

**👤 You:**
> "Create a call activity for tomorrow at 2pm"

**🤖 AI Agent:**
> ✅ **Activity Created!**
- Type: Call
- Subject: Follow-up call
- Due: Tomorrow at 2:00 PM
- Status: Pending

---

**👤 You:**
> "Show me the pipeline stages"

**🤖 AI Agent:**
> 📦 **Sales Pipeline**
1. Lead In
2. Contact Made
3. Prospect Qualified
4. Proposal Made
5. Negotiations Started
6. Won ✅
7. Lost ❌


## ❓ FAQ

**Q: What Pipedrive data can I access?**
Deals, Persons, Organizations, Activities, Notes, and Pipelines. All data respects your Pipedrive permissions.

**Q: Can I create and update records?**
Yes! Create and update deals, contacts, activities, and notes — all through natural conversation.

**Q: How does authentication work?**
Uses your personal Pipedrive API token. Find it in Settings > Personal preferences > API. No OAuth flow needed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pipedrive-crm-full](https://vinkius.com/mcp/pipedrive-crm-full)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pipedrive CRM (Full)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pipedrive-crm-full` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pipedrive CRM (Full)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pipedrive-crm-full": {
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

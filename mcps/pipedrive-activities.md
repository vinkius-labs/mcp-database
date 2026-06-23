# Pipedrive Activities MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pipedrive-activities)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-crm](../categories/sales-crm.md)

Create and manage calls, meetings, tasks, emails, and deadlines — full activity tracking for your Pipedrive account.

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


## Available Tools (8)
- **pd_create_activity**: Subject and type are required. Type must be: call, meeting, email, task, lunch, or deadline (use pd_activity_types to see custom types). Set due_date (YYYY-MM-DD), due_time (HH:MM), and duration (HH:MM). Link to deals, persons, or orgs. Activities appear in the Pipedrive calendar and task queue for the assigned user.

Schedule a sales activity in Pipedrive — a call, meeting, email follow-up, task, lunch, or deadline linked to deals or contacts
- **pd_deal_activities**: Returns all scheduled, pending, and completed activities for that deal. Use when the user asks "what activities are on this deal?", "when is the next meeting for this deal?", or needs to review the engagement history of an opportunity.

Get all activities (calls, meetings, tasks) linked to a specific deal for a complete activity history
- **pd_delete_activity**: Consider marking as done (pd_mark_activity_done) instead to preserve history. Use only when the user explicitly wants to remove an activity from the record.

Permanently delete a Pipedrive activity — this removes it from history and cannot be undone
- **pd_get_activity**: Returns subject, type, dates/times, duration, notes, linked deal/person/org, and completion status. Use after listing activities to drill into a specific item.

Get complete details of a specific Pipedrive activity by ID including notes, duration, and linked records
- **pd_list_activities**: Returns subject, type (call/meeting/email/task/lunch/deadline), due date and time, whether it is done, and linked deal/person/org. Filter by done status: "true" for completed, "false" for pending/upcoming. Use when the user asks about tasks to do, scheduled meetings, overdue items, or recent sales activity.

List Pipedrive activities (calls, meetings, tasks, emails) with due dates, types, and completion status
- **pd_activity_types**: Default types: call, meeting, task, deadline, email, lunch. Teams can add custom types. Use to discover available activity types before creating activities, especially in accounts with custom configurations.

List all activity types configured in Pipedrive — both default types (call, meeting) and custom types defined by the team
- **pd_mark_activity_done**: The activity remains in history but is no longer in the pending/overdue queue. Use when the user says they completed a call, finished a meeting, or done with a task.

Mark a Pipedrive activity as completed — removes it from the pending task queue and logs it as done
- **pd_update_activity**: Only specified fields change. Use to reschedule (change due_date), rename (change subject), or reclassify (change type). Does not mark as done — use pd_mark_activity_done for that.

Update an existing Pipedrive activity — reschedule, rename, or change type


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pipedrive Activities** MCP server using an AI Agent (Claude, ChatGPT, etc.).

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

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pipedrive-activities](https://vinkius.com/mcp/pipedrive-activities)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pipedrive Activities** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pipedrive-activities` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pipedrive Activities** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pipedrive-activities": {
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

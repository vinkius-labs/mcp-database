# Zoho CRM Activities MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/zoho-crm-activities)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/zoho-crm-activities-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/zoho-crm-activities-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Create and manage tasks, calls, events, and notes — full activity tracking for your Zoho CRM.

## Description
Connect **Zoho CRM** to any AI agent — manage your entire CRM without switching tabs.

### What you can do
- **Leads** — Search and create leads with source and status tracking
- **Contacts** — Find and create contacts linked to accounts
- **Accounts** — Search companies and organizations
- **Deals** — Search, create, and track deals through pipeline stages
- **Notes** — Create notes attached to any CRM record
- **Generic List** — Query any Zoho CRM module directly

### Who is this for?
- **Sales Reps** — CRM at your fingertips through AI
- **BDRs** — Quickly qualify and create leads
- **Sales Managers** — Pipeline visibility and deal insights
- **Support Teams** — Access contact and account data seamlessly


## Available Tools
- **zoho_create_call**: Subject is required. Call_Type: Outbound or Inbound. Call_Purpose describes the reason (Prospecting, Follow-up, Demo, etc.). Call_Start_Time uses ISO format. Use to log completed calls or schedule upcoming ones.

Log a call in Zoho CRM with subject, type (Inbound/Outbound), purpose, and start time for activity tracking
- **zoho_create_event**: Event_Title, Start_DateTime, and End_DateTime are required (ISO format). Events appear in the Zoho CRM calendar and can be linked to contacts, leads, and deals. Use to schedule meetings, demos, or any time-bound activity.

Create a calendar event in Zoho CRM with title, start/end times, and description for meetings and appointments
- **zoho_create_task**: Subject is required. Status: Not Started, Deferred, In Progress, Completed, Waiting on someone else. Priority: High, Highest, Normal, Low, Lowest. Due_Date uses YYYY-MM-DD. Use for scheduling follow-ups, assigning action items, or creating reminders.

Create a task in Zoho CRM with subject, due date, priority, and status for sales and support follow-ups
- **zoho_list_calls**: Returns call subject, type (Inbound/Outbound), call result/disposition, duration, and linked contact/lead. Use when the user asks about call activity, wants to review call history, or needs to audit sales call volume.

List call logs in Zoho CRM with subject, call type (Inbound/Outbound), result, duration, and linked contacts
- **zoho_list_events**: Returns event title, start and end DateTime, location, and linked records. Events represent meetings, demos, webinars, and other calendar-based activities. Use when the user asks about scheduled meetings, upcoming events, or calendar review.

List calendar events in Zoho CRM with title, start/end dates, location, and linked contacts
- **zoho_list_notes**: Requires module (Leads, Contacts, Deals, Accounts) and recordId. Returns note title, content, and creation date. Use when the user asks "what notes are on this contact?" or wants to review the activity history of a record.

List notes attached to a specific Zoho CRM record — see the activity log and history for any contact, deal, or account
- **zoho_list_tasks**: Returns task subject, due date, status, priority, and linked record. Tasks are action items assigned to CRM users — follow-up calls, document preparation, or approval steps. Use when the user asks about pending work, due dates, or task status.

List Zoho CRM tasks with subject, due date, status (Not Started/In Progress/Completed), and priority (High/Normal/Low)
- **zoho_update_task**: Only specified fields change. Common operations: set Status to "Completed" when done, change Priority for escalation, push Due_Date when rescheduling.

Update an existing Zoho CRM task — change status, priority, due date, or subject to reflect progress


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Zoho CRM Activities** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for leads from web form"

**🤖 AI Agent:**
> 👥 **Leads from Web Form**
| Name | Email | Company | Status |
|---|---|---|---|
| John Smith | john@acme.com | Acme Corp | New |
| Maria Garcia | maria@beta.io | Beta Inc | Contacted |

---

**👤 You:**
> "Create a deal: Enterprise Plan $25,000"

**🤖 AI Agent:**
> ✅ **Deal Created!**
- Name: Enterprise Plan
- Amount: $25,000
- Stage: Qualification
- Closing: 2024-03-30


## Installation & Usage

To install and use the **Zoho CRM Activities** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/zoho-crm-activities](https://vinkius.com/mcp/zoho-crm-activities)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

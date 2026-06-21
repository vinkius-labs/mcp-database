# Pipedrive CRM (Full) MCP Server

Manage deals, contacts, organizations, activities, notes, and pipelines — complete Pipedrive CRM access through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pipedrive-crm-full)

## Overview
**Category:** sales-crm
**Tools Count:** 11

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


## Available Tools
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


## Installation & Usage

To install and use the **Pipedrive CRM (Full)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pipedrive-crm-full](https://vinkius.com/mcp/pipedrive-crm-full)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

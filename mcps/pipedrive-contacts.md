# Pipedrive Contacts MCP Server

Search, create, and manage Pipedrive persons and organizations — full contact lifecycle management through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pipedrive-contacts)

## Overview
**Category:** customer-relationship-management
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
- **pd_create_org**: Name is required. Address is optional. Once created, persons and deals can be linked to this organization. Returns the created org with its new Pipedrive ID.

Create a new organization (company/account) in Pipedrive with name and address
- **pd_create_person**: Name is required. Link to an existing organization via org_id (use pd_search_orgs to find). Pipedrive supports multiple emails and phones per person — here a single value is accepted for simplicity. Returns the created person with their new ID.

Create a new contact (person) in Pipedrive with name, email, phone, and optional organization link
- **pd_delete_person**: Use only when the user explicitly wants to delete a contact. Consider whether the contact should remain in the system for historical deal tracking before deleting.

Permanently delete a contact from Pipedrive — this action cannot be undone
- **pd_get_org**: Returns org name, address, open/won/lost deal counts, number of people linked, and all custom fields. Use after searching to drill into a specific company for full details.

Get complete details of a specific Pipedrive organization by ID, including address, deal stats, and custom fields
- **pd_get_person**: Returns full contact data: name, all emails, all phones, organization, open/won/lost deal counts, activities count, and custom fields. Use after searching to drill into a specific contact.

Get complete details of a specific Pipedrive contact by ID, including all custom fields and activity history
- **pd_list_persons**: Returns names, emails, phones, and linked orgs. Use for contact directory browsing, headcount analysis, or when the user wants to see all people in the CRM.

List all contacts in Pipedrive with names, emails, phones, and organization associations
- **pd_person_deals**: Returns deal titles, values, stages, and statuses. Use when the user asks "what deals does this person have?" or wants to see the full sales relationship history for a contact.

Get all deals linked to a specific contact person to see their sales history and active opportunities
- **pd_search_orgs**: Returns org name, address, and associated data. Use when the user asks about a company, needs org IDs for linking to persons or deals, or wants to look up account information.

Search Pipedrive organizations (companies/accounts) by name to find business entities in your CRM
- **pd_search_persons**: Returns name, email addresses, phone numbers, and linked organization. Use when the user wants to find a specific person, look up contact info by email, or get person IDs for linking to deals or activities.

Search Pipedrive contacts by name, email, or phone to find people in your CRM with their organization links
- **pd_update_org**: Only specified fields change. Use when the user wants to correct company info, update the address, or rename an account.

Update an existing Pipedrive organization — change name, address, or other properties
- **pd_update_person**: Only specified fields are changed. Use when the user wants to correct contact details, update a phone number, or change the associated organization.

Update an existing Pipedrive contact — change name, email, phone, or other properties


## Installation & Usage

To install and use the **Pipedrive Contacts** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pipedrive-contacts](https://vinkius.com/mcp/pipedrive-contacts)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

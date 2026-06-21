# HubSpot CRM (Full) MCP Server

Manage contacts, companies, deals, tickets, notes, owners, and pipelines — full access to your HubSpot CRM through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/hubspot-crm-full)

## Overview
**Category:** industry-titans
**Tools Count:** 16

## Description
Connect **HubSpot CRM** to any AI agent — instant access to your full CRM data without switching tabs.

### What you can do
- **Contacts** — Search, create, and manage contacts
- **Companies** — Find companies by name or domain
- **Deals** — Search and create deals with pipeline tracking
- **Tickets** — Create and search support tickets
- **Notes** — Create notes attached to any CRM record
- **Owners** — View all owners and team assignments
- **Pipelines** — List deal and ticket pipeline stages

### Who is this for?
- **Sales Reps** — Manage your CRM without leaving your AI assistant
- **Support Teams** — Create tickets and notes on-the-go
- **RevOps** — Pipeline snapshots and owner assignments
- **Managers** — Full CRM visibility through conversation


## Available Tools
- **hs_associate_objects**: Common association type IDs: Contact→Company=1, Company→Contact=2, Deal→Contact=3, Contact→Deal=4, Deal→Company=5, Company→Deal=6. Use when attaching a contact to a company, linking a deal to a contact, etc.

Create an association between two HubSpot CRM objects
- **hs_get_company**: Returns name, domain, industry, revenue, and employee count. Use when you need to inspect a specific company record.

Retrieve a specific HubSpot company by its unique CRM ID
- **hs_update_deal**: Use hs_list_pipelines to find valid stage IDs before updating dealstage.

Update properties on an existing HubSpot deal
- **hs_get_deal**: Returns deal name, pipeline stage, amount, close date, and assigned owner. Use when inspecting a specific opportunity.

Retrieve a specific HubSpot deal by its unique CRM ID
- **hs_search_deals**: Returns matching deals with deal name, pipeline stage, monetary amount, pipeline name, expected close date, and assigned owner. Use when the user asks about pipeline status, wants to find a specific deal, check deal amounts, or review upcoming closes.

Search HubSpot deals by name to find opportunities in your sales pipeline with stage, amount, and close date
- **hs_search_tickets**: Returns matching tickets with subject, ticket status/stage, priority (HIGH/MEDIUM/LOW), pipeline, category, and creation date. Use when the user asks about open support tickets, needs to find a specific customer issue, or wants to check ticket status.

Search HubSpot Service Hub tickets by subject or keyword to find customer support requests
- **hs_update_contact**: Provide only the fields you want to change as key-value pairs in the properties JSON.

Update properties on an existing HubSpot contact
- **hs_create_contact**: Email is the primary identifier — provide a unique email address. HubSpot will auto-deduplicate by email. The lifecycle stage can be set to control where the contact enters the funnel (subscriber, lead, marketingqualifiedlead, salesqualifiedlead, opportunity, customer, evangelist). Returns the created contact with its new HubSpot ID.

Create a new contact in HubSpot CRM with email, name, phone, and company association
- **hs_create_deal**: The dealname is required. Optionally specify pipeline (by ID — use hs_list_pipelines to find), dealstage (stage ID within that pipeline), and amount. If no pipeline is specified, the deal goes into the default pipeline. Returns the created deal with its new HubSpot ID.

Create a new deal/opportunity in the HubSpot sales pipeline with name, stage, amount, and close date
- **hs_create_note**: The note body supports HTML formatting. Optionally associate it with a contact, company, or deal by providing their IDs. Notes appear in the timeline of associated records. Use when the user wants to log a meeting summary, record a conversation, or add internal context to a CRM record.

Create an engagement note in HubSpot attached to a contact, company, or deal for activity logging
- **hs_create_ticket**: The subject is required. Optionally set the pipeline stage (hs_pipeline_stage) and priority (hs_ticket_priority: HIGH, MEDIUM, LOW). The ticket enters the default support pipeline. Returns the created ticket with its new ID.

Create a new support ticket in HubSpot Service Hub with subject, pipeline stage, and priority
- **hs_get_contact**: Returns all standard properties including name, email, phone, company, lifecycle stage, and assigned owner. Use when you already have the contact ID from a search or association lookup.

Retrieve a specific HubSpot contact by its unique CRM ID
- **hs_list_owners**: Owners are the users who can be assigned to contacts, companies, deals, and tickets. Returns owner name, email, and whether the account is active. Use when the user asks about team members, needs owner IDs for record assignment, or wants to see who has CRM access.

List all HubSpot owners (CRM users) in the account with their name, email, and active status
- **hs_list_pipelines**: For deals, shows sales pipeline stages (e.g., Appointment Scheduled → Qualified → Proposal → Closed Won). For tickets, shows support pipeline stages (e.g., New → Waiting → Closed). Returns pipeline name, stage labels, stage IDs, and display order. Use when the user needs pipeline/stage IDs for creating deals or tickets, or wants to understand the sales/support process structure.

List all deal or ticket pipelines in HubSpot with their stages, display order, and stage IDs
- **hs_search_companies**: Returns matching companies with name, website domain, industry, annual revenue, employee count, and assigned owner. Use when the user wants to find a specific company, look up organizational details, check revenue/size data, or find companies in a particular industry.

Search HubSpot companies by name, domain, or industry to find organizations in your CRM
- **hs_search_contacts**: Returns matching contacts with first name, last name, email, phone, associated company, lifecycle stage (subscriber/lead/MQL/SQL/opportunity/customer/evangelist), and assigned owner. Use when the user wants to find a specific person, look up contact details, check which lifecycle stage someone is in, or find contacts at a particular company.

Search HubSpot contacts by name, email, phone, or company name to find people in your CRM


## Installation & Usage

To install and use the **HubSpot CRM (Full)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hubspot-crm-full](https://vinkius.com/mcp/hubspot-crm-full)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

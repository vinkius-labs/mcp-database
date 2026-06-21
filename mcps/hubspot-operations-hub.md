# HubSpot Operations Hub MCP Server

Manage workflows, CRM properties, pipelines, owners, and property groups through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/hubspot-operations-hub)

## Overview
**Category:** industry-titans
**Tools Count:** 6

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
- **hs_create_property**: Create a custom property (field) on a HubSpot CRM object to extend the data model with business-specific fields
- **hs_list_all_pipelines**: Returns pipeline name, stage labels, internal stage IDs, and display order. Pipelines define the process stages for deals (sales process) or tickets (support process). Use when configuring automations, setting up deal/ticket routing, or when the user needs pipeline/stage IDs for creating records.

List all deal or ticket pipelines with their stages, IDs, and display order for workflow configuration
- **hs_list_owners**: Owners are the users who can be assigned to contacts, companies, deals, and tickets. Returns owner ID, name, email, active status, and team memberships. Use when configuring round-robin assignment rules, auditing user access, or when the user needs owner IDs for record assignment.

List all HubSpot owners (CRM users) for use in assignment workflows, with name, email, and active status
- **hs_list_properties**: Returns property internal name, display label, data type (string/number/date/enumeration), field type (text/number/date/select/checkbox), group name, and description. Essential for understanding the CRM data model. Use when the user asks "what fields exist on contacts?", wants to audit custom properties, or needs internal property names for filters/searches.

List all properties (fields) configured on a HubSpot CRM object type — contacts, companies, deals, or tickets
- **hs_list_property_groups**: Returns group internal name and display label. Property groups organize fields into logical sections in the HubSpot UI (e.g., "Contact Information", "Social Media", "Custom Fields"). Use to find valid group names before creating custom properties with hs_create_property.

List property groups for a HubSpot CRM object — the logical sections that organize properties in the UI
- **hs_list_workflows**: Returns workflow name, type (drip/standard/nurturing), enabled status (active vs inactive), and number of actions in the workflow. Workflows automate marketing, sales, and service processes — e.g., lead nurturing emails, deal stage automation, ticket routing. Use when the user asks about active automations, wants to audit workflows, or needs to check which automations are running.

List all automation workflows in HubSpot with name, type, active/inactive status, and action count


## Installation & Usage

To install and use the **HubSpot Operations Hub** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hubspot-operations-hub](https://vinkius.com/mcp/hubspot-operations-hub)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

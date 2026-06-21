# Microsoft Dynamics 365 MCP Server

Manage accounts, opportunities, orders, and business processes on Microsoft Dynamics 365 — the unified CRM & ERP platform.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/microsoft-dynamics-365)

## Overview
**Category:** industry-titans
**Tools Count:** 10

## Description
Connect your **Microsoft Dynamics 365** environment to any AI agent and manage your CRM and ERP operations through natural conversation.

### What you can do

- **Account Management** — Create, read, and update account records including contacts, addresses, and relationship hierarchies
- **Opportunity Pipeline** — Query open opportunities by stage, probability, and close date; update deal values and ownership
- **Sales Orders** — Create and manage sales orders, quotes, and invoices across your sales organization
- **Case Management** — Create support cases, track resolution progress, and manage SLA compliance
- **Financial Operations** — Query journal entries, G/L accounts, and financial dimensions (Business Central)
- **Custom Entities** — Access any Dataverse entity through the Web API, including custom tables and relationships
- **Business Process Flows** — Check active stages in business process flows and advance records through pipeline stages

### How it works

1. Subscribe to this server
2. Enter your Azure AD app credentials (Client ID, Client Secret, Tenant ID) and Dynamics 365 environment URL
3. Start managing CRM/ERP operations through Claude, Cursor, or any MCP-compatible client

The entire Microsoft ecosystem — from Teams to Power BI to LinkedIn Sales Navigator — feeds into Dynamics 365. Now your AI agent is part of that ecosystem.

### Who is this for?

- **Sales Representatives** — update opportunities, create quotes, and check pipeline status through chat
- **Customer Service Agents** — create and resolve cases without navigating the Dynamics UI
- **Finance Teams** — query financial data and journal entries across Business Central directly
- **CRM Administrators** — audit entity configurations and manage data integrity through conversation


## Available Tools
- **query_dataverse**: Common entity sets: accounts, contacts, opportunities, incidents (cases), leads, salesorders, invoices. Use OData filter syntax.

Query any Dataverse entity set
- **count_records**: Useful for dashboards without fetching full records.

Count records in a Dynamics 365 entity set
- **get_record**: Example: get_record("accounts", "00000000-0000-0000-0000-000000000001").

Get a specific Dynamics 365 record
- **create_record**: Provide field values as JSON. For lookups, use the @odata.bind format.

Create a new record in Dynamics 365
- **update_record**: Only specify the fields you want to change.

Update an existing Dynamics 365 record
- **delete_record**: This action is irreversible.

Delete a Dynamics 365 record
- **list_accounts**: Use filter to narrow results.

List Dynamics 365 accounts
- **list_opportunities**: Filter by stage, close date, or estimated value.

List sales opportunities
- **list_cases**: List support cases (incidents)
- **list_contacts**: List Dynamics 365 contacts


## Installation & Usage

To install and use the **Microsoft Dynamics 365** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/microsoft-dynamics-365](https://vinkius.com/mcp/microsoft-dynamics-365)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Salesforce MCP Server

Connect your Salesforce CRM to any AI agent — query records with SOQL, manage accounts, contacts, opportunities, run reports, and perform CRUD operations.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/salesforce)

## Overview
**Category:** industry-titans
**Tools Count:** 12

## Description
Connect your **Salesforce** CRM to any AI agent and manage your entire sales pipeline through natural conversation.

### What you can do

- **SOQL Queries** — Execute any SOQL query to retrieve data across all objects
- **Account Management** — List, view, create, and update accounts
- **Contact & Lead Management** — Browse contacts, search across all objects
- **Opportunity Tracking** — Monitor pipeline, create and update deals
- **Reports** — List and execute Salesforce reports
- **Full CRUD** — Create, read, update, and delete any SObject type
- **Global Search** — Full-text search across all Salesforce data


## Available Tools
- **list_contacts**: List Salesforce contacts
- **list_opportunities**: List sales opportunities
- **get_record**: Specify the SObject type (Account, Contact, Opportunity, Case, Lead) and the record ID.

Get a specific Salesforce record by type and ID
- **soql_query**: Example: SELECT Id, Name FROM Account WHERE Industry = 'Technology' LIMIT 10

Execute a SOQL query against Salesforce
- **describe_object**: Useful for understanding data structure.

Get metadata about a Salesforce object
- **list_reports**: List available Salesforce reports
- **run_report**: Use list_reports first to find the report ID.

Execute a Salesforce report and get results
- **global_search**: Returns matches across Accounts, Contacts, Leads, and other objects simultaneously.

Search across all Salesforce objects
- **list_accounts**: List Salesforce accounts
- **create_record**: Provide JSON fields as a string.

Create a new Salesforce record
- **update_record**: Provide the SObject type, ID, and JSON fields to update.

Update an existing Salesforce record
- **delete_record**: This action is irreversible.

Delete a Salesforce record


## Installation & Usage

To install and use the **Salesforce** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/salesforce](https://vinkius.com/mcp/salesforce)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

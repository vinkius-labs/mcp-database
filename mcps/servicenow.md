# ServiceNow MCP Server

Manage incidents, service requests, change orders, and CMDB records on ServiceNow — the enterprise ITSM backbone.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/servicenow)

## Overview
**Category:** industry-titans
**Tools Count:** 10

## Description
Connect your **ServiceNow** instance to any AI agent and manage your entire IT service lifecycle through natural conversation.

### What you can do

- **Incident Management** — Create, update, and resolve incidents. Query open tickets by priority, assignment group, or SLA breach status
- **Service Requests** — Submit and track service catalog requests, view approval chains, and check fulfillment status
- **Change Management** — Create change requests, review CAB approvals, and monitor scheduled change windows
- **CMDB Queries** — Search configuration items, explore CI relationships, and audit asset records across your infrastructure
- **Knowledge Base** — Search and retrieve knowledge articles to help with incident resolution and self-service
- **User Management** — Look up user profiles, group memberships, and role assignments across your organization
- **Custom Table Queries** — Execute SysParm-filtered queries against any ServiceNow table with full dot-walking support

### How it works

1. Subscribe to this server
2. Enter your ServiceNow instance URL and credentials
3. Start managing IT operations through Claude, Cursor, or any MCP-compatible client

Your AI agent becomes your ITSM command center — no more navigating complex Fiori dashboards to triage a P1.

### Who is this for?

- **IT Service Managers** — triage incidents and track SLA compliance through simple chat commands
- **DevOps Engineers** — create change requests and query CMDB relationships without manual data entry
- **Help Desk Analysts** — resolve tickets faster by searching the knowledge base and updating records via conversation
- **IT Directors** — get real-time dashboards on incident volume, resolution times, and backlog health


## Available Tools
- **create_record**: Provide fields as JSON string. Common tables: incident, change_request, sc_request, problem.

Create a new record in any ServiceNow table
- **search_knowledge**: Returns matching articles with KB numbers and descriptions.

Search the ServiceNow Knowledge Base
- **update_record**: Only specify the fields you want to change.

Update an existing ServiceNow record
- **delete_record**: This action is irreversible.

Delete a ServiceNow record
- **query_table**: ). Use SysParm encoded query syntax: field=value^field2=value2. Supports dot-walking for related fields.

Query any ServiceNow table with SysParm filters
- **count_records**: Useful for dashboards and metrics without fetching full records.

Get record count from a ServiceNow table
- **get_record**: Returns all fields.

Get a single ServiceNow record by sys_id
- **list_incidents**: Filter by priority, state, assignment_group, or any field. Example query: priority=1^state=1 (open P1 incidents).

List incidents with optional filters
- **list_change_requests**: Filter by state, risk, type. Example: risk=high^state=new

List change requests
- **query_cmdb**: Common tables: cmdb_ci_server, cmdb_ci_appl, cmdb_ci_db_instance, cmdb_ci_network. Example query: name=PROD-WEB-01

Query ServiceNow CMDB configuration items


## Installation & Usage

To install and use the **ServiceNow** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/servicenow](https://vinkius.com/mcp/servicenow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

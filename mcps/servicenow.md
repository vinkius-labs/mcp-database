# ServiceNow MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/servicenow)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage incidents, service requests, change orders, and CMDB records on ServiceNow — the enterprise ITSM backbone.

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


## Available Tools (10)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ServiceNow** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all P1 incidents that are unassigned."

**🤖 AI Agent:**
> Found 4 unassigned P1 incidents: 1. INC0012345 — 'Email Service Down' (opened 2h ago), 2. INC0012350 — 'VPN Authentication Failure' (opened 45min ago), 3. INC0012352 — 'ERP Integration Timeout' (opened 30min ago), 4. INC0012355 — 'Database Replication Lag' (opened 15min ago). Would you like me to assign any of these?

---

**👤 You:**
> "Create a normal change request for 'Database Upgrade to v15' assigned to the DBA team."

**🤖 AI Agent:**
> Change request CHG0045678 has been created successfully. Type: Normal, Risk: Moderate, Assignment Group: DBA Team, Short Description: 'Database Upgrade to v15'. It is now pending CAB approval. Would you like me to add implementation notes?

---

**👤 You:**
> "Search the knowledge base for 'VPN connection issues'."

**🤖 AI Agent:**
> Found 3 relevant knowledge articles: 1. KB0098765 — 'VPN Troubleshooting Guide' (Last updated: March 2026, 45 views), 2. KB0098770 — 'Corporate VPN Setup for Remote Workers', 3. KB0098780 — 'Known VPN Issues After Security Patch 2026-Q1'. Would you like me to show the resolution steps from any of these?


## ❓ FAQ

**Q: Can I query incidents filtered by priority and assignment group?**
Yes. Use the `query_table` tool with the `incident` table and SysParm query filters like `priority=1^assignment_group=Network`. Full dot-walking is supported for related fields.

**Q: How do I create a change request through the agent?**
Use the `create_record` tool with the `change_request` table. Provide key fields like short_description, category, risk, and assignment_group. The agent returns the CHG number immediately.

**Q: Can the agent search the knowledge base for solutions?**
Absolutely. The `search_knowledge` tool searches across all published knowledge articles using keyword or category filters, returning relevant articles with their KB numbers and resolution steps.

**Q: Does it support custom tables beyond the standard ITSM modules?**
Yes. The `query_table` tool works with any ServiceNow table — standard or custom (u_ prefixed). Pass the table name and your SysParm filters, and the agent handles pagination and field expansion automatically.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/servicenow](https://vinkius.com/mcp/servicenow)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ServiceNow** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `servicenow` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ServiceNow** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "servicenow": {
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

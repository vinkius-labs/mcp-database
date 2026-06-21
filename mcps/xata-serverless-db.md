# Xata (Serverless DB) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/xata-serverless-db)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/xata-serverless-db-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/xata-serverless-db-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [databases](../categories/databases.md)

Manage your serverless databases via Xata — list organizations, manage projects, branches, and execute SQL queries directly from any AI agent.

## Description
Connect your **Xata** account to any AI agent to manage your serverless data infrastructure through natural conversation. Xata combines the power of a relational database with the ease of use of a spreadsheet, all accessible via this MCP server.

### What you can do

- **Organization Management** — List, create, and update organizations and manage team members or invitations using `list_organizations` and `list_members`.
- **Project & Branch Control** — Create and manage projects and database branches across different regions with `create_project` and `create_branch`.
- **SQL Execution** — Run SQL queries or batches directly against your database branches to fetch or manipulate data using `execute_sql`.
- **Infrastructure Insights** — Retrieve branch metrics, credentials, and project limits to monitor your serverless environment with `get_branch_metrics` and `get_project_limits`.

### How it works

1. Subscribe to this server
2. Enter your Xata API Key
3. Start managing your databases from Claude, Cursor, or any MCP-compatible client

No more switching between your IDE and the Xata dashboard to check schema or run quick queries. Your AI acts as a database administrator and developer advocate.

### Who is this for?

- **Backend Developers** — run SQL queries and manage database branches directly from the code editor.
- **DevOps Engineers** — monitor project limits and branch metrics to ensure infrastructure health.
- **Data Analysts** — quickly explore organizational data and project structures through natural language.


## Available Tools
- **create_branch**: Create a new database branch
- **create_organization**: Create a new organization
- **create_project**: Create a new project
- **delete_branch**: Delete a branch
- **delete_invitation**: Delete an organization invitation
- **request_organization_deletion**: Request organization deletion
- **delete_project**: Delete a project
- **execute_sql_batch**: Execute a batch of SQL queries in a single transaction
- **execute_sql**: Execute a SQL query against a branch
- **get_branch_credentials**: Retrieve branch credentials
- **get_branch_metrics**: Retrieve branch metrics
- **get_branch**: Get branch details
- **get_organization**: Get organization details
- **get_project_limits**: Get resource limits for projects
- **get_project**: Get project details
- **list_branches**: List all branches in a project
- **list_images**: List available images
- **list_instance_types**: List available instance types for a region
- **list_invitations**: List organization invitations
- **list_members**: List organization members
- **list_organizations**: List all organizations
- **list_projects**: List all projects in an organization
- **list_regions**: List available regions
- **remove_member**: Remove a member from an organization
- **resend_invitation**: Resend an organization invitation
- **rotate_branch_credentials**: Rotate branch credentials
- **send_invitation**: Send an invitation to join an organization
- **update_branch**: Update branch details
- **update_organization**: Update organization details
- **update_project**: Update project details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Xata (Serverless DB)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Xata organizations and their details."

**🤖 AI Agent:**
> I've retrieved your organizations. You have access to 'Main-Org' (ID: org-123) and 'Dev-Sandbox' (ID: org-456). Would you like to see the projects in one of them?

---

**👤 You:**
> "Show me all branches for project 'my-database' in organization 'org-123'."

**🤖 AI Agent:**
> In the project 'my-database', I found two branches: 'main' and 'staging'. Would you like to check the metrics for the 'main' branch?

---

**👤 You:**
> "Execute SQL: SELECT name, email FROM users WHERE active = true LIMIT 5 on the main branch."

**🤖 AI Agent:**
> Query executed successfully. Here are the first 5 active users: 1. Alice (alice@example.com), 2. Bob (bob@example.com)...


## Installation & Usage

To install and use the **Xata (Serverless DB)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/xata-serverless-db](https://vinkius.com/mcp/xata-serverless-db)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Supabase MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/supabase-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/supabase-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/supabase-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage Supabase projects, databases and secrets via API — create projects, configure Postgres, manage branches and secrets from any AI agent.

## Description
Connect your **Supabase** account to any AI agent and take full control of your backend infrastructure through natural conversation.

### What you can do

- **Project Management** — List, create, pause and restore Supabase projects across regions
- **Branch Operations** — Create development branches for preview environments with isolated databases
- **Secret Management** — List, create and delete project secrets (API keys, credentials) securely
- **PostgreSQL Configuration** — View and update Postgres server settings (max_connections, work_mem, etc.)
- **Organization Discovery** — List all organizations and their member projects

### How it works

1. Subscribe to this server
2. Enter your Supabase Personal Access Token
3. Start managing your backend from Claude, Cursor, or any MCP-compatible client

No more clicking through the Supabase dashboard to check project status or manage secrets. Your AI acts as a dedicated backend engineer.

### Who is this for?

- **Developers** — quickly provision projects, create dev branches and manage secrets without leaving your IDE
- **DevOps Engineers** — audit project configurations, pause unused projects to save costs and review Postgres settings
- **Team Leads** — monitor organization health, track project creation and verify secret security across teams


## Available Tools
- **create_branch**: The branch gets an isolated copy of the database that can be modified independently. Returns the created branch with its name and status.

Create a new branch for a Supabase project
- **create_project**: Requires the project name, organization ID and optionally the region (e.g. "us-east-1", "eu-west-2") and database password. The project will be provisioned with Postgres, Auth, Storage and API services. Returns the created project with its ref.

Create a new Supabase project
- **create_secret**: Requires the secret name and value. Optionally set the branch slug (defaults to main). The secret value is encrypted at rest. Returns confirmation of creation.

Create a secret for a Supabase project
- **delete_secret**: Provide the project ref and secret name. WARNING: the secret cannot be recovered after deletion.

Delete a secret from a Supabase project
- **get_user**: Returns user ID, email, name and account metadata. Use this to verify your token is working correctly.

Get the authenticated Supabase user
- **get_postgres_config**: Get PostgreSQL configuration for a Supabase project
- **get_project**: Provide the project ref (e.g. "abcxyz123456").

Get details for a specific Supabase project
- **list_branches**: Branches are isolated copies of the project database used for preview environments and development. Returns branch name, status, creation date and parent branch info.

List branches for a Supabase project
- **list_organizations**: Each organization can contain multiple projects. Returns organization ID, name and creation date.

List Supabase organizations
- **list_projects**: Each project is an isolated instance with its own Postgres database, Auth, Storage and Edge Functions. Returns project ref, name, region, organization ID, creation date and status.

List Supabase projects
- **list_secrets**: Optionally filter by branch slug. Secrets are used to store API keys, credentials and configuration values securely.

List environment secrets for a Supabase project
- **pause_project**: The project's database and data are preserved. Provide the project ref. The project can be restored later using restore_project.

Pause a Supabase project
- **restore_project**: The project's data is fully intact. Provide the project ref.

Restore a paused Supabase project
- **update_postgres_config**: Provide the project ref and a JSON object with the settings to change (e.g. {"max_connections":200,"work_mem":"16MB"}). Changes may require a database restart.

Update PostgreSQL configuration for a Supabase project


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Supabase** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all my Supabase projects and their regions."

**🤖 AI Agent:**
> I found 4 projects: 'prod-api' (us-east-1, active), 'staging-api' (us-east-1, active), 'dev-sandbox' (eu-west-2, active) and 'analytics-db' (ap-southeast-1, paused). Would you like details on any specific project?

---

**👤 You:**
> "Create a new dev branch called 'feature-auth' for my staging-api project."

**🤖 AI Agent:**
> Done! I've created the branch 'feature-auth' for your staging-api project. It has an isolated copy of the database that you can modify independently. The branch status is 'CREATING' and should be ready in a few minutes.

---

**👤 You:**
> "Pause my dev-sandbox project to save costs."

**🤖 AI Agent:**
> Done! I've paused the 'dev-sandbox' project. All compute resources have been stopped and costs will no longer accrue. Your database and data are fully preserved. You can restore it anytime with `restore_project`.


## Installation & Usage

To install and use the **Supabase** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/supabase-alternative](https://vinkius.com/mcp/supabase-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

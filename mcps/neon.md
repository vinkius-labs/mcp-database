# Neon MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/neon)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage serverless PostgreSQL databases via Neon — provision projects, branches, endpoints and roles from any AI agent.

## Description
Connect your **Neon** account to any AI agent and take full control of your serverless PostgreSQL infrastructure through natural conversation.

### What you can do

- **Project Management** — List, create, update and delete Neon projects with region and PostgreSQL version selection
- **Branch Operations** — Create instant branches via copy-on-write cloning, set primary branches and manage branch lifecycle
- **Compute Endpoints** — Provision read-write and read-only compute hosts for your branches
- **Database Administration** — Create and list PostgreSQL databases within any branch
- **Role Management** — Create database roles (users) with auto-generated passwords for secure access
- **Connection URIs** — Get ready-to-use psql connection strings for any branch

### How it works

1. Subscribe to this server
2. Enter your Neon API Key
3. Start managing your serverless Postgres from Claude, Cursor, or any MCP-compatible client

No more clicking through the Neon console to provision a branch or grab a connection URI. Your AI acts as a dedicated DBA.

### Who is this for?

- **Developers** — instantly provision development branches, grab connection URIs and create test databases without leaving your IDE
- **DevOps Engineers** — audit project configurations, manage branches for CI/CD pipelines and review compute endpoint status
- **DBAs** — create roles, manage databases across branches and track PostgreSQL version upgrades via conversation


## Available Tools
- **get_connection_uri**: Optionally specify a branch_id to get the URI for a specific branch (defaults to the primary branch). The URI includes the host, database name, role and password. Use this to connect psql, ORM tools or application clients.

Get a PostgreSQL connection URI for a Neon project
- **create_branch**: Optionally set a human-readable name and a parent branch ID to clone from (if omitted, clones from the project's primary branch). Branches are created instantly with zero data copy overhead. Returns the new branch along with its initial endpoints, databases and roles.

Create a new branch in a Neon project
- **create_database**: Requires the database name. Optionally set the owner role name (must exist in the branch — see list_roles). Returns the new database metadata.

Create a new database in a Neon branch
- **create_endpoint**: Specify the endpoint type: "read_write" for full access or "read_only" for read replicas. A branch can have at most one read_write endpoint. Returns the new endpoint with its connection host and configuration.

Create a compute endpoint for a Neon branch
- **create_project**: Optionally set a human-readable name, AWS region (e.g. "aws-us-east-2", "aws-eu-central-1") and PostgreSQL version (15, 16, 17). A default branch, database and read-write endpoint are automatically provisioned. Returns the new project along with its initial connection URIs, roles, databases and endpoints.

Create a new Neon project
- **create_role**: The role can be used to authenticate database connections and own databases. Provide the project_id, branch_id and desired role name. Returns the new role metadata including the generated password.

Create a new database role in a Neon branch
- **delete_branch**: The primary branch cannot be deleted — set another branch as primary first. Provide the project_id and branch_id. WARNING: this action is irreversible and destroys all branch data.

Delete a Neon branch
- **delete_project**: The project is recoverable for 7 days via the Neon console. All associated branches, databases, endpoints and data are deleted. Provide the project_id. WARNING: this action destroys all data in the project.

Delete a Neon project
- **get_branch**: Provide both the project_id and branch_id.

Get details for a specific Neon branch
- **get_project**: Provide the project_id (e.g. "purple-shape-411361") obtained from list_projects.

Get details for a specific Neon project
- **list_branches**: Each branch is an isolated PostgreSQL environment with its own compute, databases and roles. Branches can be created from any point-in-time using copy-on-write cloning. Returns branch ID, name, parent ID, primary status, creation date and current state. Use the project_id from list_projects.

List branches in a Neon project
- **list_databases**: Each database has a name, owner role and creation metadata. Use the project_id and branch_id to scope the query.

List databases in a Neon branch
- **list_endpoints**: Each endpoint has a type (read_write or read_only), host address, current state (active, idle, suspended) and autoscaling configuration. A branch can have at most one read_write endpoint. Use the project_id and branch_id.

List compute endpoints for a Neon branch
- **list_projects**: Each project is a workspace that contains branches, compute endpoints, databases and roles. Returns project ID, name, region, PostgreSQL version, creation date and resource usage metadata. Use this as the starting point for all Neon operations — you need a project_id to manage branches, databases or endpoints.

List all Neon projects
- **list_roles**: Each role has a name, creation date and privilege metadata. Use the project_id and branch_id to scope the query. Roles are used to authenticate database connections and control access.

List database roles in a Neon branch
- **set_primary_branch**: The primary branch is the default source for new branch cloning and receives the default read-write compute endpoint. Provide the project_id and the branch_id to promote.

Set a branch as the primary branch of a Neon project
- **update_project**: Provide the project_id and the new name. This does not affect branches, databases or endpoints.

Update a Neon project name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Neon** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Neon projects and show me which regions they're in."

**🤖 AI Agent:**
> I found 3 projects in your Neon account: 'prod-analytics' (aws-us-east-2, PG 16), 'staging-api' (aws-eu-central-1, PG 15) and 'dev-sandbox' (aws-us-east-2, PG 17). Would you like more details on any of them?

---

**👤 You:**
> "Create a new branch called 'feature-auth' from the primary branch of my project."

**🤖 AI Agent:**
> I've created branch 'feature-auth' (br-wispy-leaf-789012) in your project. It was cloned instantly from the primary branch using copy-on-write. The branch is ready with its own compute endpoint and databases. Want me to get the connection URI?

---

**👤 You:**
> "Get the connection URI for the main branch of my project."

**🤖 AI Agent:**
> Here's your connection URI: `postgresql://neondb_owner:xxxxxxxx@ep-cool-darkness-123456.us-east-2.aws.neon.tech/neondb?sslmode=require`. You can use this with psql, your ORM or any PostgreSQL client. The password was auto-generated by Neon.


## ❓ FAQ

**Q: How do I create a Neon API Key?**
Log in to the [**Neon Console**](https://console.neon.tech), go to **Account Settings** > **API Keys** (or **Organization Settings** > **API Keys**), click **Create New**, choose the scope (Personal, Organization or Project-scoped), and copy the token immediately — it is shown only once.

**Q: What is a Neon branch and how does branching work?**
A Neon branch is an isolated PostgreSQL environment with its own compute, databases and roles. Branches are created instantly using copy-on-write cloning from a parent branch (default: primary). This means zero data copy and instant provisioning. Each branch gets its own compute endpoints and can have different PostgreSQL schemas and data.

**Q: Can I get a ready-to-use connection URI?**
Yes! Use the `get_connection_uri` tool with your project_id and optionally a branch_id. It returns a complete PostgreSQL connection string (postgres://user:password@host/dbname) ready to use with psql, ORMs or application clients.

**Q: Can the agent delete projects and branches?**
Yes, the agent has tools to delete both projects and branches. Deleting a project marks it for recovery (7-day grace period) but destroys all associated data. Deleting a branch is irreversible and removes all its databases, roles and endpoints. Use caution when executing these actions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/neon](https://vinkius.com/mcp/neon)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Neon** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `neon` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Neon** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "neon": {
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

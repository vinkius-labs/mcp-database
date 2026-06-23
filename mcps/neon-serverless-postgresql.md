# Neon (Serverless PostgreSQL) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/neon-serverless-postgresql)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Manage serverless database infrastructure via Neon — spawn zero-copy branches, audit projects, and monitor compute endpoints.

## Description
Connect your **Neon** account to any AI agent and take full control of your serverless PostgreSQL infrastructure, database branching, and project orchestration through natural conversation.

### What you can do

- **Project Orchestration** — List all managed serverless workspaces and retrieve detailed regional deployment metrics and regional Caps directly from your agent
- **Zero-Copy Branching** — Instantly spawn brand new database branches (CoW) containing identical production schema duplicates for isolated feature testing or rapid CI/CD cycles
- **Compute Management** — Discover and list explicit compute endpoints (e.g., ep-misty-water-123) to retrieve the exact connection strings required for your application drivers
- **Branch Audit** — Inspect the execution footprint of specific branches, tracking storage deltas and timeline points (LSN) to understand exactly when a branch split from its parent
- **Database Inventory** — Enumerate internal SQL database schemas and catalog namespaces mapped inherently to specific branches to guide your connection logic
- **Role Management** — List and audit PostgreSQL user identities and credential roles capable of querying against specific bounded logical nodes securely
- **Resource Provisioning** — Initialize fresh serverless workspaces or permanently wipe out entire database ecosystems with irreversible architectural commands

### How it works

1. Subscribe to this server
2. Enter your Neon API Key
3. Start managing your serverless Postgres from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Backend Developers** — create isolated testing branches and verify database schemas through natural conversation without manual CLI scripts
- **Database Administrators** — audit compute endpoint resource usage and monitor storage caps across multiple Neon projects directly from your workspace
- **Platform Engineers** — manage database roles and automate project provisioning efficiently to maintain high-reliability standards


## Available Tools (10)
- **create_branch**: Duplicates Petabytes of PostgreSQL storage instantly using filesystem CoW links, generating an isolated query testing ground tied back directly to the `parent_id` source.

Spawn a zero-copy clone (Branch) of a PostgreSQL dataset
- **create_project**: Provision an empty Neon Project Serverless Workspace
- **delete_project**: Destroys all edge-served connection strings, severs active client connections, and completely evaporates physical NVMe-backed storage blocks.

Permanently wipe out a complete Neon Postgres ecosystem
- **get_branch**: Deconstruct the execution footprint of one specific Branch
- **get_project**: g. AWS eu-central-1) and storage size consumption caps bounded specifically to this project ID.

Analyze core routing logic mapping a Neon Project
- **list_branches**: Maps `main` branches to experimental `feature-123` branches spawned in milliseconds containing identical production schema duplicates.

List Copy-on-Write (CoW) Branches resolving to a Project
- **list_databases**: g. `main_db`, `analytics_db_schema`). Crucial for forming absolute Postgres connection strings resolving directly to correct schemas.

Identify internal SQL Database schemas mapped inherently to a Branch
- **list_endpoints**: eu-central-1.aws.neon.tech`) used practically within standard PgBouncer drivers to actively ingest real query traffic to associated active branches.

Discover connection routing endpoints spanning the Neon project
- **list_projects**: List architectural Neon Serverless PostgreSQL Projects
- **list_roles**: Maps directly to standard SQL internal `CREATE USER` outputs wrapped safely upstream.

Extract PostgreSQL user Roles operating on a Branch


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Neon (Serverless PostgreSQL)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all serverless projects in my Neon account"

**🤖 AI Agent:**
> I've retrieved your Neon projects. Currently, you have 3 workspaces: 'prod-cluster' (Region: AWS us-east-1), 'staging-env', and 'dev-sandbox'. Would you like to see the active branches for the production cluster?

---

**👤 You:**
> "Create a new branch called 'feat-user-auth' from the 'main' branch"

**🤖 AI Agent:**
> Spawning zero-copy clone… Success. I've created the 'feat-user-auth' branch (ID: br-12345) from your main source. This branch is now isolated and ready for queries. I'll provide the new compute endpoint URL for this branch immediately.

---

**👤 You:**
> "What databases and roles are configured on branch 'br-12345'?"

**🤖 AI Agent:**
> Retrieving branch inventory… On 'br-12345', I've identified 2 databases: 'main_app' and 'analytics'. There are 3 active roles: 'neondb_owner', 'app_writer', and 'readonly_user'. I can help you verify the specific permissions for any of these roles if you'd like.


## ❓ FAQ

**Q: What is Neon's 'Zero-Copy Branching' and how do I use it through the agent?**
Zero-copy branching allows you to clone a multi-terabyte database instantly using Copy-on-Write (CoW). Use the `create_branch` tool by providing a parent branch ID. Your agent will trigger the backend to generate an isolated clone in milliseconds, perfect for running migrations or testing features against production-like data.

**Q: Can my agent retrieve the exact connection strings for my compute endpoints?**
Yes. Use the `list_endpoints` tool with your Project ID. Your agent will retrieve the explicit hostnames (e.g., `ep-misty-water-123.aws.neon.tech`) used to actively ingest real query traffic to your serverless Postgres branches.

**Q: How do I check the storage consumption for a specific Neon branch?**
The `get_branch` tool retrieves the deconstructed execution footprint of an individual branch. Your agent will report the storage limits and exact number of bytes consumed uniquely by that branch's data delta since it split from its parent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/neon-serverless-postgresql](https://vinkius.com/mcp/neon-serverless-postgresql)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Neon (Serverless PostgreSQL)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `neon-serverless-postgresql` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Neon (Serverless PostgreSQL)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "neon-serverless-postgresql": {
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

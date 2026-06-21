# Neon (Serverless PostgreSQL) MCP Server

Manage serverless database infrastructure via Neon — spawn zero-copy branches, audit projects, and monitor compute endpoints.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/neon-serverless-postgresql)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

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


## Available Tools
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


## Installation & Usage

To install and use the **Neon (Serverless PostgreSQL)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/neon-serverless-postgresql](https://vinkius.com/mcp/neon-serverless-postgresql)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Turso MCP Server

Automate distributed database workflows via Turso — manage edge locations, organizations, and libSQL databases directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/turso)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

## Description
Connect your **Turso** account to any AI agent and take full control of your serverless SQLite infrastructure through natural conversation.

### What you can do

- **Organizations & Locations** — Identify root organizational tenants and lookup physical global Fly.io datacenter mappings
- **Databases & Groups** — Enumerate the complete libSQL Edge Database registry and logical groups orchestrating DB locations
- **Database Management** — Provision a massively distributed database, retrieve architectural metadata, and permanently delete instances
- **Security & Tokens** — Mints secure connection tokens, list active execution JWTs, and rotate database keys to block old tokens instantly

### How it works

1. Subscribe to this server
2. Enter your Turso API Token
3. Start managing your edge databases from Claude, Cursor, or any MCP-compatible client

No more context-switching between the terminal and your workspace. Your AI agent becomes your database operations command center.

### Who is this for?

- **Platform engineers** — monitor global database fleets, rotate compromised tokens, and check replica regions in seconds
- **Backend developers** — provision new test environments on the fly and verify libSQL metadata without leaving the IDE
- **DevOps teams** — quickly script group migrations and validate token expirations via AI
- **System administrators** — identify zombie databases and clean up unused serverless resources efficiently


## Available Tools
- **create_database**: Provide the organization slug, database name, and target group.

Provision a massively distributed Serverless SQLite database
- **create_database_token**: Mint a secure connection Token tied strictly to a specific DB
- **delete_database**: This action is irreversible.

Permanently deletes a global libSQL database
- **get_database_details**: Introspect exact architectural traits of one target libSQL instance
- **rotate_database_tokens**: Revoke all pre-existing Tokens for a database
- **list_databases**: Enumerate the complete libSQL Edge Database registry
- **list_database_groups**: Get Turso logical groups orchestrating DB locations
- **list_edge_locations**: Lookup physical global Fly.io datacenter mappings (Locations)
- **list_organizations**: Identify Turso Edge SQLite root organizational tenants
- **list_database_tokens**: List active Database execution JWT Tokens


## Installation & Usage

To install and use the **Turso** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/turso](https://vinkius.com/mcp/turso)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

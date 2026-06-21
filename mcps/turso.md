# Turso MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/turso)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/turso-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/turso-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Automate distributed database workflows via Turso — manage edge locations, organizations, and libSQL databases directly from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Turso** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Turso databases and their hostnames."

**🤖 AI Agent:**
> You have 3 databases in the organization 'startup-inc': 1. 'prod-db' (prod-db-startup.turso.io), 2. 'staging-auth' (staging-auth-startup.turso.io), and 3. 'analytics-edge' (analytics-edge-startup.turso.io). Do you need details or connection tokens for any of them?

---

**👤 You:**
> "Create a new database named 'user-cache' in the 'default' group."

**🤖 AI Agent:**
> I've successfully provisioned the 'user-cache' database. It has been allocated to the 'default' group and is available at 'user-cache-startup.turso.io'. Would you like me to mint a connection token for it?

---

**👤 You:**
> "Invalidate all tokens for the 'legacy-db' database immediately."

**🤖 AI Agent:**
> All previous JWT connection tokens for the 'legacy-db' instance have been successfully rotated and invalidated. Any clients using the old credentials will now be denied access. Let me know if you need to generate a new replacement token.


## Installation & Usage

To install and use the **Turso** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/turso](https://vinkius.com/mcp/turso)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

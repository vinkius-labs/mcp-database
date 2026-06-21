# Hasura (Instant GraphQL & REST Engine) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hasura-instant-graphql-rest-engine)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/hasura-instant-graphql-rest-engine-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/hasura-instant-graphql-rest-engine-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Instantly connect to your Hasura engine to execute GraphQL queries, manage metadata, analyze SQL execution plans, and monitor server health.

## Description
Connect your **Hasura** engine to any AI agent to automate database management and API orchestration through natural language.

### What you can do

- **GraphQL Operations** — Execute complex queries and mutations directly against your /v1/graphql endpoint with full variable support.
- **Metadata Management** — Track tables, define relationships, and manage permissions programmatically using the Metadata API.
- **Performance Analysis** — Use the explain tool to inspect generated SQL and execution plans to optimize your database performance.
- **Server Monitoring** — Check server health, verify metadata consistency, and retrieve real-time configuration and version details.
- **Database Backups** — Trigger pg_dump operations on connected Postgres sources for quick schema exports.

### How it works

1. Subscribe to this server
2. Provide your Hasura GraphQL Endpoint URL
3. Enter your Admin Secret for secure access
4. Start querying and managing your data layer from Claude, Cursor, or any MCP client

### Who is this for?

- **Backend Developers** — Test queries and manage schema tracking without leaving the terminal or IDE.
- **Data Engineers** — Quickly inspect execution plans and perform database dumps for migration tasks.
- **DevOps Engineers** — Monitor Hasura health and configuration consistency across different environments.


## Available Tools
- **check_health**: Can optionally use strict mode to verify metadata consistency.

Monitor Hasura server health
- **execute_graphql**: Supports queries, mutations, and batched requests.

Execute a GraphQL query or mutation
- **execute_metadata**: Execute a Hasura Metadata API operation
- **explain_graphql**: Analyze the generated SQL and execution plan for a GraphQL query
- **get_config**: Retrieve Hasura server configuration
- **get_version**: Get Hasura server version and type
- **pg_dump**: Execute pg_dump on a connected Postgres source


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hasura (Instant GraphQL & REST Engine)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Run a GraphQL query to fetch the first 5 users and their email addresses."

**🤖 AI Agent:**
> I've executed the `execute_graphql` tool. Here are the results: User 1 (admin@example.com), User 2 (dev@example.com)...

---

**👤 You:**
> "Explain the performance of this GraphQL query: { users { id name } }"

**🤖 AI Agent:**
> Using `explain_graphql`, I've analyzed the query. The generated SQL is 'SELECT id, name FROM users'. The execution plan shows an Index Scan with a cost of 0.00..12.40.

---

**👤 You:**
> "Check the health of my Hasura server and verify metadata consistency."

**🤖 AI Agent:**
> I've called `check_health` with strict mode. The server is healthy and all metadata is currently consistent.


## Installation & Usage

To install and use the **Hasura (Instant GraphQL & REST Engine)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hasura-instant-graphql-rest-engine](https://vinkius.com/mcp/hasura-instant-graphql-rest-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

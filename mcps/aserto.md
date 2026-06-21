# Aserto MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aserto)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/aserto-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/aserto-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage authorization policies and evaluate access control decisions via Aserto — run Rego queries, check user permissions, and audit decision logs.

## Description
Connect your **Aserto** tenant to any AI agent to manage and evaluate fine-grained access control policies through natural conversation.

### What you can do

- **Authorization Checks** — Use `authz_is` to determine if a specific user identity is authorized to perform actions based on policy and resource context.
- **Rego Query Execution** — Execute custom Rego queries against your authorizer using `authz_query` to inspect policy data or evaluate complex logic.
- **Decision Trees** — Retrieve full decision tree values across policy modules with `authz_decisiontree` for UI logic or deep policy inspection.
- **Control Plane Management** — Send commands to connected Edge Authorizers using `control_plane_exec` to sync policy instances or directories.
- **Audit & Logging** — List and retrieve decision logs using `list_decision_logs` to maintain a clear audit trail of all authorization events.

### How it works

1. Subscribe to this server
2. Enter your Aserto Tenant ID and API URL
3. Provide your Authorizer and Decision Logs API keys
4. Start evaluating security policies directly from your AI assistant

### Who is this for?

- **Security Engineers** — quickly test policy changes and verify authorization logic without manual API calls
- **Backend Developers** — integrate and debug fine-grained access control (FGAC) during the development lifecycle
- **Compliance Officers** — audit decision logs and verify that access control policies meet regulatory requirements


## Available Tools
- **authz_decisiontree**: Get decision tree values across all policy modules
- **authz_is**: Determine if a user is authorized to perform an action
- **authz_query**: Execute a general Rego query against the Authorizer
- **control_plane_exec**: Send commands to a connected Edge Authorizer
- **get_decision_log**: Retrieve a signed download URL for a specific log object
- **list_decision_logs**: List available decision log storage objects
- **query_decision_logs**: Query the last N decisions from decision logs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aserto** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if user 'alice@example.com' is authorized to 'read' the 'document_123' resource using the 'peoplefinder' policy."

**🤖 AI Agent:**
> I've evaluated the policy via `authz_is`. The decision for 'read' is **true**. Alice has the required permissions based on the provided resource context.

---

**👤 You:**
> "Run a Rego query to list all roles defined in 'data.system.roles'."

**🤖 AI Agent:**
> Executing `authz_query`... The query returned the following roles: ['admin', 'editor', 'viewer'].

---

**👤 You:**
> "List the available decision logs for my current policies."

**🤖 AI Agent:**
> I've retrieved the decision logs using `list_decision_logs`. I found 3 storage objects available for the 'production-policy' ID. Would you like to inspect a specific log?


## Installation & Usage

To install and use the **Aserto** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aserto](https://vinkius.com/mcp/aserto)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

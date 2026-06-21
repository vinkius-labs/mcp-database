# Cerbos MCP Server

Decouple authorization logic from your application. Evaluate permissions, generate query plans, and manage access control via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/cerbos)

## Overview
**Category:** developer-tools
**Tools Count:** 6

## Description
Connect your **Cerbos** instance to any AI agent to manage complex authorization policies through natural language conversation.

### What you can do

- **Permission Evaluation** — Use `check_resources` to instantly verify if a principal can perform specific actions on resources based on your policies.
- **Query Planning** — Generate AST-based query plans with `plan_resources` to filter database results according to user permissions.
- **AuthZEN Compliance** — Leverage standardized access requests using `authzen_evaluation` and `authzen_evaluations` tools.
- **System Monitoring** — Check instance health and build metadata using `get_server_info` and `get_authzen_config`.

### How it works

1. Subscribe to this server
2. Provide your Cerbos instance base URL (e.g., `http://localhost:3592`)
3. Start auditing and testing your access control logic directly from your chat interface

### Who is this for?

- **Software Engineers** — debug complex RBAC/ABAC policies without manual API calls
- **Security Auditors** — verify permission logic across different roles and resource attributes
- **DevOps Teams** — monitor Cerbos instance metadata and configuration status


## Available Tools
- **get_authzen_config**: Returns endpoint URLs for the AuthZEN APIs
- **authzen_evaluation**: Single action evaluation using the AuthZEN entity model
- **authzen_evaluations**: Supports execute_all, deny_on_first_deny, and permit_on_first_permit semantics.

Batch evaluation of multiple access requests using AuthZEN
- **check_resources**: This is a read-only evaluation.

Evaluates permissions for a principal on a set of resources
- **plan_resources**: Produces a query plan for obtaining a list of resources a principal is allowed to access
- **get_server_info**: Returns the version and build details of the Cerbos instance


## Installation & Usage

To install and use the **Cerbos** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cerbos](https://vinkius.com/mcp/cerbos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

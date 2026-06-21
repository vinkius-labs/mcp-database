# Permit.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/permitio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/permitio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/permitio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Orchestrate full-stack authorization, manage RBAC/ReBAC policies, and evaluate permissions in real-time via Permit.io.

## Description
Connect your **Permit.io** account to any AI agent to manage your application's authorization layer through natural language. This server allows you to evaluate permissions, manage your authorization schema, and handle user facts without touching code.

### What you can do

- **Policy Evaluation** — Instantly check if a user is permitted to perform specific actions on resources using the `check_permission` tool.
- **Schema Management** — Create resources, define roles, and assign permissions dynamically to build RBAC or ReBAC (Relationship-Based Access Control) structures.
- **Fact Management** — Provision users and tenants directly into your authorization environment to keep your permission data in sync.
- **AuthZen Compatibility** — Use standardized AuthZen evaluation tools for interoperable access control checks.
- **ReBAC Relations** — Define complex relationships between resources to handle hierarchical or ownership-based permissions.

### How it works

1. Subscribe to this server
2. Enter your Permit.io API Key (and optionally your PDP URL)
3. Start managing your authorization policies from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — Quickly test authorization logic or provision test users and roles without leaving the IDE.
- **Security Engineers** — Audit and update access control policies through a conversational interface.
- **Product Managers** — Define new feature permissions and roles as part of the product requirements workflow.


## Available Tools
- **assign_permissions_to_role**: Assign permissions to a role
- **assign_role_to_user**: Assign a role to a user in a tenant
- **authzen_access_evaluation**: AuthZen Access Evaluation
- **authzen_action_search**: AuthZen Action Search
- **authzen_bulk_evaluations**: AuthZen Bulk Evaluations
- **authzen_resource_search**: AuthZen Resource Search
- **authzen_subject_search**: AuthZen Subject Search
- **bulk_assign_roles**: Bulk assign roles (max 2000)
- **bulk_create_tenants**: Bulk create tenants (max 2000)
- **bulk_create_users**: Bulk create users (max 3000)
- **bulk_relationship_tuples**: Bulk create relationship tuples (max 1000)
- **check_permission**: Check if a user is permitted to perform an action on a resource
- **create_relation**: Create a ReBAC relation between resources
- **create_relationship_tuple**: Create a ReBAC relationship tuple
- **create_resource**: Create a new resource in the schema
- **create_role**: Create a new role in the schema
- **create_tenant**: Create a new tenant fact
- **create_user**: Create a new user fact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Permit.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if user 'admin@company.com' is permitted to 'delete' the 'server' resource in tenant 'production'."

**🤖 AI Agent:**
> I've evaluated the permission. The user 'admin@company.com' is **permitted** to perform the 'delete' action on the 'server' resource in the 'production' tenant.

---

**👤 You:**
> "Create a new resource 'document' with actions 'read', 'write', and 'share' in project 'my-app' environment 'dev'."

**🤖 AI Agent:**
> I have successfully created the 'document' resource with the specified actions in your 'dev' environment.

---

**👤 You:**
> "Assign the permissions 'document:read' and 'document:write' to the 'editor' role in project 'my-app' environment 'dev'."

**🤖 AI Agent:**
> The 'editor' role has been updated. It now has 'read' and 'write' permissions for the 'document' resource.


## Installation & Usage

To install and use the **Permit.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/permitio](https://vinkius.com/mcp/permitio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

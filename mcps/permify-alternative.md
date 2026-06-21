# Permify MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/permify-alternative)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/permify-alternative-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/permify-alternative-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage fine-grained authorization and access control via Permify — write schemas, manage relation tuples, and perform real-time permission checks.

## Description
Connect your **Permify** instance to any AI agent to orchestrate complex authorization models and access control policies through natural language.

### What you can do

- **Schema Management** — Write, read, and partially update authorization models (DSL) for specific tenants using `write_schema` and `partial_write_schema`.
- **Data Handling** — Manage relation tuples and attributes via `write_data` to define how users relate to resources.
- **Permission Checks** — Perform resource-based authorization checks with `check_permission`, or execute `bulk_check_permissions` for high-scale validation.
- **Relationship Auditing** — Query stored relational tuples with `read_relationships` and expand permissions to see who has access to what.
- **Multi-Tenancy** — Create, list, and delete isolated tenants to manage multiple client environments from a single interface.

### How it works

1. Subscribe to this server
2. Enter your Permify API URL and Secret Token
3. Start managing your IAM infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Engineers** — Audit and verify access control logic and relationship graphs without manual API calls
- **Backend Developers** — Quickly update schemas and test relationship tuples during development cycles
- **DevOps Teams** — Automate tenant provisioning and policy bundle deployments through the agent


## Available Tools
- **bulk_check_permissions**: Check multiple permissions in a single request
- **check_permission**: Perform a resource-based authorization check
- **create_tenant**: Create a new Permify tenant
- **delete_bundle**: Delete a predefined bundle
- **delete_data**: Delete relation tuples and attributes
- **delete_tenant**: Delete a Permify tenant
- **expand_permissions**: Retrieve all subjects that have a relationship with an entity
- **list_schemas**: List all schema versions for a tenant
- **list_tenants**: List all Permify tenants
- **lookup_entity**: Find which resources a user can perform an action on
- **lookup_subject**: Find which subjects can do an action on an entity
- **partial_write_schema**: Partially update an authorization model
- **read_attributes**: Query stored attributes
- **read_bundle**: Retrieve details of a specific bundle
- **read_relationships**: Query stored relational tuples
- **read_schema**: Inspect a specific schema version
- **run_bundle**: Execute a predefined bundle
- **subject_permission**: List which permissions a user can perform on an entity
- **write_bundle**: Define or update data bundles
- **write_data**: Create relation tuples and attribute data
- **write_schema**: Write an authorization model schema


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Permify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if user 'user:123' has 'edit' permission on 'document:doc-001' in tenant 'default'."

**🤖 AI Agent:**
> I've performed the check using `check_permission`. The result is 'ALLOWED'. User 123 has the necessary edit rights for that document.

---

**👤 You:**
> "List all schema versions for tenant 'production-v1'."

**🤖 AI Agent:**
> Fetching schema history... I found 3 versions for 'production-v1'. The latest version is 'v20231027-01'. Would you like to inspect its details using `read_schema`?

---

**👤 You:**
> "Create a new tenant called 'client-alpha-test'."

**🤖 AI Agent:**
> Executing `create_tenant`... Success! The tenant 'client-alpha-test' has been created with ID 'cat-9920'. You can now start writing its authorization schema.


## Installation & Usage

To install and use the **Permify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/permify-alternative](https://vinkius.com/mcp/permify-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

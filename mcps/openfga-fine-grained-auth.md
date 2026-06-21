# OpenFGA (Fine-Grained Auth) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/openfga-fine-grained-auth)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/openfga-fine-grained-auth-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/openfga-fine-grained-auth-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage fine-grained authorization with OpenFGA — create stores, define authorization models, and manage relationship tuples directly from your AI agent.

## Description
Connect your **OpenFGA** instance to any AI agent to manage Relationship-Based Access Control (ReBAC) through natural conversation. OpenFGA is an open-source fine-grained authorization solution inspired by Google's Zanzibar.

### What you can do

- **Store Management** — Create, list, and delete isolated stores to manage authorization data for different environments or applications.
- **Authorization Modeling** — Define and retrieve complex authorization models using types and relations to represent your system's permissions.
- **Tuple Management** — Write, read, and track changes to relationship tuples that define which users have which relations to specific objects.
- **Relationship Checks** — Instantly evaluate whether a user has a specific relation to an object (e.g., 'can user:anne view document:1?').
- **Health Monitoring** — Quickly check the status of your OpenFGA instance to ensure high availability.

### How it works

1. Subscribe to this server
2. Enter your OpenFGA API URL and API Token (if applicable)
3. Start managing your authorization logic from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Engineers** — Audit relationship tuples and verify authorization models without manual API calls.
- **Backend Developers** — Quickly test and iterate on authorization models during development directly from the IDE.
- **DevOps & SREs** — Monitor store health and manage authorization environments across different clusters.


## Available Tools
- **batch_check_relations**: Perform multiple checks in one request
- **check_relation**: Check if a user has a relation to an object
- **create_store**: Create a new OpenFGA store
- **delete_store**: Delete an OpenFGA store
- **expand_relation**: Expand a relation into a tree
- **get_authorization_model**: Get a specific authorization model
- **get_store**: Get OpenFGA store details
- **health_check**: Check OpenFGA server health
- **list_authorization_models**: List authorization models
- **list_objects**: List all objects a user can access
- **list_stores**: List all OpenFGA stores
- **list_users**: List all users who have a relation to an object
- **read_changes**: Read changes to relationship tuples
- **read_tuples**: Query stored relationship tuples
- **write_authorization_model**: Write a new authorization model
- **write_tuples**: Add or delete relationship tuples


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OpenFGA (Fine-Grained Auth)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my OpenFGA stores."

**🤖 AI Agent:**
> I've retrieved your OpenFGA stores. You have 3 stores: 'Staging' (ID: 01H1...), 'Production' (ID: 01H2...), and 'Lab' (ID: 01H3...).

---

**👤 You:**
> "Check if user 'anne' has the 'viewer' relation to 'document:doc1' in store 01H1..."

**🤖 AI Agent:**
> I checked the relation in store 01H1... and the result is 'allowed: true'. User 'anne' does have 'viewer' access to 'document:doc1'.

---

**👤 You:**
> "Create a new OpenFGA store named 'Security-Audit-Logs'."

**🤖 AI Agent:**
> The store 'Security-Audit-Logs' has been successfully created with ID: 01J9...


## Installation & Usage

To install and use the **OpenFGA (Fine-Grained Auth)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/openfga-fine-grained-auth](https://vinkius.com/mcp/openfga-fine-grained-auth)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Apideck MCP Server

Unify your software stack with Apideck — manage CRM contacts, orchestrate Vault connections, and execute proxy requests across dozens of platforms through one API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/apideck)

## Overview
**Category:** developer-tools
**Tools Count:** 6

## Description
Connect **Apideck** to your AI agent to streamline how you interact with multiple SaaS platforms. By using Apideck's Unified APIs, your agent can communicate with various CRM providers and manage user integrations without writing custom code for every service.

### What you can do

- **Unified CRM Access** — List and filter contacts across different CRM providers like Salesforce, HubSpot, or Pipedrive using the `list_crm_contacts` tool.
- **Vault Management** — Create sessions for users to link their own accounts (`create_vault_session`), list existing connections, and retrieve or delete specific service links.
- **API Proxying** — Execute direct requests to downstream service endpoints using `execute_proxy` when you need specific functionality not covered by the unified schema.
- **Connection Auditing** — Inspect the status and details of active integrations using `get_vault_connection` to ensure data flow is healthy.

### How it works

1. Subscribe to this server
2. Provide your Apideck API Key, App ID, and Consumer ID
3. Start querying your unified ecosystem from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers** — who want to interact with multiple APIs through a single, normalized interface directly from their IDE.
- **Product Managers** — who need to audit user connections and CRM data across different environments without manual API calls.
- **Support Teams** — who need to verify if a customer's integration is correctly configured in the Vault through natural language.


## Available Tools
- **list_crm_contacts**: g., salesforce, hubspot) using the Unified CRM API.

List CRM contacts from a unified integration
- **delete_vault_connection**: Delete a Vault connection
- **get_vault_connection**: Get a specific Vault connection
- **execute_proxy**: Execute a Proxy API request
- **list_vault_connections**: List Vault connections
- **create_vault_session**: Create a Vault session


## Installation & Usage

To install and use the **Apideck** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/apideck](https://vinkius.com/mcp/apideck)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Frontegg MCP Server

Manage B2B identity, provision users, and oversee tenants via AI agents with Frontegg.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/frontegg)

## Overview
**Category:** developer-tools
**Tools Count:** 12

## Description
Connect your **Frontegg** environment to any AI agent to automate your B2B SaaS identity management through the Model Context Protocol (MCP). Frontegg is a powerful user management and authentication platform designed specifically for modern SaaS applications. This MCP server enables you to manage multi-tenant architectures, provision new users, and audit security configurations directly through natural conversation.

### Key Features

- **Tenant Orchestration** — List all customer accounts (tenants), retrieve their configuration details, and programmatically create or delete tenants.
- **User Provisioning** — Access your global user database, fetch detailed profiles across tenants, and instantly invite or remove users.
- **Role & Permission Discovery** — List all system roles and granular permissions to audit your security and access control models.
- **M2M Token Management** — Retrieve Machine-to-Machine tokens for specific tenants to simplify backend integrations.
- **Real-time Synchronization** — Keep your identity and access management operations accessible to your AI assistant without leaving your primary workspace.
- **Secure Environment Access** — Authenticate securely using Vendor Client ID and API Keys to perform administrative operations safely.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Frontegg Client ID and API Key (found in your Vendor Workspace)
3. Start managing your B2B identities from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps & IT Admins** — quickly check tenant configurations or user access levels without manual dashboard navigation.
- **SaaS Founders & PMs** — get a real-time overview of customer provisioning and role assignments via simple AI commands.
- **Support Engineers** — automate the retrieval of user IDs and tenant associations while troubleshooting access issues.


## Available Tools
- **create_tenant**: Create a new tenant
- **create_user**: Provision a user
- **delete_tenant**: Delete a tenant
- **delete_user**: Remove a user
- **check_environment_status**: Verify API connection
- **get_tenant_details**: Get tenant metadata
- **get_user_details**: Get user metadata
- **list_m2m_tokens**: List machine tokens
- **list_permissions**: List granular permissions
- **list_system_roles**: g. Admin, Read-Only) available for assignment.

List roles
- **list_tenants**: List all tenants/accounts
- **list_users**: List users globally


## Installation & Usage

To install and use the **Frontegg** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/frontegg](https://vinkius.com/mcp/frontegg)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

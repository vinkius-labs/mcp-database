# Frontegg MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/frontegg)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/frontegg-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/frontegg-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage B2B identity, provision users, and oversee tenants via AI agents with Frontegg.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Frontegg** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List the first 10 tenants in our Frontegg environment."

**🤖 AI Agent:**
> Retrieving tenants... I found 10 active customer tenants, including 'Acme Corp' (ID: tnt_123) and 'Globex Inc' (ID: tnt_456). Would you like to see the users for Acme Corp?

---

**👤 You:**
> "Find the user details for 'jane@example.com'."

**🤖 AI Agent:**
> Searching users... I found Jane Doe (jane@example.com). She is assigned to tenant 'Acme Corp' and has the 'Admin' role. Her account was created on Oct 1st.

---

**👤 You:**
> "Create a new tenant named 'Stark Industries'."

**🤖 AI Agent:**
> Tenant created! I have successfully provisioned the new tenant 'Stark Industries' in your Frontegg environment. The new Tenant ID is tnt_789012.


## Installation & Usage

To install and use the **Frontegg** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/frontegg](https://vinkius.com/mcp/frontegg)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# BoxyHQ (Enterprise SSO) MCP Server

Manage Enterprise SSO and Directory Sync (SCIM) via BoxyHQ — configure SAML/OIDC connections and automate user provisioning directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/boxyhq-enterprise-sso)

## Overview
**Category:** fort-knox
**Tools Count:** 8

## Description
Connect your **BoxyHQ** instance to any AI agent to streamline enterprise authentication and user lifecycle management through natural language.

### What you can do

- **SSO Connections** — Add, update, and manage SAML and OIDC connections for specific tenants and products.
- **Directory Sync (SCIM)** — Create and configure SCIM 2.0 directories to automate user provisioning and de-provisioning.
- **Connection Auditing** — Retrieve detailed connection metadata using tenant IDs, product IDs, or client IDs.
- **Metadata Management** — Configure IdP metadata via raw XML (Base64) or direct metadata URLs for rapid deployment.
- **Lifecycle Control** — Update existing security configurations or delete stale connections to maintain a clean security posture.

### How it works

1. Subscribe to this server
2. Enter your BoxyHQ Instance URL and API Key
3. Start managing enterprise identity workflows from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Engineers** — quickly audit and update SSO configurations across multiple tenants without manual dashboard navigation.
- **DevOps & SREs** — automate the creation of SCIM directories and SAML connections during customer onboarding.
- **Product Managers** — verify the status of enterprise integrations and connection health directly from the chat interface.


## Available Tools
- **add_connection**: Add a new SAML or OIDC connection
- **create_directory**: 0 protocol.

Create a Directory Sync (SCIM) connection
- **delete_connection**: Delete an SSO connection
- **get_connections**: Get SSO connections
- **get_directory_groups**: List all groups for a tenant/product directory
- **get_directory_users**: List all users for a tenant/product directory
- **health_check**: Check BoxyHQ service health
- **update_connection**: Update an existing SSO connection


## Installation & Usage

To install and use the **BoxyHQ (Enterprise SSO)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/boxyhq-enterprise-sso](https://vinkius.com/mcp/boxyhq-enterprise-sso)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

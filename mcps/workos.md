# WorkOS MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/workos)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/workos-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/workos-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage enterprise organizations, SSO connections, and directory sync on WorkOS — the platform for enterprise-ready features.

## Description
Connect your **WorkOS** account to any AI agent and manage your enterprise identity infrastructure through natural conversation.

### What you can do

- **Organization Management** — Browse and list all enterprise organizations (tenants), create new records, and manage authorized domains
- **SSO Monitoring** — List and audit active Single Sign-On (SSO) connections (SAML, OIDC) configured for your enterprise customers
- **Directory Sync** — Monitor active HRIS and SCIM directory instances and retrieve deep details on sync status and provider types
- **Roster Management** — Retrieve the complete list of users and organizational groups synced from external directories directly from your agent
- **Audit Compliance** — Stream and retrieve audit log events for any organization to monitor security and compliance activities
- **Tenant Insights** — Quickly find unique organization, connection, and directory IDs required for enterprise feature configuration
- **Connectivity Health** — Verify the status and metadata of SSO links and directory connections to ensure uptime

### How it works

1. Subscribe to this server
2. Enter your WorkOS API Key
3. Start managing your enterprise features through Claude, Cursor, or any MCP-compatible client

No more manual navigation through the WorkOS dashboard to check a directory sync status. Your AI agent becomes your enterprise identity administrator.

### Who is this for?

- **Enterprise Engineers** — monitor SSO connection health and troubleshoot directory sync issues through simple chat commands
- **Product Managers** — audit the list of organizations and verified domains for roadmap and launch planning
- **Security & Compliance Teams** — retrieve audit logs and monitor user groups for access control verification
- **Support Teams** — quickly lookup organization details and user rosters to provide rapid technical assistance


## Available Tools
- **create_workos_organization**: Provide the name and a list of authorized domains.

Creates a new organization record
- **get_audit_log_events**: Returns a stream of events tracked in the organization.

Retrieves audit log events for an organization
- **get_sso_connection_details**: Retrieves details for a specific SSO connection
- **get_directory_details**: g. Okta, Azure AD) of a directory ID.

Retrieves metadata for a specific directory instance
- **get_organization_details**: Retrieves details for a specific organization
- **list_sso_connections**: Lists all active SSO connections
- **list_directories**: Lists all active Directory Sync instances
- **list_directory_groups**: Lists all groups synced from a directory
- **list_workos_organizations**: Lists all organizations in the WorkOS account
- **list_directory_users**: Lists all users synced from a directory


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WorkOS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all organizations in my WorkOS account."

**🤖 AI Agent:**
> I found 5 organizations: 1. 'Acme Corp' (ID: org_01E...), 2. 'Global Tech' (ID: org_01F...), 3. 'Stark Industries' (ID: org_01G...), and 2 others. Which one would you like to see details for?

---

**👤 You:**
> "Check the status of SSO connections for 'Acme Corp'."

**🤖 AI Agent:**
> Acme Corp (org_01E...) has 2 active SSO connections: 1. Okta SAML (Status: ACTIVE, ID: conn_01H...) and 2. Azure AD OIDC (Status: ACTIVE, ID: conn_01I...). Both links are healthy and operational.

---

**👤 You:**
> "List all users synced from the directory 'dir_01J...'."

**🤖 AI Agent:**
> I found 120 users in directory dir_01J.... The most recently synced users are: 1. John Doe (john@acme.com), 2. Jane Smith (jane@acme.com), and 3. Robert Brown (robert@acme.com). Would you like to see the full roster or filter by group?


## Installation & Usage

To install and use the **WorkOS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/workos](https://vinkius.com/mcp/workos)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

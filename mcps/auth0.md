# Auth0 MCP Server

Manage IAM operations—users, clients, connections, and logs in your Auth0 tenant directly via your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/auth0)

## Overview
**Category:** fort-knox
**Tools Count:** 10

## Description
Connect your **Auth0** tenant to any AI agent and empower it to become a master Identity and Access Management (IAM) operator. Handle sophisticated user operations and global security queries directly through natural conversation.

### What you can do

- **User Management** — List all users, search profiles, view connected social identities, and explicitly delete user data for right-to-be-forgotten requests
- **Client & IdP Connections** — Inspect configured Auth0 applications (SPAs, M2M APIs) and identity provider connections configured within your hub
- **RBAC & Actions** — Query global authorization roles and deployed Actions logic (serverless pipeline triggers) seamlessly
- **Tenant Logs** — Retrieve the system-level chronology of all actions, identifying blocked anomalous logins, tripped rate limits, and configuration changes instantly

### How it works

1. Subscribe to this secure MCP Server
2. Supply your Auth0 Domain and Management API Token
3. Talk to Auth0 securely through Claude, Cursor, or any compatible AI client

Your AI agent eliminates the need to navigate the verbose Auth0 dashboard while debugging identity flows.

### Who is this for?

- **Security & IAM Engineers** — quickly query detailed tenant logs or blocked login IPs purely from chat without manually searching tables
- **App Developers** — inspect User ID schemas, check OAuth app boundaries (Clients), and verify metadata mappings instantly during development
- **Compliance Officers** — guarantee swift PII user deletions and review global connection mappings in a conversational format


## Available Tools
- **delete_user**: Vaporizes all bound external identity links, MFA setups, and locally-held database credentials instantly, ensuring complete privacy compliance during active right-to-be-forgotten regulatory requests.

Permanently delete a user profile directly from Auth0
- **get_client**: 0 and OIDC configuration defined on an Auth0 application. Details allowable JWT token lifetimes, explicit allowed web origins/callbacks that defeat CSRF/Open Redirects, and mandatory encryption specifications enforcing end-to-end payload security.

Detailed OIDC properties configured for a single Client
- **get_connection**: Use this to audit parameters specifying explicit password strength validations, linked metadata attributes, or specialized enterprise-domain auto-routing triggers assigned uniquely to this specific strategy.

View details and strategies of a single authentication connection
- **get_user**: Use to view highly-sensitive identifiers, user_metadata (preference tracking editable by end user), and arrays mapping every linked external identity currently bound exclusively to this single unified account.

Retrieve the unified JSON profile for a specific Auth0 user
- **list_actions**: Actions alter authorization flows in real-time, block rogue logins, push enriched profiling into CRM, or force impromptu physical MFA checks.

List serverless Javascript logic executing dynamically in pipelines
- **list_clients**: Crucial for auditing grant types enforced globally on specific app boundaries.

List all logical applications/clients spanning this Auth0 tenant
- **list_connections**: Shows configurations targeting pure Auth0 Databases, external Google/Facebook Social wrappers, and rigid AD/LDAP infrastructure synced behind restrictive corporate firewalls.

List all Identity Provider (IdP) connections attached to Auth0
- **list_logs**: Captures successful logings, failed JWT validations, aggressive rate limits tripped, silent user migrations executed, and administrative mutations made continuously within the console dashboard.

Retrieve the chronological stream of all executed Auth0 tenant logs
- **list_roles**: Used to securely decouple authorization scopes from standard authentication, allowing APIs to restrict backend mutations securely via verified RBAC permission tokens attached intrinsically into emitted JWTs.

List RBAC roles defined intrinsically within the Auth0 Core Engine
- **list_users**: Includes core Auth0 attributes, creation timestamps, and customized app_metadata mappings securely controlled globally by the backend.

List all users registered in the Auth0 tenant


## Installation & Usage

To install and use the **Auth0** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/auth0](https://vinkius.com/mcp/auth0)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Auth0 MCP Server

Manage identity and access via Auth0 — list users, create accounts, audit logs, manage clients and review connections from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/auth0-alternative)

## Overview
**Category:** fort-knox
**Tools Count:** 13

## Description
Connect your **Auth0** tenant to any AI agent and take full control of your identity infrastructure through natural conversation.

### What you can do

- **User Management** — List, search, create, update and delete users with full profile details
- **Email Lookup** — Find users instantly by their email address
- **Activity Auditing** — Review user-specific logs (logins, failures, password changes) and global tenant logs
- **Application Audit** — List all registered client applications with their types and configurations
- **Connection Review** — Browse identity connections (Google, GitHub, SAML, OIDC, database) and their settings
- **Role Management** — List RBAC roles and their permission sets
- **Organization Overview** — View multi-tenant organizations configured in your tenant

### How it works

1. Subscribe to this server
2. Enter your Auth0 domain and Management API Token
3. Start managing your identity from Claude, Cursor, or any MCP-compatible client

No more wrestling with hundred browser tabs. Your AI acts as a dedicated identity operations engineer.

### Who is this for?

- **Security Teams** — quickly audit user activity logs, review failed login attempts and check blocked accounts
- **DevOps Engineers** — manage users programmatically, audit client applications and review identity connections
- **Product Managers** — monitor user growth, check organization membership and review application registrations


## Available Tools
- **create_user**: Requires the connection (e.g. "Username-Password-Authentication" for default DB connection) and email. Optionally set a password and username. Returns the created user with their user_id.

Create a new user in Auth0
- **delete_user**: All associated data (sessions, logs, metadata) will be deleted. Provide the user_id. WARNING: this action is irreversible.

Delete an Auth0 user
- **get_client**: Provide the client_id.

Get details for a specific Auth0 client (application)
- **get_user**: Provide the user_id (e.g. "auth0|abc123" or "google-oauth2|xyz789").

Get details for a specific Auth0 user
- **get_user_by_email**: Returns all users matching the email (there may be multiple if they signed up via different connections). Useful for finding a user when you only know their email.

Find an Auth0 user by email address
- **list_clients**: Each client shows its client_id, name, type (regular web, SPA, M2M, native), allowed callbacks and creation date. Useful for auditing which applications can authenticate users.

List applications (clients) in Auth0
- **list_connections**: Each connection shows its name, strategy (auth0, google-oauth2, github, oidc, samlp, etc.), enabled clients and options. Use this to audit which identity providers your users can sign in with. Optionally filter by strategy type.

List identity connections in Auth0
- **list_logs**: Each log entry includes the event type (e.g. "s" = success login, "f" = failed login, "du" = user deleted, "sapi" = API operation, "limit_wc" = rate limit), date, IP, user agent and details. Optionally filter by event type and paginate.

List security and activity logs for your Auth0 tenant
- **list_organizations**: Organizations allow you to model B2B multi-tenancy. Each organization shows its ID, name, display name, branding and creation date.

List organizations in Auth0
- **list_roles**: Roles define permission sets that can be assigned to users. Each role shows its name, description, ID and creation date. Useful for auditing your RBAC (Role-Based Access Control) configuration.

List roles in Auth0
- **list_user_logs**: Each log entry includes the event type, date, IP address, user agent and details. Useful for security auditing and troubleshooting user issues.

List activity logs for a specific Auth0 user
- **list_users**: Each user shows their user_id, email, name, last login, identities (connection provider), blocked status and metadata. Optionally search with a query string (q parameter) using Lucene syntax (e.g. "email:*@example.com" or "name:John"). Supports pagination with page and per_page.

List users in your Auth0 tenant
- **update_user**: Provide the user_id and a JSON object with fields to change (e.g. {"email":"new@email.com","email_verified":true,"blocked":false,"user_metadata":{"theme":"dark"}}). Only provided fields will be updated.

Update an Auth0 user


## Installation & Usage

To install and use the **Auth0** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/auth0-alternative](https://vinkius.com/mcp/auth0-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

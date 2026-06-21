# Clerk MCP Server

Manage authentication and users via Clerk — track active sessions, monitor organizations, and manage invitations directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/clerk)

## Overview
**Category:** fort-knox
**Tools Count:** 8

## Description
Connect your **Clerk** account to any AI agent and take full control of your authentication and user management through natural conversation. Streamline how you monitor your user base and B2B organizations natively.

### What you can do

- **User Oversight** — List and retrieve details for all users in your application, including metadata and status natively
- **Session Intelligence** — Access and monitor all active user sessions across your platforms flawlessly
- **Organization Logistics** — List and manage B2B organizations and their member rosters securely
- **Invitation Tracking** — Access and review all pending and completed user invitations flawlessly
- **Allowlist Management** — List identifiers like emails and domains on your authentication allowlist flawlessly
- **Dashboard Visibility** — Retrieve a high-level summary of user counts and system health directly within your workspace

### How it works

1. Subscribe to this server
2. Enter your Clerk Secret Key (obtained from your dashboard API Keys)
3. Start managing your authentication from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — monitor user signups and verify session status using natural language
- **Customer Support** — quickly look up user profiles and organization memberships without opening the dashboard
- **Product Managers** — audit invitation success rates and active user counts straight from their chat interface
- **Operations Teams** — verify authentication allowlists and system health


## Available Tools
- **get_auth_dashboard_summary**: Retrieve a summary of user counts and system health
- **get_user_auth_details**: Get detailed information for a specific user
- **list_auth_allowlist**: List identifiers (emails, domains) on the authentication allowlist
- **list_clerk_clients**: List all tracking clients (browser/device instances)
- **list_sent_invitations**: List all pending and completed user invitations
- **list_clerk_organizations**: List all organizations (B2B) in the application
- **list_active_sessions**: List all active user sessions
- **list_clerk_users**: List all users in your Clerk application


## Installation & Usage

To install and use the **Clerk** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clerk](https://vinkius.com/mcp/clerk)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# CodeRabbit MCP Server

Manage AI-powered code reviews via CodeRabbit — list users, track PR review metrics, audit admin actions, and control seat assignments from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/coderabbit)

## Overview
**Category:** ai-frontier
**Tools Count:** 9

## Description
Connect your **CodeRabbit** organization to any AI agent and take full control of your AI-powered code review operations through natural conversation.

### What you can do

- **User Management** — List all organization members, filter by seat assignment or role, and inspect individual profiles
- **Seat Control** — Bulk assign or unassign CodeRabbit seats to enable or disable AI code reviews for team members
- **Role Administration** — Promote members to admin or demote admins to member role in bulk operations
- **PR Review Metrics** — Retrieve complexity scores, review times, and comment breakdowns for merged pull requests across any date range
- **Compliance Audit Logs** — Access tamper-resistant records of administrative actions for SIEM integration and compliance reporting
- **Configuration** — View and update seat assignment modes (automatic vs. manual)

### How it works

1. Subscribe to this server
2. Enter your CodeRabbit API Key from Organization Settings
3. Start managing your code review infrastructure from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Engineering Managers** — get instant visibility into team code review velocity and quality metrics
- **Platform Engineers** — automate seat management and role administration across large organizations
- **Compliance Officers** — query audit logs for administrative action reports without accessing the dashboard


## Available Tools
- **assign_seats**: Up to 500 user IDs per request.

Assign CodeRabbit seats to users
- **get_audit_logs**: Ideal for compliance reporting.

Retrieve organization audit logs
- **demote_users**: Demote users from admin to member role
- **get_seat_mode**: Get the current seat assignment mode
- **list_users**: Optionally filter by seat assignment status or role.

List all users in the CodeRabbit organization
- **get_metrics**: Useful for engineering productivity analysis.

Retrieve PR review metrics for a date range
- **promote_users**: Promote users to admin role
- **unassign_seats**: Does not delete user accounts.

Remove CodeRabbit seats from users
- **update_seat_mode**: Requires Enterprise plan.

Update the seat assignment mode


## Installation & Usage

To install and use the **CodeRabbit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coderabbit](https://vinkius.com/mcp/coderabbit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

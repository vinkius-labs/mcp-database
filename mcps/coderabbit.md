# CodeRabbit MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/coderabbit)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/coderabbit-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/coderabbit-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Manage AI-powered code reviews via CodeRabbit — list users, track PR review metrics, audit admin actions, and control seat assignments from any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CodeRabbit** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all team members who don't have a CodeRabbit seat assigned."

**🤖 AI Agent:**
> I found 4 unassigned members:

- **sarah.chen** (Member)
- **marcus.dev** (Member)
- **alex.ops** (Admin)
- **new.hire** (Member)

Would you like me to assign seats to all of them?

---

**👤 You:**
> "What were our code review metrics for March 2026?"

**🤖 AI Agent:**
> Here are the March 2026 review metrics:

- **Total PRs reviewed:** 142
- **Average complexity score:** 7.3/10
- **Average review time:** 4.2 minutes
- **Critical issues found:** 23
- **Suggestions accepted:** 67%

Would you like a breakdown by repository or author?

---

**👤 You:**
> "Show me the audit trail of admin actions from last week."

**🤖 AI Agent:**
> Audit log entries for the past 7 days:

1. **seat.assigned** — admin@company.com assigned 3 seats (Mar 28)
2. **role.promoted** — admin@company.com promoted marcus.dev to admin (Mar 29)
3. **config.updated** — admin@company.com changed review language to TypeScript-only (Mar 30)

All entries are tamper-resistant and SIEM-ready.


## Installation & Usage

To install and use the **CodeRabbit** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/coderabbit](https://vinkius.com/mcp/coderabbit)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

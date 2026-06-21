# Applied Epic MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/applied-epic)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/applied-epic-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/applied-epic-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [erp-operations](../categories/erp-operations.md)

Manage insurance clients, policies, and activities with Applied Epic — track renewals and compliance via AI.

## Description
The **Applied Epic MCP Server** provides a powerful natural language interface to your Applied Systems insurance management platform. Connect your Applied Epic account to your AI agent to gain real-time visibility into your client relationships, policy lifecycles, and agency workflows.

### Key Capabilities

- **Client Management** — List and search for clients, and access full demographic and compliance data.
- **Policy Lifecycle** — Track active and historical policies, including effective and expiration dates and current statuses.
- **Workflow Automation** — Create and manage activities (tasks/logs) directly from your chat interface to ensure consistent follow-ups.
- **Lines of Business** — Drill down into specific lines of business for any policy, such as Workers Comp or General Liability.
- **Attachment Oversight** — Find and manage documents, photos, and proof of insurance linked to your clients and policies.
- **Secure Integration** — Uses industry-standard OAuth 2.0 authentication to safely access your agency's data.

### Who is this for?

- **Insurance Agents** — Quickly check client information and policy details without navigating complex menus.
- **Account Managers** — Monitor upcoming renewals and ensure all compliance tasks are completed on time.
- **Agency Operations** — Streamline workflow tracking and documentation management using AI-assisted automation.


## Available Tools
- **create_activity**: Create a new activity record
- **get_account_check**: Verify Applied Epic account connection
- **get_client**: Get details for a specific client
- **get_policy**: Get details for a specific policy
- **list_activities**: List all activities (tasks/logs)
- **list_attachments**: List all file attachments
- **list_clients**: List all insurance clients in Applied Epic
- **list_lines**: g., Workers Comp, GL) for a specific policyId.

List lines of business for a policy
- **list_policies**: List all insurance policies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Applied Epic** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active insurance clients."

**🤖 AI Agent:**
> I've retrieved your active clients. You have 150 active clients, including 'Global Logistics Inc.' and 'Downtown Realty'.

---

**👤 You:**
> "Show me upcoming policy expirations for next month."

**🤖 AI Agent:**
> You have 12 policies expiring next month. The largest is 'Policy #ABC-123' for 'Global Logistics Inc.' expiring on the 15th.

---

**👤 You:**
> "Create an activity 'Renewal Follow-up' for client ID 'C998877'."

**🤖 AI Agent:**
> Activity 'Renewal Follow-up' has been successfully created and linked to client 'C998877'.


## Installation & Usage

To install and use the **Applied Epic** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/applied-epic](https://vinkius.com/mcp/applied-epic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

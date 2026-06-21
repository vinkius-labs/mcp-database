# Bitwarden MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bitwarden)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/bitwarden-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/bitwarden-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Manage Bitwarden organization resources—collections, events, groups, members, and policies—directly from your AI agent.

## Description
Connect your **Bitwarden** organization to any AI agent to audit security logs, manage collections, and oversee your team's access through natural conversation.

### What you can do

- **Collections Management** — List all organization collections to understand how vault items are organized and shared
- **Audit Trail & Events** — Retrieve detailed event logs to monitor administrative actions and security-related activities
- **Member Oversight** — List all members within your organization to verify access and seat utilization
- **Group Organization** — Query user groups to manage team-based permissions and access control
- **Policy Review** — Inspect active security and administrative policies to ensure compliance with organizational standards

### How it works

1. Subscribe to this server
2. Enter your Bitwarden Client ID and Client Secret
3. Start auditing your organization from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Administrators** — quickly audit event logs and verify policy compliance without navigating the web vault
- **IT Operations** — manage organization members and groups directly from automation workflows
- **Compliance Officers** — retrieve collections and access structures for security reporting


## Available Tools
- **list_collections**: List organization collections
- **list_events**: List organization event logs
- **list_groups**: List organization groups
- **list_members**: List organization members
- **list_policies**: List organization policies


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bitwarden** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all collections in my Bitwarden organization."

**🤖 AI Agent:**
> I've retrieved the collections for your organization. You have 4 active collections: 'Engineering-Shared', 'Marketing-Vault', 'Finance-Keys', and 'General-Access'. Would you like more details on any of these?

---

**👤 You:**
> "Show me the recent event logs for auditing."

**🤖 AI Agent:**
> Fetching the audit trail... I found the latest events. Recent actions include a policy update by 'admin@corp.com' and 3 new member invitations. Would you like me to list the specific details of the policy change?

---

**👤 You:**
> "Who are the current members of our Bitwarden organization?"

**🤖 AI Agent:**
> I've compiled the member list. There are currently 12 active members and 2 pending invitations. Notable users include 'Alice (Owner)', 'Bob (Admin)', and 'Charlie (User)'. Should I check their group assignments?


## Installation & Usage

To install and use the **Bitwarden** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bitwarden](https://vinkius.com/mcp/bitwarden)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Atlassian Crowd MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/atlassian-crowd)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/atlassian-crowd-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/atlassian-crowd-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Equip your AI agent to manage users, groups, and directory memberships via the Atlassian Crowd API.

## Description
Integrate **Atlassian Crowd**, the single sign-on and identity management application, directly into your AI workflow. Manage your corporate user directories, audit group memberships, and provision new accounts using natural language.

### What you can do

- **User Management** — List, search, and retrieve detailed profiles for active and inactive users.
- **Group Control** — Monitor security groups and manage organizational memberships seamlessly.
- **Account Provisioning** — Create new user accounts with full attribute definitions via chat.
- **Identity Auditing** — Search for users by attributes and verify directory-wide security restrictions.

### How it works

1. Connect the Atlassian Crowd integration to your AI assistant.
2. Authorize using your Crowd Base URL, Application Name, and Application Password.
3. Orchestrate your identity and access management through intuitive conversation.

### Who is this for?

- **IT Administrators** — Quickly audit user groups and reset or verify account statuses.
- **Security Teams** — Search for specific user attributes and monitor directory access patterns.
- **DevOps Engineers** — Provision and manage application-specific user accounts via chat.


## Available Tools
- **create_new_user**: Provision a new user account in Crowd
- **get_group_details**: Get details for a specific group
- **get_user_details**: Get full profile and attributes for a specific user
- **list_group_members**: List all users who are members of a specific group
- **list_all_groups**: List all security and organizational groups
- **list_inactive_users**: List all disabled or inactive user accounts
- **list_user_memberships**: List all groups a specific user belongs to
- **list_active_users**: List all active users managed in Crowd
- **search_users_by_name**: Search for users whose name starts with a prefix
- **search_users_by_attribute**: Search for users using a CQL-like restriction string


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Atlassian Crowd** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active users in the 'Internal Staff' directory."

**🤖 AI Agent:**
> I've retrieved 150 active users from the 'Internal Staff' directory. Highlights include 'admin', 'jsmith', and 'mjones'. Would you like to see the group memberships for any of them?

---

**👤 You:**
> "Which groups does user 'jsmith' belong to?"

**🤖 AI Agent:**
> User 'jsmith' is a member of 3 groups: 'jira-users', 'confluence-users', and 'engineering-leads'. Should I check his access permissions for a specific application?

---

**👤 You:**
> "Search for users with an email address ending in '@vinkius.com'."

**🤖 AI Agent:**
> I found 12 users with emails ending in '@vinkius.com', including 'renato@vinkius.com' and 'support@vinkius.com'. Would you like to see their full profile details?


## Installation & Usage

To install and use the **Atlassian Crowd** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/atlassian-crowd](https://vinkius.com/mcp/atlassian-crowd)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Forj MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/forj)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/forj-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/forj-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage community members, groups, and activity via AI agents with Forj (formerly Mobilize).

## Description
Connect your **Forj** (formerly Mobilize) account to any AI agent to automate your community management and member engagement through the Model Context Protocol (MCP). Forj provides a powerful platform for organizing professional communities into groups, tracking member activity, and facilitating seamless synchronization with external CRMs. This MCP server enables you to manage your groups, search for members, and oversee community interactions directly through natural conversation.

### Key Features

- **Member Discovery** — Search for community members by name or keywords, and find specific users instantly by their email address.
- **Group Management** — List all organizational groups, create new groups, and fetch detailed metadata for specific community segments.
- **Membership Control** — Assign existing members to specific groups and monitor pending membership requests awaiting approval.
- **Engagement Insights** — Retrieve detailed activity logs for specific members to understand their level of participation and interactions.
- **Invitation Tracking** — Monitor sent and pending community invitations to maintain a healthy growth pipeline.
- **System Monitoring** — Access account metadata and list active webhooks used for real-time community data synchronization.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Forj API Key and Secret Key (found in your platform settings)
3. Start managing your professional community directly from your favorite AI tools


## Available Tools
- **add_user_to_group**: Add member to group
- **create_group**: Create a new group
- **find_user**: Find user by email
- **get_account_details**: Get community account info
- **get_group**: Get group details
- **get_user_activity**: Get member activity log
- **list_group_members**: List members in a group
- **list_groups**: List community groups
- **list_invitations**: List sent invitations
- **list_pending_requests**: List group join requests
- **list_webhooks**: List active webhooks
- **search_users**: Search community members


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Forj** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all groups in my Forj community."

**🤖 AI Agent:**
> Retrieving groups... I found 4 organizational groups, including 'General Discussions' and 'VIP Members'.

---

**👤 You:**
> "Find the member profile for 'jane.doe@example.com'."

**🤖 AI Agent:**
> Searching... I found a profile for Jane Doe. She is a member of 3 groups and was last active yesterday.

---

**👤 You:**
> "Show me recent activity for user ID 'user_123'."

**🤖 AI Agent:**
> Retrieving activity log... User user_123 recently joined the 'Beta Testers' group and posted 2 comments.


## Installation & Usage

To install and use the **Forj** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/forj](https://vinkius.com/mcp/forj)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Engagespot MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/engagespot)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/engagespot-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/engagespot-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage multi-channel notifications via Engagespot — trigger workflows, manage user profiles, and handle notification preferences directly from any AI agent.

## Description
Connect your **Engagespot** account to any AI agent to orchestrate multi-channel notification workflows (Email, SMS, Push, In-app) through natural conversation.

### What you can do

- **Notification Workflows** — Trigger complex notification workflows using unique identifiers and custom data payloads via `send_notification`.
- **User Management** — Create, update, or delete user profiles and sync identifiers with your backend using `create_or_update_user` and `delete_user`.
- **Inbox Management** — List, delete, or clear notifications for specific users with `list_notifications` and `delete_all_notifications`.
- **Preference Control** — Retrieve and update notification preferences across different categories and channels using `get_preferences` and `update_preferences`.
- **Workflow Control** — Cancel active workflow runs using `cancel_workflow_run` with specific cancellation keys.

### How it works

1. Subscribe to this server
2. Enter your Engagespot API Key, API Secret, and Target User ID
3. Start sending and managing notifications from Claude, Cursor, or any MCP-compatible client

No more manual API calls to test your notification logic. Your AI acts as a communication orchestrator, ensuring your users get the right message at the right time.

### Who is this for?

- **Product Engineers** — instantly test notification workflows and user profile syncing without writing boilerplate code
- **Customer Success Teams** — check a user's notification history or update their preferences via simple commands
- **DevOps & Growth Hackers** — automate transactional messaging and monitor notification delivery directly from the terminal or IDE


## Available Tools
- **cancel_workflow_run**: Cancel a running workflow to prevent further messages
- **create_or_update_user**: Create a new user or update an existing user profile
- **delete_all_notifications**: Delete all notifications for the authenticated user
- **delete_notification**: Delete a specific notification by its ID
- **delete_user**: Delete a user from the workspace
- **get_preferences**: Get notification preferences for the authenticated user
- **list_notifications**: List notifications for the authenticated user
- **send_notification**: Send a notification by triggering a workflow
- **update_preferences**: Update notification preferences for the authenticated user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Engagespot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a 'new_order' notification to user_99 with data {"orderId": "12345"}."

**🤖 AI Agent:**
> I've triggered the 'new_order' workflow for user_99. The notification has been queued for delivery with the provided order data.

---

**👤 You:**
> "Update user 'dev_user_01' with email 'dev@company.com' and first name 'Alice'."

**🤖 AI Agent:**
> User 'dev_user_01' has been successfully updated. The profile now reflects the new email and first name in the Engagespot database.

---

**👤 You:**
> "List my recent notifications and then clear my inbox."

**🤖 AI Agent:**
> I've retrieved your notifications. You had 3 unread messages. As requested, I have now cleared your entire inbox using the delete all command.


## Installation & Usage

To install and use the **Engagespot** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/engagespot](https://vinkius.com/mcp/engagespot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

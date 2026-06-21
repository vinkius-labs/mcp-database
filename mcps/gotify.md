# Gotify MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gotify)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gotify-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gotify-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Send and receive push notifications via your own Gotify server — manage messages, applications, and clients directly through AI.

## Description
Connect your **Gotify** instance to any AI agent to streamline your notification workflows. Gotify is a self-hosted notification server, and this MCP server allows you to interact with its API using natural language.

### What you can do

- **Messaging** — Send push notifications with custom priorities and titles, or retrieve and delete existing messages from your stream.
- **Application Management** — Create, list, update, or delete Gotify applications to organize your notification sources and tokens.
- **Client Control** — Manage clients and tokens to authorize different devices or services to receive messages.
- **User Administration** — (Admin only) List or create users to manage access to your private Gotify instance.

### How it works

1. Subscribe to this server
2. Enter your Gotify URL and your Application or Client tokens
3. Start sending alerts or managing your server from Claude, Cursor, or any MCP client

### Who is this for?

- **DevOps Engineers** — automate alerts for CI/CD pipelines or server health checks directly from the terminal.
- **Developers** — test notification payloads and manage app tokens without leaving the code editor.
- **Home Automation Enthusiasts** — bridge your AI assistant with your self-hosted notification hub.


## Available Tools
- **change_password**: Change current user password
- **create_application**: Create a new application
- **create_client**: Create a new client
- **create_user**: Create a new user (Admin only)
- **delete_all_messages**: Delete all messages for the authenticated client
- **delete_application**: Delete an application
- **delete_client**: Delete a client
- **delete_message**: Delete a specific message
- **get_applications**: List all applications
- **get_clients**: List all clients
- **get_current_user**: Get current user details
- **get_health**: Get server health status
- **get_messages**: Requires GOTIFY_CLIENT_TOKEN.

Retrieve messages
- **get_plugin_config**: Get plugin configuration
- **get_plugin_display**: Get plugin display info
- **get_plugins**: List all plugins
- **get_users**: List all users (Admin only)
- **get_version**: Get server version info
- **send_message**: Requires GOTIFY_APP_TOKEN.

Send a message via Gotify
- **update_application**: Update an application
- **update_client**: Update a client
- **update_plugin_config**: Update plugin configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gotify** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a high-priority Gotify message titled 'System Alert' saying 'Disk space is low on Server A'."

**🤖 AI Agent:**
> I've sent the high-priority message (Priority 8) to your Gotify server. The message 'Disk space is low on Server A' has been pushed successfully.

---

**👤 You:**
> "List all my current Gotify applications and their descriptions."

**🤖 AI Agent:**
> I found 3 applications: 'Backup-Bot' (Status alerts), 'GitHub-Webhooks' (Repo updates), and 'Home-Monitor' (IoT sensors). Which one would you like to manage?

---

**👤 You:**
> "Get the last 5 messages from my Gotify server."

**🤖 AI Agent:**
> Retrieving your recent messages... I've found 5 messages. The most recent is 'Build Success' from 10 minutes ago. Would you like me to summarize the others?


## Installation & Usage

To install and use the **Gotify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gotify](https://vinkius.com/mcp/gotify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

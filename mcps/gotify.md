# Gotify MCP Server

Send and receive push notifications via your own Gotify server — manage messages, applications, and clients directly through AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/gotify)

## Overview
**Category:** communication-messaging
**Tools Count:** 22

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


## Installation & Usage

To install and use the **Gotify** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gotify](https://vinkius.com/mcp/gotify)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

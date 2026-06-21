# Pumble MCP Server

Bring your AI agent into your Pumble workspace — read channel history, post messages, create channels, and manage team communication seamlessly.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pumble)

## Overview
**Category:** collaboration-tools
**Tools Count:** 10

## Description
Connect your **Pumble** workspace to any AI agent and bring powerful automation directly to your team's communication hub.

### What you can do

- **Read & Manage Channels** — List all public and private channels, fetch detailed metadata, and dynamically create new discussion channels on the fly
- **Message Operations** — Retrieve conversation histories, post new messages, update typos, or delete outdated announcements seamlessly
- **Interactive Reactions** — Add emoji reactions to messages automatically to acknowledge requests without cluttering the chat
- **User Directory** — List all workspace users and pull detailed profiles (including emails and time zones) to ensure accurate tagging

### How it works

1. Subscribe to this server
2. Authorize via your Pumble API Key (generated in-app)
3. Start managing your communications directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Engineering Teams** — trigger automated status updates or bug reports directly into specific channels
- **Community Managers** — have your agent scan channels, organize discussions, and reply to common questions
- **Operations Leads** — provision new project channels instantly and broadcast identical messages across the workspace


## Available Tools
- **chat_add_reaction**: Adds an emoji reaction to a message
- **chat_delete_message**: This action is irreversible.

Deletes a message from a Pumble channel
- **chat_history_messages**: Retrieves recent messages from a channel
- **chat_post_message**: Specify the channel ID and the message text.

Sends a message to a Pumble channel
- **chat_update_message**: Updates a pre-existing message
- **create_chat_channel**: Specify name and whether it should be private.

Creates a new communication channel
- **get_channel_info**: Retrieves detailed information about a specific channel
- **get_user_info**: Retrieves detailed information for a specific user
- **list_all_channels**: Lists all public and private channels available in the workspace
- **list_workspace_users**: Lists all users in the Pumble workspace


## Installation & Usage

To install and use the **Pumble** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pumble](https://vinkius.com/mcp/pumble)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

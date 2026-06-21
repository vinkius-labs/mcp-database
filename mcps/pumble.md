# Pumble MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pumble)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pumble-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pumble-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration-tools](../categories/collaboration-tools.md)

Bring your AI agent into your Pumble workspace — read channel history, post messages, create channels, and manage team communication seamlessly.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pumble** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our active channels in Pumble."

**🤖 AI Agent:**
> I found 5 active channels in your workspace. The main ones are `#general`, `#dev-updates`, and `#marketing-q4`. Which one should I inspect?

---

**👤 You:**
> "Post a message in the #dev-updates channel stating that 'Deployment 2.1 is completed'."

**🤖 AI Agent:**
> Done! I've securely posted 'Deployment 2.1 is completed' to the `#dev-updates` channel.

---

**👤 You:**
> "Read the last 3 messages from #marketing-q4 and react to the last one with a 'thumbsup'."

**🤖 AI Agent:**
> Here's what was discussed in #marketing-q4: 
1. User A: 'Are the assets ready?'
2. User B: 'Yes, loaded in drive.'
3. User A: 'Perfect, deploying campaigns.'
I also successfully placed a 👍 reaction on User A's last message.


## Installation & Usage

To install and use the **Pumble** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pumble](https://vinkius.com/mcp/pumble)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

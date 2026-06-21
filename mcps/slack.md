# Slack MCP Server

Automate Slack messaging — send messages, search conversations, list channels and users directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/slack)

## Overview
**Category:** talk-to-me
**Tools Count:** 6

## Description
Transform your team communication into an AI-powered workflow with **Slack**, the world's leading workplace messaging platform. Your agent becomes a direct participant in your Slack workspace — sending messages, searching across channels, and reacting to conversations without you ever switching tabs.

### What you can do

- **Send Messages** — Post messages to any channel or DM, including threaded replies, using Slack's rich mrkdwn formatting.
- **Search Conversations** — Find messages across your entire workspace by keyword, sender, or channel using powerful search modifiers.
- **Browse Channels** — List all available channels with their topics, purposes, and member counts to understand your workspace structure.
- **Read Channel History** — Retrieve recent messages from any channel to catch up on conversations or audit activity.
- **Manage Users** — List workspace members with their roles, emails, statuses, and timezones.
- **React to Messages** — Add emoji reactions to specific messages for quick acknowledgments.

### How it works

1. Subscribe to this server
2. Enter your Slack Bot Token (from api.slack.com/apps → OAuth & Permissions)
3. Start managing your Slack workspace from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Team Leads** — broadcast updates, search for past decisions, and monitor channel activity without leaving your AI workflow.
- **Developers** — get notified, post deployment updates, and search for error reports across your engineering channels.
- **Operations Managers** — audit communication patterns, find specific discussions, and coordinate across multiple channels effortlessly.


## Available Tools
- **channels_list**: Returns public and private channels the bot has access to. Channel IDs are needed for sending messages or reading history.

List Slack channels in the workspace
- **channels_history**: Requires the channel ID (use channels_list to find it). Returns messages in reverse chronological order.

Get recent messages from a Slack channel
- **messages_send**: Requires the channel ID. Use channels_list to find available channels. Optionally specify thread_ts to reply in a thread.

Send a message to a Slack channel or DM
- **messages_search**: Searches message content, usernames, and channels. Results are sorted by most recent first.

Search for messages across the Slack workspace
- **users_list**: Returns user IDs, names, emails, and status. User IDs are needed for sending DMs or identifying message authors.

List users in the Slack workspace
- **reactions_add**: Requires the channel ID and the exact message timestamp (ts). Use channels_history to find message timestamps.

Add a reaction emoji to a Slack message


## Installation & Usage

To install and use the **Slack** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/slack](https://vinkius.com/mcp/slack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Twist MCP Server

Automate asynchronous communication workflows via Twist — manage workspaces, channels, threads, comments, and direct messages via any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/twist)

## Overview
**Category:** collaboration-tools
**Tools Count:** 10

## Description
Connect your **Twist** account to any AI agent and take full control of your team’s asynchronous, distraction-free dialogue through natural conversation.

### What you can do

- **Workspaces & Members** — Identify top-level organizations actively driving your team and find all associated workspace user accounts
- **Channels & Groups** — List open organizational categories holding specific deep-threaded discussions within your sub-department
- **Thread Execution** — Spark a new asynchronous discussion into a channel by writing full markup elements and posting deep remarks over an existing subject
- **Direct Messaging** — Access any active 1-on-1 conversations and directly parse long direct messages, modify recent text errors, or append comments rapidly

### How it works

1. Subscribe to this server
2. Enter your Twist API Token via the Developer Portal
3. Leverage your new communications assistant connecting securely from Claude, Cursor, or any MCP-compatible environment

No more switching contexts and scrambling to find important threads on standard messaging software. Twist’s architecture works seamlessly inside an agentic command center to let you focus.

### Who is this for?

- **Product Managers** — spin up new announcement threads with structured markdown summaries to specific channels
- **Engineering Teams** — auto-read debugging or release threads asynchronously skipping massive chat floods
- **Remote employees** — query your PM's 1-on-1 direct messages to catch up without an actual video-call


## Available Tools
- **create_comment**: Provide the thread_id and your message.

Posts a reply to an existing thread
- **send_direct_message**: Provide conversation_id and content.

Sends a private message to a specific conversation
- **create_thread**: Provide channel_id, title, and initial content.

Creates a new asynchronous discussion thread in a channel
- **list_channels**: Provide the workspace_id.

Lists all channels within a specific Twist workspace
- **list_direct_messages**: Provide the conversation_id.

Lists messages from a specific 1-on-1 direct conversation
- **list_threads**: Provide the channel_id.

Lists all conversation threads within a specific channel
- **list_workspace_users**: Lists all members of a specific workspace
- **list_workspaces**: Identify bounded Twist Workspaces actively driving Async Teams
- **update_direct_message**: Provide the message_id.

Modifies a previously sent direct message
- **update_thread**: Provide the thread_id.

Updates the title or content of an existing thread


## Installation & Usage

To install and use the **Twist** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/twist](https://vinkius.com/mcp/twist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

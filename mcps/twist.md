# Twist MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/twist)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/twist-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/twist-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [collaboration-tools](../categories/collaboration-tools.md)

Automate asynchronous communication workflows via Twist — manage workspaces, channels, threads, comments, and direct messages via any AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Twist** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Summarize all responses in the 'Q3 Pipeline' thread to see where we landed."

**🤖 AI Agent:**
> I've pulled 12 responses from the 'Q3 Pipeline' thread. The team decided to focus on Enterprise features and push the Analytics sprint to Q4. Sara mentioned the scoping doc is finalized. Should I prepare a comment indicating your alignment?

---

**👤 You:**
> "Post a new thread to the #bugs channel describing the latency issue in the EU region."

**🤖 AI Agent:**
> I've created a new thread titled '[SEV-2] Extremely high latency on EU DB shards'. The content is fully formatted, including your ping logs and initial analysis. Thread ID is 44351.

---

**👤 You:**
> "Check all my PMs with Mark and see if he shared his Figma files yesterday."

**🤖 AI Agent:**
> I've reviewed your direct messages with Mark. Yesterday afternoon, he mentioned sharing a link via Figma, and left the exact URL 'figma.com/design/xyz'. No physical attachments dot-zip were detected.


## Installation & Usage

To install and use the **Twist** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/twist](https://vinkius.com/mcp/twist)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

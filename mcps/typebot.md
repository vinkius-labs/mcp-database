# Typebot MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/typebot)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/typebot-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/typebot-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Build conversational forms and chatbot flows with a beautiful open-source visual editor that creates engaging user experiences.

## Description
Connect your **Typebot** account to any AI agent and simplify how you build, manage, and analyze your conversational assistants through natural conversation.

### What you can do

- **Bot Management** — List all typebots across your workspaces and folders, and retrieve detailed metadata and flow structures.
- **Deployment Control** — Publish the latest bot changes to production instantly without leaving your agent.
- **Result Analysis** — List and export user submissions and conversation results to track leads and performance.
- **Organization Oversight** — Manage workspaces and folders to keep your conversational projects structured.
- **Session Testing** — Programmatically start new chat sessions to verify bot logic and user experiences.

### How it works

1. Subscribe to this server
2. Enter your Typebot API Token (found in your account settings)
3. Start managing your conversational forms from Claude, Cursor, or any MCP client

### Who is this for?

- **Conversation Designers** — quickly verify bot logic and publish updates via simple AI commands.
- **Marketing & Sales Teams** — monitor incoming results and export lead data directly from the workspace.
- **Product Managers** — get instant bird's-eye views of bot performance and organization folders via the AI assistant.


## Available Tools
- **delete_typebot**: Permanently delete a typebot
- **get_typebot_details**: Essential for reviewing the bot logic.

Get details and structure for a specific typebot
- **list_typebots**: Can be filtered by a specific workspace ID.

List all conversational typebots
- **list_folders**: Folders are used to group related typebots.

List all folders in a workspace
- **list_typebot_results**: Essential for data analysis and lead export.

List collected user responses for a bot
- **list_workspaces**: Workspaces contain folders and bots.

List all accessible Typebot workspaces
- **publish_typebot**: Requires the unique bot ID.

Publish and deploy the latest bot changes
- **start_chat_session**: Useful for testing bot flows or automated interactions.

Programmatically start a new bot conversation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Typebot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all typebots in my current workspace."

**🤖 AI Agent:**
> I've retrieved your typebots. You have 3 active bots: 'Lead Gen Flow', 'Customer Survey v2', and 'Support Assistant'. Which one would you like to publish or analyze?

---

**👤 You:**
> "Show me the collected results for the 'Lead Gen Flow' bot."

**🤖 AI Agent:**
> I've fetched the results. There are 15 recent submissions including leads from 'John Doe' (john@example.com) and 'Sarah Smith'. Shall I retrieve the detailed answers for any of them?

---

**👤 You:**
> "Publish the latest changes for bot 'bot_10293'."

**🤖 AI Agent:**
> Success! The latest changes for bot bot_10293 have been published to production. Your conversational form is now up-to-date at its public URL.


## Installation & Usage

To install and use the **Typebot** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/typebot](https://vinkius.com/mcp/typebot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

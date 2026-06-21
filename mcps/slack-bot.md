# Slack Bot MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/slack-bot)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/slack-bot-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/slack-bot-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Control and manage your Slack workspace — audit channels, messages, and users via AI.

## Description
Empower your AI agent to orchestrate your entire workspace communication on **Slack**, the leading platform for team collaboration. By connecting your Slack bot to your agent, you transform complex workspace management into a natural conversation. Your agent can instantly list your channels, audit message history, and send updates without you ever touching a dashboard. Whether you are a community manager or a project lead, your agent acts as a real-time coordinator, ensuring your team is always informed and your communication data is organized.

### What you can do

- **Conversation Auditing** — List all public channels in your workspace and retrieve detailed metadata, including purpose and topics.
- **Messaging Intelligence** — Send and delete messages in any channel, and retrieve recent message history for real-time monitoring.
- **User Administration** — Query workspace member lists, check user profiles, and monitor real-time presence (active/away).
- **Channel Governance** — Autonomously join or leave public channels to keep your bot's scope relevant and efficient.
- **Operational Monitoring** — Quickly retrieve detailed channel and user information to maintain strict organizational control.

### How it works

1. Subscribe to this server
2. Enter your Slack Bot User OAuth Token
3. Start managing your Slack workspace through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — monitor project channels and send status updates straight from your workflow.
- **Community Managers** — verify member lists and audit message history without manual dashboard logins.
- **Support Teams** — perform rapid user status checks and send announcements directly from chat.
- **Operations Leads** — automate Slack data querying to orchestrate cross-functional communication smoothly.


## Available Tools
- **send_message**: Send a message to a Slack channel
- **delete_message**: Delete a message from Slack
- **get_channel_info**: Get details for a specific channel
- **get_user_info**: Get details for a specific user
- **join_channel**: Join a public channel
- **leave_channel**: Leave a Slack channel
- **list_channels**: List Slack channels
- **list_users**: List all users in the workspace
- **get_history**: Get message history for a channel
- **get_presence**: Check if a user is active or away


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Slack Bot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all public channels in my Slack workspace."

**🤖 AI Agent:**
> I've retrieved your public channels. You have 5 active channels, including #general, #marketing, and #dev-updates. Which one would you like to audit for history?

---

**👤 You:**
> "Send 'Good morning team!' to #general."

**🤖 AI Agent:**
> Message delivered! I've sent your greeting to #general (ID: C12345). The message is now visible to all members.

---

**👤 You:**
> "Check if user ID U12345 is currently active."

**🤖 AI Agent:**
> Checking presence... User U12345 is currently 'active'. I can retrieve their full profile details if you'd like.


## Installation & Usage

To install and use the **Slack Bot** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/slack-bot](https://vinkius.com/mcp/slack-bot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

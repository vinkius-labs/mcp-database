# Slack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/slack-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Manage channels, users, and send messages on Slack with AI agents.

## Description
Connect your **Slack** workspace to any AI agent to automate your team communication and collaboration. Slack provides a premier platform for business messaging, and this integration allows you to retrieve channel info, send messages, and search through conversational history through natural conversation.

### What you can do

- **Communication Orchestration** — Post instant messages to channels or direct conversations and manage team threads programmatically.
- **Channel & User Management** — List all available channels and retrieve detailed member profile metadata directly from the AI interface.
- **Search & Discovery Intelligence** — Search through messages and retrieve channel histories to stay informed on team discussions via natural language.
- **Presence & Status Tracking** — Access user presence metadata and monitor team availability to ensure optimal collaboration.
- **Operational Monitoring** — Test authentication and monitor workspace health to ensure reliable connectivity between Slack and your AI workflows.

### How it works

1. Subscribe to this server
2. Enter your Slack Bot User OAuth Token (xoxb-...) from your app settings
3. Start managing your team communications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Project Managers** — quickly post updates and retrieve team discussion points without switching between channels.
- **Support Teams** — automate the retrieval of user details and monitor support channels via natural conversation.
- **Operations Managers** — streamline the delivery of notifications and coordinate team communications directly within the chat.


## Available Tools (11)
- **list_pins**: List all pinned messages in a channel
- **list_reactions**: Get reactions on a specific message
- **check_connection**: Verify API access
- **get_channel_details**: Get metadata for a channel
- **get_channel_history**: List recent messages
- **get_user_presence**: Check if a user is online
- **get_user_profile**: Get details for a user
- **list_channels**: List public channels
- **list_users**: List workspace members
- **send_message**: Send a message to a channel
- **search_messages**: Search for messages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Slack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Post an update to the #general channel: 'The new feature is live!'."

**🤖 AI Agent:**
> Message posted successfully! I've sent the update to the #general channel in your Slack workspace.

---

**👤 You:**
> "Show me the activity summary for all channels with message volumes and active participants this week."

**🤖 AI Agent:**
> Activity across 24 channels this week. Most active: #engineering (456 messages, 18 participants), #general (345, 42 participants), #product (234, 12 participants), #support (189, 8 participants), #sales (156, 14 participants). Quietest: #announcements (3 messages), #random (23). Total messages: 2,340. Active users: 67 of 85 (78.8%). Peak hours: 10-11 AM and 2-3 PM. Threads: 234 created, avg 4.2 replies. Reactions: 1,890 total, most used: 👍 (456), 🎉 (234), ❤️ (189). Files shared: 89.

---

**👤 You:**
> "Post a message to the #engineering channel announcing the deployment freeze for next week."

**🤖 AI Agent:**
> Message posted to #engineering. Content: "🚨 *Deployment Freeze Notice* 🚨\n\nTeam, we have a deployment freeze from Monday May 19 through Friday May 23 for the quarterly release preparation. All PRs must be merged by Friday EOD. Emergency hotfixes only during the freeze window. Please coordinate with @release-team for any exceptions.\n\n📋 Freeze checklist: https://wiki.internal/release-prep\n🗓 Release date: May 26". Message ID: msg_1716234567. Reactions received within 5 minutes: 12 (👍 8, 👀 4). Thread reply from @sarah: "Got it, finishing my PR today."


## ❓ FAQ

**Q: How do I find my Slack Bot User OAuth Token?**
Log in to [**Slack API**](https://api.slack.com/apps), select your app, and navigate to **OAuth & Permissions**. You will find the token starting with `xoxb-` under the **OAuth Tokens for Your Workspace** section.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/slack-alternative](https://vinkius.com/mcp/slack-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Slack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `slack-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Slack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "slack-alternative": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

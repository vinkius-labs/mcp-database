# Mattermost MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mattermost)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Collaborate securely with an open-source messaging platform that gives your team full control over data and deployment.

## Description
Connect your **Mattermost** workspace to any AI agent and manage team collaboration through natural conversation.

### What you can do

- **Messaging** — Send, read, and reply to messages in channels and DMs
- **Channel Management** — Create, join, and archive channels
- **Thread Tracking** — Browse message threads and ongoing discussions
- **User Management** — View user profiles, roles, and online status
- **Search** — Search for messages, files, and users across the workspace
- **Webhooks** — Trigger actions and monitor incoming webhooks

### How it works

1. Subscribe to this server
2. Enter your Mattermost Base URL and Access Token
3. Start managing your workspace from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps** — automate alerts and incident response channels
- **Engineering Teams** — integrate code deployments with chat
- **Community Managers** — manage large open-source communities


## Available Tools
- **create_new_channel**: Create a channel
- **post_message**: Send chat message
- **get_server_config**: Check server settings
- **get_my_profile**: Get user info
- **test_server_ping**: Check API health
- **get_team_details**: Get team info
- **list_team_channels**: List team channels
- **list_channel_posts**: Get channel history
- **list_system_roles**: List access roles
- **list_teams**: List your teams
- **list_server_users**: List all users
- **list_incoming_webhooks**: Get event configs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mattermost** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show unread messages in the #deployments channel."

**🤖 AI Agent:**
> #deployments: 3 new messages. 1) @bot: 'Deploying v2.4.1 to Production 🚀' (10 min ago). 2) @mike: 'Monitoring CPU usage...' (8 min). 3) @bot: 'Deploy successful ✅ All checks passed' (2 min ago).

---

**👤 You:**
> "Send a message to the #engineering channel announcing the meeting."

**🤖 AI Agent:**
> Message posted! ✅ Channel: #engineering. Content: 'Hey team! Just a reminder that our all-hands meeting starts in 15 minutes. See you there! @channel'. Message ID: msg_8901.

---

**👤 You:**
> "Search for 'API rate limit' and show thread replies."

**🤖 AI Agent:**
> Found 1 matching thread in #backend. Original (Apr 12): 'We are hitting the API rate limit on the third-party integration.' Replies: 4. @sarah: 'I will increase the backoff time.' @mike: 'Done, PR #45 merged.' @sarah: 'Metrics look stable now ✅'.


## ❓ FAQ

**Q: Can I read messages and reply to threads?**
Yes. Browse channel history, read specific threads, and post replies or new messages with markdown formatting.

**Q: How does Mattermost authentication work?**
Mattermost requires your instance's **Base URL** and a Personal **Access Token** for Bearer authentication.

**Q: Can I manage channels and users?**
Yes. Create new public/private channels, invite users, and check their online status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mattermost](https://vinkius.com/mcp/mattermost)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mattermost** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mattermost` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mattermost** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mattermost": {
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

# Slack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/slack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Automate Slack messaging — send messages, search conversations, list channels and users directly from any AI agent.

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


## Available Tools (6)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Slack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all channels in my Slack workspace."

**🤖 AI Agent:**
> I found 12 channels in your workspace. The most active ones are #general (45 members), #engineering (28 members), and #product (19 members). Would you like to read recent messages from any of them?

---

**👤 You:**
> "Post a message in #engineering: 'Deploy v2.4.1 is live on production 🚀'"

**🤖 AI Agent:**
> Message posted successfully to #engineering: 'Deploy v2.4.1 is live on production 🚀'. Would you like me to also react with a ✅ emoji?

---

**👤 You:**
> "Search for messages about 'API outage' from last week."

**🤖 AI Agent:**
> I found 8 messages mentioning 'API outage'. The first report came from @alex in #incidents at 2:34 PM on Monday. The root cause was identified as a database connection pool exhaustion. Would you like to see the full thread?


## ❓ FAQ

**Q: How do I get started with Slack MCP?**
Subscribe, then create a Slack App at **api.slack.com/apps → Create New App**. Go to **OAuth & Permissions**, add the required bot scopes (channels:read, chat:write, search:read, users:read), install the app to your workspace, and paste the **Bot User OAuth Token** (starts with xoxb-) here. No code, no webhooks — just connect and go.

**Q: Can my AI agent send messages and reply in threads?**
Yes. Your agent can post to any channel the bot has been invited to — including threaded replies. Just say 'post in #engineering that the deploy is complete' or 'reply in the thread about the bug fix'. It supports Slack's full mrkdwn formatting including bold, links, code blocks, and mentions.

**Q: How can I find a specific conversation from last week?**
Tell your agent to search for it — 'find messages about the Q3 budget review' or 'search for messages from @sarah about the client proposal'. The agent uses Slack's search API with support for modifiers like from:user, in:channel, and date ranges. No more scrolling through channels — your agent retrieves the exact messages you need.

**Q: Can I manage multiple channels and monitor team activity?**
Absolutely. List all channels to get an overview of your workspace structure, read history from specific channels to audit conversations, and check team member profiles, statuses, and timezones. Perfect for distributed teams, engineering organizations, and operations managers who need a bird's-eye view of communication across dozens of channels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/slack](https://vinkius.com/mcp/slack)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `slack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Slack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "slack": {
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

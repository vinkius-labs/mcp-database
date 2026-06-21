# Pumble MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pumble)
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


## ❓ FAQ

**Q: How do I securely obtain my API Key?**
Installation in Pumble is unique. In your workspace, click **+ Add apps** in the left sidebar, find the **API** addon, and install it. After doing so, go to any chat input box in Pumble and type `/api-keys generate`. A private, ephemeral message will appear containing your secret token. Paste that token here.

**Q: Can my AI automatically reply to unread issues?**
Yes. You can instruct your agent to regularly fetch messages from a specific channel (`chat_history_messages`). The agent can evaluate questions, generate answers based on your knowledge base, and then use `chat_post_message` to post the solution back to the team instantly.

**Q: Is it possible for the AI to react with emojis?**
Absolutely. It uses the `chat_add_reaction` functionality. A common use case is having the agent process a batch of tickets reported in Pumble, and instruct it to leave a '✅' checkmark reaction on the original message to signify that work is complete.

**Q: What happens if a bot message has a typo?**
Unlike standard webhooks, this integration provides full bidirectional control. If your AI posted something incorrect, simply ask it to update its previous message. It will fetch its message ID and push a new payload using the `chat_update_message` tool instantly without leaving double messages.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pumble](https://vinkius.com/mcp/pumble)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pumble** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pumble` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pumble** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pumble": {
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

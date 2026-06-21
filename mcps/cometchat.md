# CometChat MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cometchat)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Enable your AI agent to manage chat users, groups, and messages via the CometChat API.

## Description
Connect your AI assistant to **CometChat**, the communication platform providing chat, voice, and video capabilities for applications.

### What you can do

- **User Management** — List registered users, check online status, and retrieve user profiles.
- **Group Operations** — Create, list, and manage chat groups with different privacy settings.
- **Message History** — Retrieve conversation histories for users or groups and search past messages.

### How it works

1. Add the CometChat integration to your AI toolset.
2. Provide your App ID, Region, and API Key from the CometChat dashboard.
3. Manage your chat infrastructure via natural language commands.

### Who is this for?

- **Product Managers** — Check user activity and group usage without digging through dashboards.
- **Support Engineers** — Debug message delivery issues by inspecting conversation logs.
- **Developers** — Test chat features and verify group configurations directly from chat.


## Available Tools
- **create_group**: Create a new group in CometChat
- **create_user**: Create a new user in CometChat
- **deactivate_user**: Deactivate a user instead of deleting them
- **delete_user**: Permanently delete a user from CometChat
- **get_group_details**: Retrieve details of a specific group
- **get_user**: Retrieve detailed information about a specific user
- **list_groups**: Retrieve a list of groups from CometChat
- **list_messages**: Retrieve chat history messages
- **list_users**: Retrieve a list of users from CometChat
- **send_message**: Send a text message to a user or group


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CometChat** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the first 20 users in CometChat."

**🤖 AI Agent:**
> Here are the first 20 users:
1. 'alice' — Alice Johnson (online)
2. 'bob' — Bob Smith (offline, last seen 2h ago)
3. 'carlos' — Carlos López (online)
...
Would you like to check message history for any user?

---

**👤 You:**
> "Create a public group named 'Marketing Team' with GUID 'marketing-team'."

**🤖 AI Agent:**
> Group created successfully!
- Name: Marketing Team
- GUID: marketing-team
- Type: Public
- Members: 0
Would you like to add members to this group?

---

**👤 You:**
> "Retrieve the conversation history between users 'alice' and 'bob'."

**🤖 AI Agent:**
> Fetched 50 messages between Alice and Bob. The latest message from Alice is: 'I will send the reports tomorrow.' Sent at 10:45 AM today.


## ❓ FAQ

**Q: How do I get my CometChat API credentials?**
Log in to the CometChat dashboard at app.cometchat.com. Your App ID, Region, and API Key are displayed on the app overview page.

**Q: What is the difference between UID and GUID?**
UID (User ID) is the unique identifier for a user. GUID (Group ID) is the unique identifier for a group. Both are used to target specific resources in the API.

**Q: Can I send files with this integration?**
The current version supports text messages. File and media sending may be added in future updates.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cometchat](https://vinkius.com/mcp/cometchat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CometChat** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cometchat` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CometChat** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cometchat": {
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

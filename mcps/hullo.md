# Hullo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/hullo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage coworking spaces with desk bookings, member check-ins, and community engagement tools for modern workspaces.

## Description
Connect your **Hullo** account to any AI agent and manage member communications through natural conversation.

### What you can do

- **Member Management** — List all members, create new member profiles with contact details, and inspect individual member records
- **Direct Messaging** — Send messages to members with customizable content and message types
- **Conversation Tracking** — Browse all conversations and inspect individual threads with full message history

### How it works

1. Subscribe to this server
2. Enter your Hullo API Key from your account settings
3. Start managing communications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Community Managers** — send messages, manage member profiles, and track conversations without switching to the dashboard
- **Customer Success Teams** — communicate with customers, onboard new members, and review conversation histories
- **Operations Teams** — manage member databases and automate communication workflows through AI


## Available Tools
- **create_member**: Pass member data as a JSON string.

Create a new member
- **get_conversation**: Get conversation details
- **get_member**: Get member details
- **list_conversations**: List all conversations
- **list_members**: List all members
- **send_message**: Pass message data as a JSON string.

Send a message to a member


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Hullo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all members and send a welcome message to the newest one."

**🤖 AI Agent:**
> 42 members total. Newest: Ana Costa (member_042, ana@example.com, joined today). Other recent: James Rodriguez (member_041, joined yesterday), Lisa Park (member_040, joined 3 days ago). Welcome message sent! ✅ To: Ana Costa (member_042). Content: 'Welcome to our community, Ana! We're glad to have you. Feel free to reach out if you have any questions.' Message type: welcome. Delivery: confirmed. Would you like to view conversations or create another member?

---

**👤 You:**
> "Show all active conversations and the full thread for the latest one."

**🤖 AI Agent:**
> 18 active conversations. Latest: Conversation with Ana Costa (conv_089, started 30 min ago, 3 messages). Thread: [System 30 min ago]: Welcome message delivered. [Ana 20 min ago]: 'Thanks! Quick question — how do I set up my profile preferences?' [You 10 min ago]: 'You can access profile settings from the menu in the top-right corner. Let me know if you need help!' Other recent: Conv with James Rodriguez (conv_088, 5 messages, last activity 2 hours ago). Conv with Lisa Park (conv_087, 8 messages, last activity yesterday). Would you like to reply to Ana or view another conversation?

---

**👤 You:**
> "Create a new member for 'Carlos Mendes' and send him a welcome message."

**🤖 AI Agent:**
> Member created! Name: Carlos Mendes, Email: carlos@example.com, Phone: +55 11 9876-5432, ID: member_043. You now have 43 members. Welcome message sent! ✅ To: Carlos Mendes (member_043). Content: 'Welcome to our community, Carlos! We're excited to have you aboard. Here are some resources to get you started...' Delivery: confirmed. A new conversation has been created (conv_090). Would you like to view his profile or list all conversations?


## ❓ FAQ

**Q: Can I send messages to members through the AI agent?**
Yes. The `send_message` tool sends a direct message to a member. Provide a JSON payload with the `member_id`, `content` (the message text), and `type` (message type). Use `list_members` first to find the member ID.

**Q: Can I view the full conversation history with a member?**
Yes. Use `list_conversations` to see all active conversations, then `get_conversation` with a specific conversation ID to retrieve the full message thread including sender, timestamp, and content for each message.

**Q: Can I create new member profiles and manage their contact information?**
Yes. Use `create_member` with a JSON payload containing `first_name`, `last_name`, `email`, `phone`, and other contact details. Use `list_members` to browse existing members and `get_member` to inspect a specific profile.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/hullo](https://vinkius.com/mcp/hullo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Hullo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `hullo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Hullo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "hullo": {
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

# Dashly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dashly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Convert more website visitors with targeted pop-ups, live chat triggers, and automated lead nurturing sequences.

## Description
Connect your **Dashly** account to any AI agent and take full control of your conversational marketing and user tracking workflows through natural conversation.

### What you can do

- **User Lifecycle Orchestration** — List and manage your entire high-fidelity user database programmatically, retrieving detailed profile metadata and custom property updates
- **Conversational Intelligence** — Query active chat sessions, retrieve high-fidelity message history, and send instant replies directly through your agent
- **Event Tracking Architecture** — Programmatically record custom user actions (e.g., 'Pricing Viewed') to maintain a perfectly coordinated audit trail of customer behavior
- **Channel Optimization** — Access your complete directory of communication channels to coordinate your engagement strategy across multiple touchpoints
- **Operational Monitoring** — Verify account-level API connectivity and monitor user activity trends directly through your agent for instant performance reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Auth Token** from your Dashly dashboard (Settings > Integrations > API Keys)
3. Start orchestrating your customer engagement from Claude, Cursor, or any MCP client

No more manual toggling between chat tabs or missing critical user events. Your AI acts as your dedicated engagement coordinator and behavioral architect.

### Who is this for?

- **Customer Support Leads** — instantly retrieve user history and reply to conversations using natural language commands
- **Marketing Operations** — track custom events and segment users without leaving your creative workspace
- **Product Managers** — monitor user property updates and engagement health through simple AI queries


## Available Tools (8)
- **send_reply**: Send a reply to a conversation
- **set_user_props**: Set custom properties for a user
- **track_event**: Track a custom event for a user
- **get_conversation**: Get details for a specific conversation
- **get_user_details**: Get details for a specific user
- **list_channels**: List communication channels
- **list_conversations**: List recent conversations
- **list_users**: List all Dashly users


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dashly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active chat conversations in my Dashly account."

**🤖 AI Agent:**
> I've retrieved your conversations. You currently have 5 active sessions, including 'Conversation #123' with John Doe and 'Lead Inquiry'. Would you like the detailed high-fidelity message history for any of them?

---

**👤 You:**
> "Track event 'Newsletter Signup' for user 'user_456'."

**🤖 AI Agent:**
> Event orchestrated! I've successfully recorded the 'Newsletter Signup' action for user 456. This event is now active in their high-fidelity behavioral profile. Need help updating any custom properties for them?

---

**👤 You:**
> "Get the profile metadata for user ID 'user_789'."

**🤖 AI Agent:**
> User profile orchestrated! I've retrieved the metadata for user 789. They are currently tagged as a 'VIP' and have 10 custom properties set. Shall I list the detailed high-fidelity history for this lead?


## ❓ FAQ

**Q: How do I find my Dashly Auth Token?**
Log in to your account, navigate to **Settings** > **Integrations** > **API Keys**, and copy your unique Auth Token.

**Q: Can I record custom user events via AI?**
Yes! The `track_event` tool allows your agent to log specific user actions programmatically by providing the user ID and event name.

**Q: How do I check active chat sessions?**
Use the `list_conversations` tool to retrieve a comprehensive directory of all current chat interactions and their high-fidelity metadata.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dashly](https://vinkius.com/mcp/dashly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dashly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dashly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dashly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dashly": {
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

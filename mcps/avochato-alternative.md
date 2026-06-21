# Avochato MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/avochato-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Text your customers on the channels they prefer with two-way business messaging that integrates into your existing workflows.

## Description
Connect your **Avochato** account to any AI agent and take full control of your high-fidelity business texting and customer engagement workflows through natural conversation.

### What you can do

- **Multichannel Messaging Orchestration** — Instantly dispatch high-fidelity SMS and MMS messages to customers and leads with automatic link and media handling
- **Relationship Intelligence** — Sync and manage your entire business contact directory programmatically, retrieving detailed high-fidelity profiles and interaction history
- **Ticket Lifecycle Management** — Organize team workflows by creating and updating tickets, monitoring status transitions, and assigning ownership in real-time
- **Communication Architecture** — Access complete conversation logs and message threads to maintain high-fidelity oversight of your organizational digital voice
- **Operational Monitoring** — Configure real-time webhooks for incoming messages and retrieve account-level metadata directly through your agent for instant reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Auth ID** and **Auth Secret** from your Avochato settings (API Access)
3. Start automating your customer notifications and engagement from Claude, Cursor, or any MCP client

No more manual logging of text interactions or missing critical client messages. Your AI acts as your dedicated communication coordinator and support architect.

### Who is this for?

- **Sales Teams** — instantly send personalized order updates and follow-up messages using natural language commands
- **Support Agents** — manage high-volume ticket queues and update customer statuses without leaving your workspace
- **Marketing Managers** — orchestrate SMS broadcasts and monitor audience engagement through simple AI queries


## Available Tools (12)
- **create_contact**: Create a new contact
- **create_webhook**: Create a new webhook
- **delete_webhook**: Delete a webhook
- **get_contact**: Get contact details
- **get_account_info**: Get account identity
- **list_contacts**: List SMS contacts
- **list_messages**: List SMS/MMS messages
- **list_tickets**: List conversation tickets
- **list_webhooks**: List active webhooks
- **send_message**: Send an SMS/MMS
- **update_contact**: Update contact info
- **update_ticket**: Update ticket status


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Avochato** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a SMS 'Your order is ready!' to '+14155550123'."

**🤖 AI Agent:**
> Message dispatched! I've successfully sent the notification to +14155550123 via Avochato. The status is currently 'Sent'. Shall I alert you as soon as the recipient replies?

---

**👤 You:**
> "List all active tickets in my Avochato inbox."

**🤖 AI Agent:**
> I've retrieved your inbox. You currently have 5 active tickets, including @user1 and @user2. One ticket is flagged as high priority. Would you like the detailed conversation history for any of these?

---

**👤 You:**
> "Update ticket '12345' status to 'closed'."

**🤖 AI Agent:**
> Ticket updated! I've successfully closed ticket 12345 in your organization's workflow. It's now moved to the historical records. Need help with any other organizational tasks?


## ❓ FAQ

**Q: How do I find my Avochato API credentials?**
Log in to your account, navigate to **Settings** > **API Access**, and copy your unique Auth ID and Auth Secret.

**Q: Can I send media files via AI?**
Yes! The `send_message` tool accepts a `media_url` parameter, allowing your agent to dispatch high-fidelity MMS content programmatically.

**Q: How do I check active tickets?**
Use the `list_tickets` tool to retrieve your complete directory of active and pending support tickets directly through your agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/avochato-alternative](https://vinkius.com/mcp/avochato-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Avochato** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `avochato-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Avochato** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "avochato-alternative": {
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

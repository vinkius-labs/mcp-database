# Heymarket MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/heymarket)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Text customers from a shared business number with two-way SMS, scheduled messages, and CRM integrations for team communication.

## Description
Connect your **Heymarket** account to any AI agent and take full control of your business text messaging and SMS workflows through natural conversation.

### What you can do

- **SMS Orchestration** — Send and receive text messages programmatically across your business numbers
- **Shared Inbox Management** — Monitor active chat threads and manage team-based conversations in real-time
- **Contact Relationships** — Create and update detailed contact profiles to maintain a high-fidelity customer database
- **Team Collaboration** — Retrieve staff member directories and manage assignments for inbound message routing
- **Message Monitoring** — Track outbound message delivery status and retrieve complete conversation histories for audit

### How it works

1. Subscribe to this server
2. Retrieve your API Key from your Heymarket Dashboard (Administration > Integrations > API)
3. Start managing your SMS communications from Claude, Cursor, or any MCP client

No more manual texting from a mobile device or switching tabs to check your inbox. Your AI acts as your dedicated communication coordinator.

### Who is this for?

- **Sales Teams** — automate lead qualification and follow-ups via SMS using natural language queries
- **Customer Support** — manage high-volume text queues and update contact details without leaving your workspace
- **Operations Managers** — monitor team response times and coordinate staff assignments across shared inboxes


## Available Tools (9)
- **create_contact**: Register a new contact
- **get_chat_history**: Get conversation history
- **get_message_details**: Get details for a message
- **list_active_chats**: List active conversations
- **list_contacts**: Supports filtering by phone number.

List Heymarket contacts
- **list_team_members**: List Heymarket workspace members
- **send_sms_message**: Requires member_id and to_number.

Send an SMS or MMS message
- **update_chat_status**: Modify chat state or assignment
- **update_contact_profile**: Modify an existing contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Heymarket** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS 'Your order is ready!' to '+15551234567' using member 'M123'."

**🤖 AI Agent:**
> Message sent! I've successfully delivered your update to '+15551234567' via Heymarket. The message ID is 'msg_98765'.

---

**👤 You:**
> "List all active chat conversations from the shared inbox."

**🤖 AI Agent:**
> I've retrieved 5 active threads. Notable conversations include 'Support Request #402' and 'New Lead Inquiry'. Would you like to read the latest messages for any of these?

---

**👤 You:**
> "Update contact 'C456' with first name 'John' and add a note."

**🤖 AI Agent:**
> Contact 'C456' updated! I've set the first name to 'John' and added your note to their profile in Heymarket. Their profile is now up to date.


## ❓ FAQ

**Q: How do I generate an API Key for Heymarket?**
Log in to your Heymarket account, navigate to **Administration** > **Integrations** > **API**, and click **Create Key** to generate your unique identifier.

**Q: Can the agent send images or media via SMS (MMS)?**
Yes! If you provide a public media URL in the message tool, Heymarket will automatically deliver it as an MMS to the recipient.

**Q: How do I find the correct Member ID to send messages from?**
Use the `list_team_members` tool. It will return all staff members in your workspace along with their unique `id`, which you can then use as the sender.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/heymarket](https://vinkius.com/mcp/heymarket)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Heymarket** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `heymarket` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Heymarket** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "heymarket": {
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

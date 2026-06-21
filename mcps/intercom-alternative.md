# Intercom MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/intercom-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Connect with customers through AI-powered chat, targeted messages, and product tours that drive engagement and reduce churn.

## Description
Connect your **Intercom** account to any AI agent and manage customer communications through natural conversation.

### What you can do

- **Contact Management** — List contacts, inspect profiles with tags and custom attributes, and search by email or name
- **Conversation Tracking** — Browse all conversations, inspect threads with full message history, and monitor status
- **Messaging** — Send messages to contacts and reply to active conversations
- **Company Records** — List companies, inspect profiles with user counts and custom data
- **CRM Search** — Search contacts and companies using Intercom's query syntax
- **Admin Management** — List all team members and their roles

### How it works

1. Subscribe to this server
2. Enter your Intercom Access Token from the developer hub
3. Start managing customers from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Support Teams** — manage conversations and reply to customers through AI
- **Sales Teams** — search leads, inspect company profiles, and track engagement
- **Customer Success** — monitor conversations and contact activity


## Available Tools
- **create_contact**: Register a new contact
- **create_conversation**: Start a new conversation
- **get_contact_details**: Get details for a contact
- **get_conversation_details**: Get conversation history
- **list_admins**: List workspace admins
- **list_help_articles**: List help center articles
- **list_contacts**: List Intercom contacts
- **list_conversations**: List recent conversations
- **list_data_attributes**: List custom attributes
- **list_segments**: List workspace segments
- **reply_to_conversation**: Reply to a conversation
- **search_contacts**: Search contacts with filters


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Intercom** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all open conversations and the contact details for the most recent one."

**🤖 AI Agent:**
> 18 open conversations. Latest: Conv #4521 — 'Ana Costa' (ana@company.com) asking about pricing, 10 min ago, 3 messages. Contact: Ana Costa, Company: TechCorp (50 employees), Plan: Pro, Last seen: 2 min ago, Tags: enterprise-lead. Would you like to reply or search contacts?

---

**👤 You:**
> "Search for all contacts at acmecorp.com and list their companies."

**🤖 AI Agent:**
> 4 contacts at acmecorp.com: John Smith (CTO), Lisa Park (VP Eng), Mike Torres (Director), Sarah Chen (PM). Company: Acme Corp — 250 employees, Enterprise plan, $12K MRR, 4 active users, last activity today. Tags: enterprise, high-value. Would you like to send a message or view conversations?

---

**👤 You:**
> "Send a follow-up message to Ana Costa and list all team admins."

**🤖 AI Agent:**
> Message sent! ✅ To: Ana Costa. Content: 'Hi Ana, following up on your pricing question. Our Pro plan at $99/mo includes all features you mentioned. Happy to schedule a demo!' Team admins: 6. Sarah (Owner), Mike (Admin), Lisa (Admin), James (Member), Chen (Member), David (Member).


## ❓ FAQ

**Q: Can I search for contacts and send messages through the AI agent?**
Yes. Use `search_contacts` to find contacts by email, name, or custom attributes. Then use `send_message` to send a message to a specific contact, or reply to an active conversation thread.

**Q: Can I view full conversation histories?**
Yes. `list_conversations` shows all conversations with status. Use `get_conversation` with a conversation ID to retrieve the full message thread including sender, timestamps, and content.

**Q: What type of Intercom token do I need?**
You need an **Access Token** from a Private App in the Intercom Developer Hub. This provides scoped API access with Bearer authentication against `api.intercom.io`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/intercom-alternative](https://vinkius.com/mcp/intercom-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Intercom** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `intercom-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Intercom** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "intercom-alternative": {
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

# Bird (Omnichannel Communication) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bird-omnichannel-communication)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Manage omnichannel communication via Bird (MessageBird) — send SMS, WhatsApp messages, and track delivery logs.

## Description
Connect your **Bird (formerly MessageBird)** account to any AI agent and take full control of your global communication infrastructure, omnichannel messaging, and CRM contacts through natural conversation.

### What you can do

- **Omnichannel Dispatch** — Send messages across SMS, WhatsApp, and Telegram using a single set of tools, automatically mapping the correct channel IDs directly from your agent
- **Massive SMS Scalability** — Dispatch high-priority SMS messages globally by specifying alphanumeric originators and E.164 recipient formats securely
- **Real-time Delivery Audit** — Retrieve detailed message metadata and delivery receipts (delivered, buffered, rejected) to investigate carrier-level rejections natively
- **CRM Contact Management** — Manage your communication directory by upserting contact entities and retrieving detailed profiles including custom attributes and metadata mappings
- **Financial Visibility** — Monitor your account balance and financial limits in real-time to prevent automated communication halts or unexpected billing issues
- **Broadcast History** — List and audit your chronological message streams to understand your engagement reach and delivery volume across multiple platforms
- **Threaded Conversations** — Enumerate active omnichannel chat groups to manage customer interactions across different messaging apps efficiently

### How it works

1. Subscribe to this server
2. Enter your Bird (MessageBird) Access Key
3. Start managing your global communication from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Growth Engineers** — automate the dispatch of marketing notifications and monitor delivery rates through natural conversation without manual dashboard exports
- **Support Operations** — manage omnichannel customer conversations and verify contact metadata directly from your workspace
- **Software Developers** — test communication flows and validate carrier delivery statuses across multiple geographies efficiently


## Available Tools (10)
- **create_contact**: Create a new CRM contact
- **delete_contact**: Delete a CRM contact
- **get_balance**: Get account balance
- **get_contact_details**: Get specific contact details
- **get_message_details**: Get details for a specific SMS
- **list_contacts**: List CRM contacts
- **list_conversations**: List active omnichannel conversations
- **list_messages**: List sent SMS messages
- **send_sms**: Send an SMS message
- **send_omnichannel_message**: Send a message via WhatsApp or Telegram


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bird (Omnichannel Communication)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS to '+1234567890' with the text 'Your package is ready for pickup'"

**🤖 AI Agent:**
> Dispatching SMS… I've successfully sent the message to '+1234567890'. The Message ID is 'sms-98765'. I'll monitor the delivery status and let you know once it's confirmed as delivered.

---

**👤 You:**
> "What is my current Bird account balance?"

**🤖 AI Agent:**
> Retrieving balance… You currently have €145.50 available in your account. Based on your recent traffic, this is enough to cover approximately 12,000 more global SMS messages. Would you like me to check for any delivery failures?

---

**👤 You:**
> "List all contacts in my communication directory"

**🤖 AI Agent:**
> I've retrieved your contacts. You have 1,250 registered entities. Recent contacts include 'Alex Smith' (+44123456789) and 'Sarah Johnson' (+1987654321). Which one would you like to see the detailed profile for?


## ❓ FAQ

**Q: Can I send WhatsApp messages through my agent using Bird?**
Yes. Use the `dispatch_omnichannel_stream` tool by specifying your WhatsApp Channel ID. Your agent will handle the formatting and transmit the text payload directly to your customer's WhatsApp inbox securely.

**Q: How do I check why an SMS wasn't delivered?**
The `get_sms_metadata` tool allows your agent to retrieve the precise delivery status for any Message ID. You'll be able to see if the carrier rejected the message or if it's currently buffered in their network.

**Q: Can my agent monitor my account balance to avoid service interruptions?**
Absolutely. Use the `get_account_balance` tool to retrieve your current funds status. Your agent will report your financial limits, helping you ensure there are enough credits to support your global communication flows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bird-omnichannel-communication](https://vinkius.com/mcp/bird-omnichannel-communication)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bird (Omnichannel Communication)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bird-omnichannel-communication` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bird (Omnichannel Communication)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bird-omnichannel-communication": {
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

# GoTo Connect MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/goto-connect)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your cloud phone system — view call records, send SMS, and manage voicemails via AI.

## Description
Connect your **GoTo Connect** (formerly Jive) unified communications account to your AI agent and manage your business telephony directly from your workflow. Use natural language to query call histories, send and receive SMS messages, and manage your contacts without opening the GoTo desktop app.

### What you can do

- **Call Records (CDR)** — Retrieve detailed call histories for specific users to audit activity or find a missed call
- **SMS Messaging** — Send SMS messages to clients directly from the chat and retrieve conversation histories
- **Voicemail Management** — List recent voicemails and check their transcription status
- **Device & User Management** — Look up active users, their extension numbers, and the status of their assigned devices
- **Contact Management** — Search through your company contacts and add new entries programmatically

### How it works

1. Subscribe to this server
2. Enter your GoTo OAuth Client ID and Secret (from the GoTo Developer Portal)
3. Complete the secure GoTo authorization flow
4. Start managing your communications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Representatives** — quickly send an SMS follow-up to a prospect right after logging a call in your CRM
- **Customer Support** — look up a client's recent call history or check if a voicemail was left before reaching out
- **IT Administrators** — easily verify which devices are assigned to a specific user extension through simple text commands


## Available Tools
- **create_contact**: Create a new contact
- **get_call_record**: Get details for a specific call record
- **get_call_records**: List call records (history) for a user
- **get_me**: Get details for the currently authenticated GoTo user
- **get_user**: Get details for a specific user
- **get_voicemail**: Get details for a specific voicemail
- **list_contacts**: List a user's contacts
- **list_devices**: List devices associated with a user
- **list_sms_messages**: List SMS messages for a user
- **list_users**: List GoTo Connect users
- **list_voicemails**: List voicemails for a user
- **send_sms**: Send an SMS message via GoTo Connect


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GoTo Connect** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show my recent call records."

**🤖 AI Agent:**
> Retrieving call history... Your last 3 calls were:
1. INBOUND from +1 (555) 123-4567 (Duration: 4m 12s)
2. OUTBOUND to +1 (555) 987-6543 (Duration: 12m 05s)
3. MISSED INBOUND from +1 (555) 555-5555

---

**👤 You:**
> "Send a text from my number to +15551234567 saying 'Hi, our meeting is starting in 5 mins'."

**🤖 AI Agent:**
> Sending SMS... Success! The message 'Hi, our meeting is starting in 5 mins' has been sent to +1 (555) 123-4567.

---

**👤 You:**
> "Check if an active voicemail remains for extension 202 unhandled."

**🤖 AI Agent:**
> Checking voicemails...
Yes, there is currently one untouched voice message (14 seconds long) originating from a classified client left at 9:00 AM.


## ❓ FAQ

**Q: Can I send an SMS message directly from the AI chat?**
Yes! Use the `send_sms` tool. Provide the sender number (one of your GoTo Connect numbers), the recipient's number, and the message body. The AI will send the text on your behalf.

**Q: How do I check my missed calls or voicemails?**
First, you can use `get_me` to confirm your User ID. Then, use `get_call_records` to view your call history (including missed calls) or `list_voicemails` to see if anyone left a message.

**Q: Is it possible to lookup extensions for active users?**
Yes. Using the directory management tools, you can actively search for any colleague by name or department to fetch their direct extension securely.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/goto-connect](https://vinkius.com/mcp/goto-connect)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **GoTo Connect** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `goto-connect` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **GoTo Connect** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "goto-connect": {
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

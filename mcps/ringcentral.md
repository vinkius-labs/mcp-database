# RingCentral MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ringcentral)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage business communications via RingCentral — send SMS, track call logs, and monitor presence directly from your AI agent.

## Description
Connect your **RingCentral** account to any AI agent to streamline your telephony and messaging workflows through natural conversation.

### What you can do

- **Messaging & SMS** — Send SMS messages directly to any recipient and browse your message store (SMS, Fax, Voicemail) history.
- **Call Analytics** — List and filter call logs by date, type, or detail level to audit communication patterns.
- **Presence Monitoring** — Check the real-time status and telephony state of your extension to manage availability.
- **Webhook Subscriptions** — Create, list, and renew event subscriptions to stay notified about incoming messages or calls.
- **Unified Communication** — Access your entire message store to retrieve past interactions without leaving your workspace.

### How it works

1. Subscribe to this server
2. Enter your RingCentral Access Token
3. Start managing your business communications from Claude, Cursor, or any MCP client

### Who is this for?

- **Sales Teams** — quickly send follow-up SMS and check call history with prospects.
- **Support Agents** — monitor presence and review voicemails or faxes within their primary AI interface.
- **Operations Managers** — audit call logs and manage automated webhook subscriptions for system integrations.


## Available Tools
- **list_call_logs**: Can be filtered by view type, date range, and call type.

List RingCentral call logs for the authenticated extension
- **create_subscription**: Create a new webhook subscription
- **list_subscriptions**: List all active subscriptions
- **list_message_store**: List messages from the message store
- **get_presence**: Get presence status for the authenticated extension
- **renew_subscription**: Renew an existing subscription
- **send_sms**: Send an SMS message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RingCentral** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS to +1234567890 from my number +1098765432 saying 'Hello from AI agent!'"

**🤖 AI Agent:**
> I've sent the SMS. The message ID is 12345678 and the status is currently 'Sent'.

---

**👤 You:**
> "Show me my call logs from the last 24 hours."

**🤖 AI Agent:**
> I found 3 calls in the last 24 hours: two inbound voice calls from +15550102 and one outbound fax. Would you like the detailed view for any of these?

---

**👤 You:**
> "Check my current presence status and tell me if I'm on a call."

**🤖 AI Agent:**
> Your current status is 'Available' and your telephony state is 'Idle'. You are not currently on an active call.


## ❓ FAQ

**Q: Can I send an SMS to a specific phone number using this server?**
Yes! Use the `send_sms` tool by providing the sender number, recipient number, and your message text. The AI will handle the API request and confirm delivery status.

**Q: Is it possible to filter my call history by date?**
Absolutely. The `list_call_logs` tool allows you to specify `dateFrom` and `dateTo` parameters (ISO 8601) to retrieve calls within a specific timeframe.

**Q: How can I check if my extension is currently busy or available?**
You can use the `get_presence` tool. It retrieves your current presence status and telephony state, and you can even request `detailedTelephonyState` for more info on active calls.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ringcentral](https://vinkius.com/mcp/ringcentral)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RingCentral** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `ringcentral` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RingCentral** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ringcentral": {
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

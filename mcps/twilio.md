# Twilio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/twilio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Automate communication workflows via Twilio — manage SMS messaging, voice calls, call recordings, and account usage directly from any AI agent.

## Description
Connect your **Twilio** account to any AI agent and take full control of your telecommunications infrastructure through natural conversation.

### What you can do

- **SMS Messaging** — Dispatch plain text messages instantly and read detailed metadata, including delivery status or segments
- **Voice Calls** — Initiate outbound phone calls pointing to TwiML URLs, track call activities, and immediately cancel active/in-progress calls
- **Audio Recordings** — Enumerate historically stored voice recordings across your ecosystem and retrieve their direct play URLs
- **Usage & Governance** — Monitor your exact spend stats alongside billing records, and audit current API keys for programmatic access

### How it works

1. Subscribe to this server
2. Enter your Twilio Account SID and Auth Token
3. Start operating your comms infrastructure from Claude, Cursor, or any MCP-compatible client

No more bouncing between the Twilio Console and your dashboard. Your AI agent becomes your programmable communication center.

### Who is this for?

- **DevOps & SREs** — trigger SMS paging alerts, cancel stuck calls, and audit rogue API keys without writing code
- **Support Managers** — review recent voice recordings or fetch missed SMS conversations instantly
- **Engineers** — test outbound logic with a simple prompt before hard-coding the actual TwiML workflows
- **Founders** — query exact spend usage records for the week to keep budgets under control


## Available Tools
- **cancel_active_call**: Immediately terminates an active voice call
- **delete_message**: The message body becomes inaccessible after deletion. This action is irreversible.

Permanently delete an SMS message record
- **get_account_info**: Retrieves information about the master Twilio account status
- **get_message_details**: Retrieves detailed metadata for a specific SMS message
- **get_recording_details**: Requires the recording SID (starting with RE).

Get detailed information about a specific call recording
- **get_usage_records**: Retrieves usage statistics and billing records for the account
- **list_calls**: Lists recent voice calls associated with the account
- **list_api_keys**: Lists API keys configured for the account
- **list_messages**: Lists recent SMS messages sent or received by the account
- **list_phone_numbers**: List all incoming phone numbers owned by the account
- **list_call_queues**: List all call queues configured for the account
- **list_recordings**: Lists all voice recordings stored in the account
- **lookup_phone_number**: Provide the number in E.164 format.

Look up information about a phone number
- **create_voice_call**: Provide a caller ID, receiver number, and a TwiML URL.

Initiates an outbound voice call using TwiML instructions
- **send_sms**: Provide an E.164 sender number and target receiver number.

Sends an SMS message using the Twilio API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Twilio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS to +14155552671 from my main number saying 'Server 3 is down, investigate ASAP'."

**🤖 AI Agent:**
> The SMS has been successfully dispatched. The Message SID is SMxyz123 and the current status is 'queued'. I can check back in a minute to confirm delivery.

---

**👤 You:**
> "List my recent phone calls and tell me if any failed."

**🤖 AI Agent:**
> I've retrieved 15 recent calls. 14 completed successfully. One call (SID CAabc456) has the status 'failed' to +15551234. Would you like to view the error details?

---

**👤 You:**
> "Show me our Twilio usage statistics to help understand our bill."

**🤖 AI Agent:**
> Accessing usage records... So far, your heaviest consumption comes from SMS outbound ($45.00 total over 4,500 messages). Voice minutes account for $12.30. Should I break down the voice categories further?


## ❓ FAQ

**Q: Can my AI agent trigger an incident alert SMS to the on-call engineer?**
Absolutely. You can provide your Twilio phone number, the destination E.164 number, and the alert body text. The agent will hit the Twilio API instantly, dispatch the SMS, and return the Message SID along with delivery status.

**Q: How can I stop a rogue voice call stuck in a loop?**
Ask your agent to list active or recent voice calls and find the offending Call SID. Then instruct the AI to cancel the active call by its ID. The agent updates its status to 'canceled', dropping the connection right away.

**Q: Can it check how much my company has spent so far this month?**
Yes. Ask the agent to pull your account's usage records. It interfaces with the Twilio billing records and can display breakdowns of amounts sent, call durations, and costs incurred, giving you full transparency without opening the dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/twilio](https://vinkius.com/mcp/twilio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Twilio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `twilio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Twilio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "twilio": {
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

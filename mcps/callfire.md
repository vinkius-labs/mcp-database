# CallFire MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/callfire)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage voice and SMS communications via CallFire — track calls, send texts, and monitor campaigns directly from any AI agent.

## Description
Connect your **CallFire** account to any AI agent and orchestrate your voice and SMS communications, campaign tracking, and contact engagement through natural conversation.

### What you can do

- **SMS Dispatch** — Send single or bulk SMS messages to your customers directly from your workspace.
- **Voice Call Management** — Trigger individual voice calls and monitor the status of sent calls in real-time.
- **Campaign Oversight** — List and retrieve metadata for your campaign sounds and verify your communication setups.
- **Keyword Management** — List and monitor your rented keywords for SMS interaction.
- **Automation Tracking** — Access and monitor your active webhooks to ensure your integrations are healthy.
- **Account Insights** — Retrieve core profile and site information straight from your workspace.

### How it works

1. Subscribe to this server
2. Enter your CallFire API Username and Password
3. Start managing your communications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Teams** — quickly send SMS notifications or alerts without manual portal work.
- **Sales & Support** — trigger follow-up calls or check message statuses straight from their workflow tools.
- **Ops Managers** — monitor campaign assets and webhook health using natural language.


## Available Tools (10)
- **get_account_info**: Retrieve core account information
- **get_call_details**: Get details of a specific call
- **get_sms_details**: Get details of a specific SMS
- **list_calls**: List made voice calls
- **list_campaign_sounds**: List configured campaign sounds
- **list_keywords**: List rented keywords
- **list_sent_sms**: List sent SMS messages
- **list_webhooks**: List active webhooks
- **send_voice_call**: Trigger a single voice call
- **send_sms**: Send an SMS message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CallFire** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS to +1234567890 saying 'Hi from Vinkius'."

**🤖 AI Agent:**
> I've sent the SMS to +1234567890. The message ID is msg_123 and it's currently marked as 'READY'.

---

**👤 You:**
> "List my last 5 voice calls in CallFire."

**🤖 AI Agent:**
> I've retrieved your calls. You have 5 recent calls, including a finished call to +1987654321 and a failed attempt to +15550199.

---

**👤 You:**
> "Show the details for SMS with ID 99283."

**🤖 AI Agent:**
> SMS 99283 was sent to +1234567890 on March 20th. The status is 'FINISHED' and the message body was 'Your code is 1234'.


## ❓ FAQ

**Q: Can I send an SMS using the agent?**
Yes! Use the `send_sms` tool with the recipient's phone number and your message content. Your agent will trigger the dispatch through CallFire instantly.

**Q: How do I check the status of a specific call?**
Simply ask the agent to `get_call_details` and provide the Call ID. It will retrieve the latest status, such as 'finished' or 'failed', directly from CallFire.

**Q: Does the integration allow creating a new voice broadcast?**
The current toolset is focused on individual actions and querying (Read-Only/Individual Dispatch) for operational control. Massive broadcasts should be configured via the CallFire web dashboard.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/callfire](https://vinkius.com/mcp/callfire)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CallFire** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `callfire` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CallFire** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "callfire": {
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

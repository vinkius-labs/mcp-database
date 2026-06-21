# CallFire MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/callfire)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/callfire-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/callfire-mcp)
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


## Available Tools
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


## Installation & Usage

To install and use the **CallFire** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/callfire](https://vinkius.com/mcp/callfire)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

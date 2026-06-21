# TNZ Communications MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tnz-communications)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tnz-communications-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tnz-communications-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Send SMS, Voice (TTS), and Fax messages via TNZ directly from your AI agent.

## Description
Empower your AI agent with access to the **TNZ Group** messaging gateway to automate your SMS, Voice, and Fax communications in New Zealand and globally.

### What you can do

- **Multichannel Messaging** — Send SMS, automated voice calls (Text-to-Speech), and digital faxes programmatically.
- **Delivery Oversight** — Monitor the real-time status of sent messages and retrieve incoming SMS replies.
- **Contact & Group Control** — Manage your TNZ address book and organize contacts into groups for broadcast messaging.
- **Operational Monitoring** — Track your account credit balance and retrieve detailed messaging usage and cost reports.

### How it works

1. Subscribe to this server
2. Enter your TNZ Auth Token from your dashboard
3. Start communicating from Claude, Cursor, or any MCP client

### Who is this for?

- **Business Operations** — Quickly send notifications and alerts to staff or customers via natural conversation.
- **Marketing Teams** — Automate SMS and Voice outreach sequences and track engagement results.
- **Customer Support** — Monitor and respond to incoming SMS replies without leaving your workspace.


## Available Tools
- **check_api_health**: Verify TNZ API connectivity
- **create_tnz_contact**: Add a new contact to TNZ
- **get_account_balance**: Check account credit balance
- **get_messaging_usage_report**: Retrieve usage and cost reports
- **get_message_delivery_status**: Check delivery status of a message
- **list_tnz_contacts**: List saved contacts in TNZ
- **list_contact_groups**: List your contact groups
- **list_received_sms_replies**: List inbound SMS replies
- **list_message_templates**: List saved message templates
- **send_digital_fax**: Send a document as a fax
- **send_sms_message**: Send an SMS message
- **send_tts_voice_call**: Send a voice call (Text-to-Speech)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TNZ Communications** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a SMS to +6421000000: 'The delivery is arriving at 2 PM today.'"

**🤖 AI Agent:**
> Done! I've sent the SMS message to +6421000000 via TNZ. MessageID: ref_123.

---

**👤 You:**
> "What is the status of my message ID 'ref_123'?"

**🤖 AI Agent:**
> The status for message 'ref_123' is 'DELIVERED'. It was received by the recipient today at 10:15 AM.

---

**👤 You:**
> "Check my current TNZ account balance."

**🤖 AI Agent:**
> You currently have $25.50 remaining in your TNZ Communications account.


## Installation & Usage

To install and use the **TNZ Communications** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tnz-communications](https://vinkius.com/mcp/tnz-communications)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

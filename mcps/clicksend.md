# ClickSend MCP Server

Manage SMS and multi-channel messaging via ClickSend — send messages, track history, and monitor inbound SMS directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/clicksend)

## Overview
**Category:** talk-to-me
**Tools Count:** 8

## Description
Connect your **ClickSend** account to any AI agent and take full control of your multi-channel messaging through natural conversation. Streamline how you communicate with customers via SMS, Voice, and even Physical Post natively.

### What you can do

- **SMS Delivery** — Send single or batch SMS messages to recipients globally in E.164 format natively
- **History Intelligence** — Access detailed outbound and inbound SMS history to audit conversations flawlessly
- **Campaign Management** — List and review scheduled SMS marketing campaigns and their current states securely
- **Voice & Post Logistics** — Retrieve history for automated voice calls and physical letters sent via ClickSend flawlessly
- **Contact Management** — List and monitor contacts stored in your account to manage your audience securely
- **Account Visibility** — Retrieve core account details, including credit balance, directly within your workspace flawlessly

### How it works

1. Subscribe to this server
2. Enter your ClickSend API Username and API Key (found in Dashboard > API Credentials)
3. Start managing your communications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — monitor SMS campaign performance and verify delivery using natural language
- **Operations Teams** — audit automated alerts and verify outbound voice call history without opening the dashboard
- **Customer Support** — quickly look up inbound SMS messages and recipient profiles straight from their chat interface
- **DevOps Engineers** — verify system alerts and monitor messaging throughput


## Available Tools
- **get_clicksend_account_info**: Retrieve core account details and balance
- **get_sms_outbound_history**: Retrieve a history of sent SMS messages
- **list_clicksend_contacts**: List all contacts stored in ClickSend
- **list_received_sms**: List all inbound (received) SMS messages
- **get_physical_mail_history**: Retrieve a history of physical letters sent via ClickSend Post
- **list_sms_marketing_campaigns**: List all scheduled and sent SMS marketing campaigns
- **get_voice_call_history**: Retrieve a history of automated voice calls sent
- **send_clicksend_sms**: Numbers should be in E.164 format.

Send one or more SMS messages


## Installation & Usage

To install and use the **ClickSend** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clicksend](https://vinkius.com/mcp/clicksend)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

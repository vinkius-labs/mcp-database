# Twilio MCP Server

Automate communication workflows via Twilio — manage SMS messaging, voice calls, call recordings, and account usage directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/twilio)

## Overview
**Category:** talk-to-me
**Tools Count:** 15

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


## Installation & Usage

To install and use the **Twilio** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/twilio](https://vinkius.com/mcp/twilio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

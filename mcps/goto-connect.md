# GoTo Connect MCP Server

Manage your cloud phone system — view call records, send SMS, and manage voicemails via AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/goto-connect)

## Overview
**Category:** productivity
**Tools Count:** 12

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


## Installation & Usage

To install and use the **GoTo Connect** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/goto-connect](https://vinkius.com/mcp/goto-connect)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

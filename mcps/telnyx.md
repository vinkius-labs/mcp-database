# Telnyx MCP Server

Send and manage SMS/MMS, check account balances, and configure messaging profiles natively via your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/telnyx)

## Overview
**Category:** communication-messaging
**Tools Count:** 10

## Description
Connect your **Telnyx** account to any AI agent and manage your voice and messaging operations directly through natural conversation.

### What you can do

- **Send Messages** — Dispatch SMS and MMS texts, including media URLs, across your numbers in real-time
- **Check Delivery Status** — Look up message details and verify whether texts were successfully delivered or rejected
- **Manage Phone Numbers** — Browse your active E.164 phone numbers and retrieve configuration details
- **Messaging Profiles** — Create, update, list, and delete messaging profiles for your applications
- **Account Billing** — Monitor your exact account balance and available credits before dispatching campaigns

### How it works

1. Subscribe to this server
2. Enter your Telnyx API Key
3. Start managing telecom services strictly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Development teams** — debug messaging webhooks, check logs, and provision profiles quickly without leaving their IDE
- **Marketing managers** — trigger specific text campaigns or verify the balance before a massive SMS broadcast
- **Support tech** — investigate SMS delivery failures by retrieving precise message statues in seconds


## Available Tools
- **create_messaging_profile**: Creates a new messaging profile
- **delete_messaging_profile**: This action is irreversible.

Permanently deletes a messaging profile
- **get_account_balance**: Retrieves the current Telnyx account credit balance
- **get_message_details**: Retrieves details and delivery status for a specific message
- **get_number_settings**: Retrieves configuration and capability details for a specific phone number
- **get_messaging_profile_details**: Retrieves details for a specific messaging profile
- **list_phone_numbers**: 164 numbers and retrieve their unique IDs.

Lists all phone numbers owned by the account
- **list_messaging_profiles**: Lists all messaging profiles in the account
- **send_text_message**: Provide a registered Telnyx from_number and a target to_number in E.164 format.

Sends an outbound SMS message via Telnyx
- **send_media_message**: Provide from/to numbers and a 100% public JPEG/PNG URL.

Sends an outbound MMS message with a media URL


## Installation & Usage

To install and use the **Telnyx** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/telnyx](https://vinkius.com/mcp/telnyx)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

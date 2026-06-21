# Vonage MCP Server

Send SMS, WhatsApp, and Viber messages, and manage virtual numbers and 2FA via Vonage communications platform.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/vonage)

## Overview
**Category:** talk-to-me
**Tools Count:** 10

## Description
Connect your **Vonage** account to any AI agent and power your global communications through natural conversation.

### What you can do

- **Multi-Channel Messaging** — Send outbound messages via SMS, WhatsApp Business, and Viber with ease
- **2FA & Verification** — Start and check identity verification requests (OTP) to secure your user accounts
- **Number Management** — List all virtual phone numbers rented by your account and update their inbound webhooks
- **Account Insights** — Check your real-time account credit balance and monitor spending directly from your agent
- **Global Pricing** — Retrieve outbound SMS pricing for any country to estimate communication costs accurately
- **Virtual Numbers** — View caller ID capabilities (SMS, Voice) for all your rented virtual numbers

### How it works

1. Subscribe to this server
2. Enter your Vonage API Key and API Secret
3. Start dispatching messages and managing numbers through Claude, Cursor, or any MCP-compatible client

No more manual logging into communication dashboards to send a single text. Your AI agent becomes your communication command center.

### Who is this for?

- **Customer Support** — send quick verification codes or updates to customers across multiple messaging channels
- **Marketing Teams** — estimate campaign costs and manage virtual numbers for different regions
- **Developers** — test messaging integrations and monitor API usage through simple chat commands
- **Operations Managers** — track account balance and manage global communication workflows efficiently


## Available Tools
- **cancel_verification_request**: Aborts an active verification request
- **get_account_balance**: Retrieves the current Vonage account credit balance
- **get_country_pricing**: Provide the ISO 3166-1 alpha-2 country code.

Retrieves outbound SMS pricing for a specific country
- **list_rented_numbers**: Lists all virtual phone numbers rented by the account
- **send_sms**: Provide a sender name (alpha or number) and a target phone number in E.164 format.

Sends an outbound SMS message via Vonage
- **send_viber_message**: Provide your specific Viber Publisher ID.

Sends a Viber service message via Vonage
- **send_whatsapp_message**: Requires a verified WhatsApp Business Number as the sender.

Sends a WhatsApp message via the Vonage Messages API
- **update_number_webhook**: Requires the number in E.164 format.

Updates the inbound SMS callback URL for a virtual number
- **check_verification_code**: Checks the OTP code submitted by a user for an active verification request
- **start_verification**: Provide the target number and your brand name.

Starts a 2FA identity verification by sending an OTP code


## Installation & Usage

To install and use the **Vonage** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vonage](https://vinkius.com/mcp/vonage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

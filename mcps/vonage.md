# Vonage MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/vonage)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Send SMS, WhatsApp, and Viber messages, and manage virtual numbers and 2FA via Vonage communications platform.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vonage** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS to +123456789 saying 'Your order is ready for pickup!'."

**🤖 AI Agent:**
> I've sent the SMS to +123456789 via Vonage. Message: 'Your order is ready for pickup!'. The message was successfully dispatched (Message ID: msg-abc).

---

**👤 You:**
> "Start a verification for number +123456789 with brand 'MyCoolApp'."

**🤖 AI Agent:**
> Identity verification started for +123456789. The OTP code has been sent. Your Request ID is 'req-xyz'. Please let me know the code when you receive it to complete the check.

---

**👤 You:**
> "What is my current account balance and the SMS price for the UK?"

**🤖 AI Agent:**
> Your current Vonage balance is 42.50 EUR. For the United Kingdom (GB), the outbound SMS price is approximately 0.045 EUR per message. You have enough credit for roughly 944 messages.


## ❓ FAQ

**Q: Can I send WhatsApp messages using this server?**
Yes. The `send_whatsapp_message` tool allows you to send outbound WhatsApp messages through the Vonage Messages API. You'll need a verified WhatsApp Business Number configured in your Vonage account as the sender.

**Q: How do I implement two-factor authentication (2FA)?**
You can use the `start_verification` tool to send an OTP code to a user's phone. Once the user receives the code, use `check_verification_code` with the `request_id` to validate it. Your agent can handle the entire flow through a single conversation.

**Q: Can I check how much sending an SMS will cost me?**
Absolutely. Use the `get_country_pricing` tool and provide the ISO country code (e.g., 'US' or 'GB'). Your agent will return the outbound SMS pricing for that region, helping you estimate costs before sending.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/vonage](https://vinkius.com/mcp/vonage)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vonage** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `vonage` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vonage** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vonage": {
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

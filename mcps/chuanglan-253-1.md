# Chuanglan 253 MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/chuanglan-253-1)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Ultra-high volume SMS & 1-click login API — send verification codes, notifications, and bulk messages globally via Chuanglan 253.

## Description
Connect your **Chuanglan 253** SMS gateway to any AI agent and transform your communication workflows through natural conversation. Chuanglan (创蓝) is one of China's largest CPaaS providers, handling billions of SMS messages monthly for verification, notifications, and marketing.

### What you can do

- **Send SMS Messages** — Deliver text messages to any phone number worldwide with country code support
- **Verification Codes** — Send one-time passwords (OTP) for 1-click login flows and two-factor authentication
- **Voice Verification** — Fallback to automated voice calls when SMS delivery is unreliable
- **Balance Monitoring** — Check your SMS credit balance and quota in real-time before campaigns
- **Delivery Tracking** — Query the status of individual messages or entire batches with message IDs
- **Template Management** — List, create, and manage pre-approved SMS templates for compliance
- **Account Management** — View account settings, permissions, and enabled features

### How it works

1. Subscribe to this server
2. Enter your Chuanglan 253 API Account and Password
3. Start sending SMS and verification codes from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes your SMS operations center, handling verification flows, delivery monitoring, and campaign tracking without touching a dashboard.

### Who is this for?

- **Developers** — Integrate SMS verification and 1-click login directly into AI-assisted workflows
- **Product Teams** — Monitor SMS delivery rates and template compliance through natural language queries
- **Operations** — Track bulk SMS campaign status and account balance without API calls
- **Security Teams** — Send verification codes and voice calls for multi-factor authentication flows


## Available Tools
- **create_template**: The template must be approved before it can be used. Template content should include variable placeholders like {1}, {2} for dynamic content. Approval typically takes a few minutes to hours.

Create a new SMS template in Chuanglan 253
- **get_account_info**: ).

Get Chuanglan 253 account information and settings
- **get_sms_balance**: Use this to monitor available messaging capacity before sending campaigns.

Check SMS account balance on Chuanglan 253
- **query_batch_sms_status**: This is useful for checking the status of bulk SMS campaigns where multiple messages were sent with the same tracking identifier.

Query delivery status for a batch of SMS messages
- **query_sms_status**: Returns whether the message was delivered, is pending, or failed, along with timestamps.

Query delivery status of a specific SMS message
- **query_template_list**: Templates are pre-approved message formats that can be used for sending. Each template has an ID, name, content, and approval status.

List all SMS templates in your Chuanglan account
- **send_international_sms**: The phone number must include the country code without 00 prefix (e.g., 5511999999999 for Brazil). This endpoint uses the international gateway and requires proper permissions.

Send an international SMS message via Chuanglan 253
- **send_sms**: The phone number must include the country code (e.g., 86 for China, 55 for Brazil). For Chinese domestic SMS, the message content must start with a signature in brackets like [YourBrand]. Returns submission status and message ID.

Send an SMS message via Chuanglan 253 platform
- **send_verification_sms**: This is commonly used for 1-click login flows, phone number verification, and two-factor authentication. The message format should follow the template registered in your account. Phone number must include country code.

Send a verification code SMS (1-click login style)
- **send_voice_verification**: This is an alternative to SMS verification, useful when SMS delivery fails or for enhanced security. The code will be spoken in the call.

Send a voice verification call with a code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Chuanglan 253** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a verification code 837462 to phone number 8615800000000."

**🤖 AI Agent:**
> ✅ Verification code sent successfully! Message ID: 162575412960104448. The code 837462 has been delivered to 8615800000000. You can track delivery status using the message ID if needed.

---

**👤 You:**
> "Check my SMS balance and account status."

**🤖 AI Agent:**
> 📊 Your Chuanglan account is active with a balance of 15,847 SMS credits. You have sufficient quota for bulk campaigns. Account status: Active, all features enabled (domestic SMS, international SMS, voice verification).

---

**👤 You:**
> "What's the delivery status of message ID 162575412960104448?"

**🤖 AI Agent:**
> 📬 Message ID 162575412960104448 status: DELIVRD (Delivered successfully). Delivered at 2024-01-15 14:32:07. The verification code reached the recipient's device.


## ❓ FAQ

**Q: How do I format phone numbers for sending SMS?**
Phone numbers must include the country code without the 00 prefix. For example: China uses 86 (e.g., 8615800000000), Brazil uses 55 (e.g., 5511999999999), US uses 1 (e.g., 12025551234). The number should be 5-20 digits total. For Chinese domestic SMS, the message must start with a registered signature like [YourBrand].

**Q: What's the difference between send_sms and send_international_sms tools?**
The `send_sms` tool uses the standard SMS gateway (smssh.253.com) optimized for Chinese domestic messages and requires pre-registered templates and signatures. The `send_international_sms` tool uses the international gateway (intapi.253.com) for global delivery outside China, which supports SenderId and doesn't require Chinese-style signatures. International SMS permissions must be separately enabled in your account.

**Q: How does the MD5 signature authentication work?**
The Chuanglan API uses MD5 signature authentication for security. Your password is NEVER sent in the request body. Instead, it's combined with the request parameters and timestamp (nonce), then hashed with MD5 to generate a `sign` header. The server validates this signature to ensure request integrity. The framework handles all signature generation automatically — you only need to provide your account and password.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/chuanglan-253-1](https://vinkius.com/mcp/chuanglan-253-1)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Chuanglan 253** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `chuanglan-253-1` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Chuanglan 253** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "chuanglan-253-1": {
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

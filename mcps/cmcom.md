# CM.com MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cmcom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Reach customers on WhatsApp, SMS, RCS, and voice with a unified messaging platform built for conversational commerce.

## Description
Connect your **CM.com** account to any AI agent and control your omnichannel communications through natural conversation.

### What you can do

- **SMS Messaging** — Send individual SMS messages or broadcast to multiple recipients in a single request
- **Rich Messaging** — Deliver messages through WhatsApp, Viber, RCS, or Apple Messages for Business
- **WhatsApp Templates** — Send pre-approved WhatsApp Business template messages with namespace support
- **Voice Communications** — Place automated calls for voice OTP delivery or text-to-speech notifications
- **Email Delivery** — Send HTML emails through CM.com's delivery infrastructure
- **OTP Verification** — Send SMS OTPs and verify codes for two-factor authentication
- **Account Management** — Check your credit balance and list virtual phone numbers

### How it works

1. Subscribe to this server
2. Enter your CM.com Product Token from your Channels dashboard
3. Start sending messages from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Teams** — send transactional SMS, WhatsApp notifications, and voice alerts without writing integration code
- **Security Teams** — implement OTP verification flows for two-factor authentication directly from AI workflows
- **Marketing Teams** — send bulk SMS campaigns and check delivery through conversational AI


## Available Tools
- **get_balance**: com account.

Check account balance
- **list_numbers**: com account.

List phone numbers
- **send_bulk_sms**: Send bulk SMS
- **send_email**: com email delivery infrastructure.

Send an email
- **send_otp_sms**: Send OTP via SMS
- **send_rich_message**: Send a rich message
- **send_sms**: Send an SMS
- **send_voice_message**: Send voice notification
- **send_voice_otp**: Send voice OTP
- **send_whatsapp**: Send WhatsApp template
- **verify_otp**: Verify OTP code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CM.com** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS to +31612345678 saying 'Your order has been shipped' from our company number."

**🤖 AI Agent:**
> SMS sent successfully! From: 'MyCompany', To: +31612345678, Body: 'Your order has been shipped'. Message ID: msg_84201. Status: delivered. Credits used: 1. Current balance: 4,231 credits remaining. Would you like to send the same message to other recipients?

---

**👤 You:**
> "Send OTP verification to +1555987654 and then verify the code 482910."

**🤖 AI Agent:**
> Step 1: OTP sent via SMS to +1555987654. Verification ID: ver_29401. The recipient should receive a 6-digit code within 10 seconds. Step 2: Verifying code 482910... ✅ Code verified successfully! Verification status: 'approved'. The OTP flow is complete — the user is now authenticated. Would you like to send a confirmation SMS?

---

**👤 You:**
> "Send a WhatsApp template message about appointment confirmation to +44789012345."

**🤖 AI Agent:**
> WhatsApp template message sent! From: +31201234567, To: +44789012345. Template: 'appointment_confirmation' (namespace: 'my_business_ns'). Status: accepted by WhatsApp Business API. The recipient will see the formatted message in their WhatsApp chat. Note: template messages require prior approval from Meta. Would you like to also send an SMS fallback?


## ❓ FAQ

**Q: Can I send messages through WhatsApp, Viber, and other rich channels?**
Yes! The `send_rich_message` action lets you send through WhatsApp, Viber, RCS, or Apple Messages by specifying the channel parameter. For WhatsApp Business specifically, use `send_whatsapp` to send pre-approved template messages with a template ID and namespace.

**Q: Can I implement two-factor authentication with OTP verification?**
Yes. Use `send_otp_sms` to deliver a verification code via SMS — it returns a verification ID. Then call `verify_otp` with that verification ID and the code the user enters. For voice-based OTP delivery, use `send_voice_otp` to read the code to the user via an automated phone call.

**Q: Can I check my CM.com credit balance before sending campaigns?**
Yes. The `get_balance` tool retrieves your current credit balance. Use `list_numbers` to see all virtual phone numbers in your account. Both tools help you plan campaigns before committing to bulk sends via `send_bulk_sms`.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cmcom](https://vinkius.com/mcp/cmcom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **CM.com** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `cmcom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **CM.com** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cmcom": {
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

# CM.com MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cmcom)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cmcom-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cmcom-mcp)
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


## Installation & Usage

To install and use the **CM.com** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cmcom](https://vinkius.com/mcp/cmcom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

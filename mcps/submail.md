# Submail / 赛邮云 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/submail)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/submail-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/submail-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Powerful SMS, Email, and Voice communication platform — orchestrate multi-channel messaging via AI.

## Description
Empower your AI agent to orchestrate your multi-channel communications with **Submail** (赛邮云), the premier cloud communication platform in China. By connecting Submail to your agent, you transform complex SMS broadcasting, HTML email sending, and voice-to-speech notifications into a natural conversation. Your agent can instantly send transactional messages, calculate remaining credit balances, and coordinate verify-by-voice calls without you ever needing to navigate the comprehensive Submail Management Console. Whether you are managing user alerts or coordinating automated verification flows, your agent acts as a real-time communication coordinator, providing accurate and fast results from a single, authorized source.

### What you can do

- **Multi-Channel Orchestration** — Send SMS, HTML emails, and voice notifications from a single agent interface.
- **Template Automation** — Utilize project-based templates (XSend) with custom variables for dynamic messaging.
- **Verification Management** — Trigger voice verification codes and monitor real-time delivery status.
- **Credit Auditing** — Query remaining balances for SMS, Mail, and Voice credits to ensure service continuity.
- **Operational Monitoring** — Verify API connectivity and AppID configurations to maintain system-wide health.

### How it works

1. Subscribe to this server
2. Enter your Submail AppID and AppKey
3. Start managing your communications through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **DevOps & Backend Engineers** — automate system notifications and monitor communication health through natural language.
- **Customer Operations** — manage transactional messaging and verify user identities directly from your AI-powered workspace.
- **Developers** — integrate professional-grade multi-channel APIs into your AI-driven daily routines.
- **Submail Power Users** — integrate your existing communication projects into your AI-driven daily routines.


## Available Tools
- **get_mail_balance**: Get Mail credits balance
- **get_sms_balance**: Get SMS credits balance
- **get_voice_balance**: Get Voice credits balance
- **send_mail**: Send Email
- **send_sms**: Send SMS message
- **send_template_sms**: Send template SMS (XSend)
- **send_voice**: Send Voice notification
- **send_voice_verify**: Send Voice verification code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Submail / 赛邮云** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a standard SMS to '13800138000' with content 'Your package has arrived'."

**🤖 AI Agent:**
> I've successfully sent the SMS to `13800138000`. The Submail send ID is `88210934`. Would you like me to check your remaining SMS balance?

---

**👤 You:**
> "Check my current account balance for Mail and Voice credits."

**🤖 AI Agent:**
> I've retrieved your balances. You have 15,240 Mail credits and 850 Voice credits remaining. Should I also check your SMS balance to ensure all channels are topped up?

---

**👤 You:**
> "Send a voice verification code '1234' to '13800138000'."

**🤖 AI Agent:**
> I've initiated the voice verification call to `13800138000`. The code '1234' will be read to the user. Would you like me to monitor the call status for you?


## Installation & Usage

To install and use the **Submail / 赛邮云** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/submail](https://vinkius.com/mcp/submail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

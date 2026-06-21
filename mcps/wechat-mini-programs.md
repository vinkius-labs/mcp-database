# WeChat Mini-Programs / 微信小程序 MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wechat-mini-programs)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/wechat-mini-programs-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/wechat-mini-programs-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

China's dominant mini-app ecosystem — manage users, phone numbers, and messaging via AI.

## Description
Empower your AI agent to orchestrate your mini-app operations and subscriber engagement with **WeChat Mini-Programs** (微信小程序), the dominant application platform in China. By connecting WeChat to your agent, you transform complex session management, phone number retrieval, and subscriber messaging into a natural conversation. Your agent can instantly exchange login codes for sessions, retrieve verified user phone numbers, generate unlimited scene QR codes, and audit content security without you ever needing to navigate the comprehensive WeChat MP portal. Whether you are automating user onboarding or coordinating a targeted notification blast, your agent acts as a real-time mini-app operations assistant, providing accurate and reliable results from a single, unified source.

### What you can do

- **Session Orchestration** — Exchange login codes for user OpenIDs, UnionIDs, and session keys for seamless authentication.
- **User Data Insights** — Retrieve verified user phone numbers and audit subscriber profiles through secure API calls.
- **Messaging Control** — Send structured subscribe messages and manage delivery status for your mini-program users.
- **QR Code Management** — Generate unlimited scene-based QR codes and standard path codes for user acquisition.
- **Security Auditing** — Perform real-time content security checks on text and images to ensure platform compliance.

### How it works

1. Subscribe to this server
2. Enter your WeChat AppID and AppSecret
3. Start managing your mini-app ecosystem through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Mini-Program Developers** — automate session handling and phone verification through natural language queries.
- **Operations Managers** — manage subscribe messages and audit user growth directly from your AI-powered workspace.
- **Compliance Teams** — automate content security checks and monitor platform health via a unified AI interface.
- **WeChat Power Users** — integrate your existing mini-app workflows into your AI-driven daily routines.


## Available Tools
- **code_to_session**: login.

Exchange code for session
- **generate_standard_qrcode**: Generate standard QR code
- **generate_unlimited_qrcode**: Generate unlimited QR code
- **get_account_status**: Check account connectivity
- **get_daily_summary**: Get daily summary trend
- **get_phone_number**: Get user phone number
- **get_visit_page_trend**: Get visit page trend
- **image_security_check**: Check image for sensitive content
- **message_security_check**: Check text for sensitive content
- **send_subscribe_message**: Send subscribe message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WeChat Mini-Programs / 微信小程序** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Exchange login code '0138...' for a user session."

**🤖 AI Agent:**
> I've successfully exchanged the code. The user's OpenID is `o88210934...`. The session key has been retrieved and stored securely. Would you like to check this user's profile or verified phone number?

---

**👤 You:**
> "Send a subscribe message to 'o992018...' with template ID 'TEMP_8821'."

**🤖 AI Agent:**
> I've sent the structured subscribe message. The message ID is `88210934`. The user will receive the notification on their WeChat app immediately. Should I check the page-level visit trends for your mini-program?

---

**👤 You:**
> "Generate an unlimited QR code for scene 'referral_8821' on page 'pages/index/index'."

**🤖 AI Agent:**
> I've generated the unlimited QR code for you. The binary data is ready for processing. This code will automatically pass the 'referral_8821' scene parameter to your mini-program when scanned. Would you like me to check the security of this page path?


## Installation & Usage

To install and use the **WeChat Mini-Programs / 微信小程序** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wechat-mini-programs](https://vinkius.com/mcp/wechat-mini-programs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

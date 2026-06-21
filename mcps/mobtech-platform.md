# MobTech Platform MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mobtech-platform)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mobtech-platform-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mobtech-platform-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Bring MobTech's SMSSDK and ShareSDK to your AI workflow. Automate SMS code verifications and analyze social engagement.

## Description
Connect your AI agents to **MobTech**, China's leading mobile development SDK provider. This server integrates directly with MobTech's APIs to provide backend support for SMSSDK and ShareSDK.

### What you can do

- **SMS Verification** — Automatically verify user-submitted SMS 2FA codes against the MobTech backend without writing REST queries
- **Phone Auditing** — Check delivery statuses or rate limiting rules on specific phone numbers
- **Social Analytics** — Extract ShareSDK data to track how often your app was shared to WeChat, Weibo, or QQ
- **OAuth Verification** — Check the social authentication binding status of users

### How it works

1. Subscribe to this server
2. Insert your **AppKey** and **AppSecret** from the [MobTech Dashboard](http://www.mob.com/)
3. Start verifying numbers from your agent context

### Who is this for?

- **Authentication Bots** — Agents handling onboarding and user identity verification flows
- **Marketing Analysts** — Extract share metrics across various Asian social networks instantly
- **App Developers** — Programmatic backend support for apps using MobTech SDKs


## Available Tools
- **check_phone_status**: Check if a phone number limit has been reached
- **get_share_analytics**: Get analytics for social sharing via ShareSDK
- **get_social_auth_status**: Check the OAuth binding status for a user
- **verify_sms_code**: Verify an SMS activation code sent to a user


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MobTech Platform** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Verify the SMS code 582910 for phone number +86 13800000000."

**🤖 AI Agent:**
> I've contacted MobTech. The verification code 582910 is valid for this phone number. You can proceed with logging the user in.

---

**👤 You:**
> "Check the share analytics for WeChat for the last 7 days."

**🤖 AI Agent:**
> According to the ShareSDK data, there were 4,210 WeChat session shares and 1,200 Moments shares tracked in the last 7 days.


## Installation & Usage

To install and use the **MobTech Platform** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mobtech-platform](https://vinkius.com/mcp/mobtech-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

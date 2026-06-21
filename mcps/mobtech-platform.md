# MobTech Platform MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mobtech-platform)
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


## ❓ FAQ

**Q: Where do I find my AppKey?**
Log into the MobTech official dashboard at mob.com, access your App settings, and your AppKey will be displayed at the top of the interface.

**Q: Can I completely bypass the Mobile SDK?**
This backend MCP wraps the API meant to *verify* SMS sent via your front-end Mobile App SDK. Your front-end app should still invoke the SDK for sending SMS and handling UI.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mobtech-platform](https://vinkius.com/mcp/mobtech-platform)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MobTech Platform** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mobtech-platform` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MobTech Platform** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mobtech-platform": {
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

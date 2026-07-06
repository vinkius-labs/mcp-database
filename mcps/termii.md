# Termii MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/termii)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Verify users and send business messages across SMS, WhatsApp, and voice channels with an African-first communication API.

## Description
Connect your **Termii** account to any AI agent and simplify how you manage your global messaging, secure verification, and multi-channel engagement through natural conversation.

### What you can do

- **Multi-channel Messaging** — Send standard SMS and WhatsApp messages to recipients worldwide with reliable delivery tracking.
- **Secure Verification (OTP)** — Send and verify one-time passwords (OTP) programmatically to secure your user onboarding and transactions.
- **Sender ID Management** — List all registered Sender IDs to ensure your messages are delivered with recognized branding.
- **Financial Monitoring** — Check your account balance and track credit usage for your messaging campaigns directly from the agent.
- **Global Coverage** — Reach users across different channels (SMS, WhatsApp, Voice) using Termii's unified communication infrastructure.
- **Real-time Oversight** — Monitor transaction statuses and verify identity tokens instantly via AI commands.

### How it works

1. Subscribe to this server
2. Enter your Termii API Key (found in your account dashboard)
3. Start managing your communications and verification from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers & DevOps** — quickly test messaging delivery and integrate OTP verification via simple AI commands.
- **Marketing Teams** — automate proactive outreach and monitor credit balances directly from the workspace.
- **Security Analysts** — verify identity tokens and monitor communication flows via the AI assistant.


## Available Tools (6)
- **send_sms**: Pass data as a JSON string.

Send an SMS message
- **send_whatsapp**: Pass data as a JSON string.

Send a WhatsApp message
- **verify_otp**: Verify an OTP code
- **check_balance**: Check account balance
- **list_sender_ids**: List all registered Sender IDs
- **send_otp**: Pass options in JSON.

Send a one-time password


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Termii** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a verification code (OTP) to +15550199."

**🤖 AI Agent:**
> Verification initiated! I've triggered the OTP code delivery to +15550199 via Termii. The request reference ID is pin_88231. I'll let you know when the user provides the code to verify.

---

**👤 You:**
> "Check my account balance."

**🤖 AI Agent:**
> Fetching balance... You currently have $45.50 in your Termii account. This balance is sufficient for your upcoming automated SMS and WhatsApp campaigns.

---

**👤 You:**
> "List all Sender IDs registered for my account."

**🤖 AI Agent:**
> I've retrieved your Sender IDs. You have 3 authorized IDs: 'VINKIUS', 'ALERT_MS', and 'AUTH_MSG'. Which one would you like to use for your next campaign?


## ❓ FAQ

**Q: Can I send an OTP code for user verification via AI?**
Yes! Use the `send_otp` action. Provide the destination number, your Sender ID, and the message type in the JSON payload. Your agent will trigger the OTP delivery instantly.

**Q: How do I check my remaining account balance?**
Run the `check_balance` query. The agent will retrieve your current available credits directly from Termii, helping you monitor your messaging budget.

**Q: Is it possible to see my registered Sender IDs via AI?**
Absolutely. Use the `list_sender_ids` tool. Your agent will retrieve the complete list of all Sender IDs authorized for your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/termii](https://vinkius.com/mcp/termii)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Termii** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `termii` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Termii** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "termii": {
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

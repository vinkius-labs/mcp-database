# Telnyx MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/telnyx-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage your Telnyx communications — audit phone numbers, messages, and calls via AI.

## Description
Empower your AI agent to orchestrate your entire global communication infrastructure with **Telnyx**, the leading platform for mission-critical connectivity. By connecting Telnyx to your agent, you transform complex telecom management into a natural conversation. Your agent can instantly list your phone numbers, audit message delivery, and retrieve call logs without you ever touching a technical portal. Whether you are providing secure alerts or managing global voice infrastructure, your agent acts as a real-time telecom strategist, ensuring your communication is always reliable and your account data is organized.

### What you can do

- **Messaging Intelligence** — Send SMS messages globally and retrieve detailed message status and history instantly.
- **Call Auditing** — List all recent voice calls and retrieve metadata for each, including direction and duration.
- **Number Oversight** — List and monitor all phone numbers associated with your account to maintain strict control.
- **Financial Intelligence** — Check your real-time account balance to manage organizational costs effectively.
- **Profile Management** — List messaging profiles and verified numbers to ensure your communication strategy is active.

### How it works

1. Subscribe to this server
2. Enter your Telnyx API Key
3. Start managing your telecom workflow through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Operations Managers** — monitor communication spend and send quick SMS alerts straight from your workflow.
- **Customer Success Teams** — verify message delivery and audit call logs without manual portal logins.
- **Telecom Engineers** — perform rapid audits of number configurations and messaging profiles.
- **Business Owners** — automate telecom querying to orchestrate your data-driven communication strategy smoothly.


## Available Tools
- **get_call**: Get details for a specific call
- **get_me**: Get authenticated Telnyx public key/info
- **get_phone_number**: Get details for a specific phone number
- **get_balance**: Get account balance
- **list_calls**: List recent voice calls
- **list_messages**: List recent messages
- **list_messaging_profiles**: List messaging profiles
- **list_phone_numbers**: List Telnyx phone numbers
- **list_verified_numbers**: List verified numbers
- **send_message**: Send an SMS message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Telnyx** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Telnyx phone numbers."

**🤖 AI Agent:**
> I've retrieved your phone numbers. You have 2 active numbers: '+1 234 567 890' and '+1 987 654 321'. Both are active and ready for voice/SMS.

---

**👤 You:**
> "Check my Telnyx account balance."

**🤖 AI Agent:**
> I've retrieved your balance. You currently have $125.50 available in your Telnyx account. Credit limit is $0.00.

---

**👤 You:**
> "Show me the last 5 calls for my project."

**🤖 AI Agent:**
> I've found 5 recent calls. Notable interactions include an outbound call to '+1 111 2222' with status 'completed'. Would you like the full metadata for any specific call?


## ❓ FAQ

**Q: How do I find my Telnyx API Key?**
Log in to the [**Telnyx Mission Control Portal**](https://portal.telnyx.com/), go to **Account Settings** > **API Keys**, and create a new key. Copy and paste it below.

**Q: Can the agent check my available balance?**
Yes. Use the `get_balance` tool. Your agent will retrieve your current account balance and credit limit from Telnyx instantly.

**Q: Is it possible to send global SMS messages via the agent?**
Yes. The `send_message` tool allows your agent to deliver SMS to any global number using your Telnyx phone numbers, provided your account has the correct messaging profiles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/telnyx-alternative](https://vinkius.com/mcp/telnyx-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Telnyx** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `telnyx-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Telnyx** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "telnyx-alternative": {
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

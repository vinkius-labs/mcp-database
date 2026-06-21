# ClickSend MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clicksend)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [talk-to-me](../categories/talk-to-me.md)

Manage SMS and multi-channel messaging via ClickSend — send messages, track history, and monitor inbound SMS directly from any AI agent.

## Description
Connect your **ClickSend** account to any AI agent and take full control of your multi-channel messaging through natural conversation. Streamline how you communicate with customers via SMS, Voice, and even Physical Post natively.

### What you can do

- **SMS Delivery** — Send single or batch SMS messages to recipients globally in E.164 format natively
- **History Intelligence** — Access detailed outbound and inbound SMS history to audit conversations flawlessly
- **Campaign Management** — List and review scheduled SMS marketing campaigns and their current states securely
- **Voice & Post Logistics** — Retrieve history for automated voice calls and physical letters sent via ClickSend flawlessly
- **Contact Management** — List and monitor contacts stored in your account to manage your audience securely
- **Account Visibility** — Retrieve core account details, including credit balance, directly within your workspace flawlessly

### How it works

1. Subscribe to this server
2. Enter your ClickSend API Username and API Key (found in Dashboard > API Credentials)
3. Start managing your communications from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — monitor SMS campaign performance and verify delivery using natural language
- **Operations Teams** — audit automated alerts and verify outbound voice call history without opening the dashboard
- **Customer Support** — quickly look up inbound SMS messages and recipient profiles straight from their chat interface
- **DevOps Engineers** — verify system alerts and monitor messaging throughput


## Available Tools (8)
- **get_clicksend_account_info**: Retrieve core account details and balance
- **get_sms_outbound_history**: Retrieve a history of sent SMS messages
- **list_clicksend_contacts**: List all contacts stored in ClickSend
- **list_received_sms**: List all inbound (received) SMS messages
- **get_physical_mail_history**: Retrieve a history of physical letters sent via ClickSend Post
- **list_sms_marketing_campaigns**: List all scheduled and sent SMS marketing campaigns
- **get_voice_call_history**: Retrieve a history of automated voice calls sent
- **send_clicksend_sms**: Numbers should be in E.164 format.

Send one or more SMS messages


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ClickSend** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a 'Welcome to Vinkius!' SMS to +1234567890."

**🤖 AI Agent:**
> Sending your welcome message... The SMS has been successfully submitted to ClickSend for delivery to +1234567890. Status: Queued.

---

**👤 You:**
> "List all received SMS from today."

**🤖 AI Agent:**
> Retrieving inbound messages... You received 3 replies today: 'Yes, I'm interested' from +1...99, 'Stop' from +1...22, and 'Thank you' from +1...44.

---

**👤 You:**
> "What is my current ClickSend balance?"

**🤖 AI Agent:**
> Checking your account balance... You currently have $25.40 available in your ClickSend account. This is enough for approximately 1,200 more local SMS messages.


## ❓ FAQ

**Q: Can I see the replies to my SMS messages through the agent?**
Yes! Use the `list_received_sms` tool. The agent will return all inbound SMS messages sent to your ClickSend numbers, allowing you to review customer replies.

**Q: How do I check how many credits I have left?**
Use the `get_clicksend_account_info` tool. Your agent will fetch your account details, which include your current balance for messaging and other services.

**Q: Where do I find my ClickSend API Key?**
Log in to your ClickSend dashboard and navigate to **Developers > API Credentials**. Your API Username and API Key are listed there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clicksend](https://vinkius.com/mcp/clicksend)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ClickSend** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clicksend` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ClickSend** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clicksend": {
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

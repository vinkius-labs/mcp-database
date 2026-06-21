# FreeClimb MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/freeclimb)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Build programmable voice and SMS workflows via AI agents with FreeClimb.

## Description
Connect your **FreeClimb** account to any AI agent to automate your telecommunications and customer engagement through the Model Context Protocol (MCP). FreeClimb provides a robust cloud platform for making calls, sending SMS messages, and managing programmable communication logic. This MCP server enables you to initiate calls, track message history, and oversee your phone numbers directly through natural conversation.

### Key Features

- **Programmable Voice** — Initiate outbound calls using application-defined logic and retrieve detailed call metadata.
- **SMS Messaging** — Send and receive text messages globally and monitor message delivery statuses instantly.
- **Application Oversight** — Access and list your communication applications to maintain full context of your bot's logic.
- **Number Management** — List owned phone numbers and search for new buyable numbers across different regions.
- **Conference Control** — Monitor active multi-party conferences and manage participant interactions.
- **Account Monitoring** — Retrieve real-time account status and balance information to ensure uninterrupted service.
- **Scalable Infrastructure** — Leverage FreeClimb's carrier-grade network directly from your chat interface.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your FreeClimb Account ID and API Key (found in your dashboard)
3. Start managing your voice and SMS workflows from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers & Engineers** — quickly test communication flows or send test alerts without leaving your IDE.
- **Support Teams** — automate the sending of follow-up SMS or check call history logs via simple AI commands.
- **Ops Managers** — monitor communication costs and manage phone number inventory through natural conversation.


## Available Tools
- **get_account_status**: Check account and balance
- **get_application_details**: Get app metadata
- **get_call_details**: Get call metadata
- **get_sms_details**: Get message metadata
- **list_applications**: List communication apps
- **list_buyable_numbers**: Search for new numbers
- **list_calls**: List recent calls
- **list_conferences**: List active conferences
- **list_my_numbers**: List owned phone numbers
- **list_sms_messages**: List sent/received SMS
- **make_call**: Place a phone call
- **send_sms**: Send an SMS message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **FreeClimb** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS from '+1234567890' to '+10987654321' saying 'Your appointment is confirmed'."

**🤖 AI Agent:**
> Message sent! I've successfully queued your SMS via FreeClimb. The message ID is 'msg_abc123'. I'll let you know if there are any delivery issues.

---

**👤 You:**
> "List all phone numbers currently in my FreeClimb account."

**🤖 AI Agent:**
> Retrieving numbers... I found 3 active phone numbers in your account, including '+1234567890' (Voice/SMS enabled).

---

**👤 You:**
> "Place a call from '+1234567890' to '+10987654321' using application 'app_987'."

**🤖 AI Agent:**
> Call initiated! I've started an outbound call via FreeClimb using app_987. The call ID is 'call_xyz789'. You can track its status in real-time.


## ❓ FAQ

**Q: How do I get my Account ID and API Key for FreeClimb?**
Log in to your FreeClimb dashboard at https://www.freeclimb.com/dashboard to find your credentials prominently displayed on the main page.

**Q: What is an 'Application ID' required for making calls?**
An Application ID points to a specific voice or SMS configuration in your FreeClimb account. You can list your active apps using the 'list_applications' tool.

**Q: Can I search for new phone numbers to buy?**
Yes, use the 'list_buyable_numbers' tool to see available inventory in the FreeClimb network.

**Q: Is global SMS supported?**
Yes, FreeClimb supports sending SMS messages to over 190 countries worldwide.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/freeclimb](https://vinkius.com/mcp/freeclimb)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **FreeClimb** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `freeclimb` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **FreeClimb** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "freeclimb": {
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

# TextGrid MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/textgrid)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Build voice and messaging applications with a CPaaS platform that offers programmable SMS, MMS, and voice APIs globally.

## Description
Connect your **TextGrid** account to any AI agent and simplify how you manage your cloud telephony, global messaging, and communication logs through natural conversation.

### What you can do

- **Global Messaging** — Send instant SMS and MMS messages to recipients worldwide with full status tracking.
- **Voice Call Control** — Initiate outbound voice calls and retrieve a complete history of inbound and outbound communication.
- **Phone Number Management** — List your active numbers and search for new available phone numbers across different countries.
- **Usage & Cost Tracking** — Retrieve detailed usage statistics and records to monitor your communication budget.
- **Account Oversight** — Fetch account metadata, API keys, and physical addresses for regulatory compliance.
- **Operational Monitoring** — Check API health and verify connectivity directly from the agent.

### How it works

1. Subscribe to this server
2. Enter your TextGrid Account SID and Auth Token (found in your account dashboard)
3. Start managing your cloud communications from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers & DevOps** — quickly test SMS delivery and initiate voice calls via simple AI commands.
- **Customer Support Teams** — retrieve message histories and verify delivery statuses directly from the workspace.
- **Operations Managers** — monitor usage costs and manage phone number inventory via the AI assistant.


## Available Tools
- **check_api_health**: Verify Textgrid API status
- **initiate_voice_call**: Start a new voice call
- **get_account_details**: Get account profile and balance
- **get_message_details**: Get details for a specific message
- **get_usage_statistics**: Retrieve usage and cost records
- **list_account_addresses**: List addresses for regulatory compliance
- **search_available_numbers**: Search for new phone numbers
- **list_voice_calls**: List voice call history
- **list_active_phone_numbers**: List your active phone numbers
- **list_api_keys**: List account API keys
- **list_sms_messages**: List sent and received SMS messages
- **send_sms_message**: Send a new SMS or MMS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TextGrid** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS to +15550199 saying 'Your verification code is 12345'."

**🤖 AI Agent:**
> SMS sent! I've triggered the message to +15550199 from your TextGrid number. The message SID is MSG-88231. Shall I track its delivery status for you?

---

**👤 You:**
> "Show me the last 3 voice calls from my history."

**🤖 AI Agent:**
> I've fetched your call history. You had: 1 Incoming from +123456 (Completed, 5m), 1 Outbound to +987654 (Failed), and 1 Incoming from Unknown (Missed). Would you like details on any specific call?

---

**👤 You:**
> "Search for available mobile numbers in the United Kingdom."

**🤖 AI Agent:**
> Fetching available numbers... I found 5 numbers available in the UK (Country Code: GB) including +447700... and +447701... Shall I retrieve the pricing and feature list for these?


## ❓ FAQ

**Q: Can I check the delivery status of a specific message via AI?**
Yes! Use the `get_message_details` tool and provide the Message SID. Your agent will retrieve the real-time delivery status (e.g., sent, delivered, failed) and other metadata.

**Q: How do I find a new available phone number in the US?**
Run the `search_available_numbers` query and set the `countryCode` parameter to 'US'. The agent will return a list of phone numbers available for purchase in that region.

**Q: Is it possible to see the costs associated with my messaging usage?**
Absolutely. Use the `get_usage_statistics` tool to retrieve detailed usage records and associated costs for your SMS and voice services directly from TextGrid.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/textgrid](https://vinkius.com/mcp/textgrid)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **TextGrid** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `textgrid` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **TextGrid** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "textgrid": {
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

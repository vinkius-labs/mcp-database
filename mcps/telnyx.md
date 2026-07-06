# Telnyx MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/telnyx)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Send and manage SMS/MMS, check account balances, and configure messaging profiles natively via your AI agent.

## Description
Connect your **Telnyx** account to any AI agent and manage your voice and messaging operations directly through natural conversation.

### What you can do

- **Send Messages** — Dispatch SMS and MMS texts, including media URLs, across your numbers in real-time
- **Check Delivery Status** — Look up message details and verify whether texts were successfully delivered or rejected
- **Manage Phone Numbers** — Browse your active E.164 phone numbers and retrieve configuration details
- **Messaging Profiles** — Create, update, list, and delete messaging profiles for your applications
- **Account Billing** — Monitor your exact account balance and available credits before dispatching campaigns

### How it works

1. Subscribe to this server
2. Enter your Telnyx API Key
3. Start managing telecom services strictly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Development teams** — debug messaging webhooks, check logs, and provision profiles quickly without leaving their IDE
- **Marketing managers** — trigger specific text campaigns or verify the balance before a massive SMS broadcast
- **Support tech** — investigate SMS delivery failures by retrieving precise message statues in seconds


## Available Tools (10)
- **delete_messaging_profile**: This action is irreversible.

Permanently deletes a messaging profile
- **get_account_balance**: Retrieves the current Telnyx account credit balance
- **get_message_details**: Retrieves details and delivery status for a specific message
- **get_number_settings**: Retrieves configuration and capability details for a specific phone number
- **get_messaging_profile_details**: Retrieves details for a specific messaging profile
- **list_phone_numbers**: 164 numbers and retrieve their unique IDs.

Lists all phone numbers owned by the account
- **list_messaging_profiles**: Lists all messaging profiles in the account
- **send_text_message**: Provide a registered Telnyx from_number and a target to_number in E.164 format.

Sends an outbound SMS message via Telnyx
- **create_messaging_profile**: Creates a new messaging profile
- **send_media_message**: Provide from/to numbers and a 100% public JPEG/PNG URL.

Sends an outbound MMS message with a media URL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Telnyx** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my current Telnyx account balance?"

**🤖 AI Agent:**
> Your current Telnyx account balance is $245.50. You possess sufficient credits to continue your standard outbound messaging and voice operations.

---

**👤 You:**
> "List all the phone numbers I currently own and their IDs."

**🤖 AI Agent:**
> I retrieved 2 active numbers from your account:
- +14155552671 (ID: 15b14eb1-XXXX)
- +14155559982 (ID: 39a48be9-XXXX)
Both are fully functional. Would you like to check the detailed settings for one of them?

---

**👤 You:**
> "Send a text message from +14155552671 to +12125550999 saying that the server is down."

**🤖 AI Agent:**
> The SMS has been successfully submitted to Telnyx for delivery.
From: +14155552671
To: +12125550999
Message: 'The server is down.'
Message UUID: 8e5f22e8-xxxx. Would you like me to check its real-time delivery status?


## ❓ FAQ

**Q: Can my AI agent check if a specific message was delivered?**
Yes. If an end user reports completely missing an important text, you can ask your agent to pull up the message status using its unique ID. The agent will read back exactly whether Telnyx successfully handed off the payload or if it encountered carrier-level rejection codes.

**Q: Is it possible to track the account billing balance?**
Absolutely. You can request your current Telnyx account balance to confirm you have enough credit left to continue broadcasting. Just ask 'What is my current Telnyx balance?' and your agent will give you the exact remaining dollar threshold.

**Q: Can I configure new Messaging Profiles via AI?**
Yes! Developers often need to isolate test traffic from production. You can simply ask your agent to list all current global profiles, and if needed, instruct it to immediately create a new messaging profile to attach webhook URLs.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/telnyx](https://vinkius.com/mcp/telnyx)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `telnyx` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Telnyx** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "telnyx": {
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

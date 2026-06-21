# Mitto MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mitto)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Automate SMS messaging and 2FA verification via Mitto — send single or bulk messages, verify OTPs, and lookup phone numbers directly from your AI agent.

## Description
Connect your **Mitto** account to any AI agent to handle global communication workflows through natural conversation.

### What you can do

- **SMS Messaging** — Send single or bulk SMS messages globally with custom sender IDs and delivery tracking.
- **Two-Factor Authentication (2FA)** — Generate, send, and verify OTP codes via SMS or Voice channels to secure your user accounts.
- **Number Lookup** — Validate phone numbers and retrieve carrier information to ensure deliverability.
- **Usage Analytics** — Monitor your SMS and 2FA usage statistics grouped by country or date ranges.
- **Application Management** — Manage your Mitto applications and masked numbers for privacy-focused communication.

### How it works

1. Subscribe to this server
2. Enter your Mitto API Key
3. Start sending messages and verifying users from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — integrate SMS notifications and 2FA into apps without leaving the IDE
- **Support Teams** — send quick updates or verification codes to customers via chat
- **Marketing Teams** — manage bulk SMS campaigns and track conversion rates directly


## Available Tools
- **add_masked_number**: Add a masked number
- **add_masking_participant**: Add a masking participant
- **cancel_2fa**: Cancel a 2FA OTP request
- **create_masking_application**: Create a number masking application
- **create_masking_context**: Create a masking context
- **delete_masking_application**: Delete a number masking application
- **delete_masking_context**: Delete a masking context
- **delete_masked_number**: Delete a masked number
- **delete_masking_participant**: Delete a masking participant
- **get_2fa_usage**: Get 2FA usage records
- **get_sms_usage_by_country**: Get SMS usage by country
- **list_masking_applications**: List number masking applications
- **list_masking_contexts**: List masking contexts
- **list_masked_numbers**: List masked numbers
- **list_masking_participants**: List masking participants
- **lookup_number**: Lookup mobile number information
- **search_2fa**: Search 2FA SDRs
- **search_masking_interactions**: Search masking interactions
- **send_2fa**: Send a 2FA OTP message
- **send_bulk_sms**: Send bulk SMS messages
- **send_sms**: Send a single SMS message
- **set_2fa_limits**: Set 2FA limits
- **set_2fa_workflows**: g., SMS to Voice) for 2FA.

Set 2FA workflows
- **track_sms_conversion**: Track SMS conversion
- **update_masking_application**: Update a number masking application
- **update_masking_context**: Update a masking context
- **verify_2fa**: Verify a 2FA OTP code


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mitto** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS to +1234567890 saying 'Your order is ready for pickup!' from 'MyStore'."

**🤖 AI Agent:**
> I've sent the SMS to +1234567890. The message ID is `msg_987654`. You can track its delivery status using this ID.

---

**👤 You:**
> "Send a 2FA verification code to +447700900123."

**🤖 AI Agent:**
> The 2FA code has been sent to +447700900123. Please provide the code once the user receives it, along with the Request ID: `req_abc123`.

---

**👤 You:**
> "Lookup the phone number +4915123456789 to see the carrier info."

**🤖 AI Agent:**
> I've looked up the number. It is a mobile number in Germany, currently served by 'Deutsche Telekom'. The number is valid and active.


## ❓ FAQ

**Q: Can I send an SMS to multiple phone numbers at the same time?**
Yes! Use the `send_bulk_sms` tool. You can provide an array of recipient numbers in E.164 format and a single message body to reach multiple users at once.

**Q: How do I verify a security code sent to a user?**
After sending a code with `send_2fa`, use the `verify_2fa` tool. You will need the `requestId` from the initial send and the `code` provided by the user to confirm their identity.

**Q: Can I check which countries I am sending the most messages to?**
Yes, the `get_sms_usage_by_country` tool allows you to retrieve usage statistics grouped by country, helping you analyze your global communication reach.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mitto](https://vinkius.com/mcp/mitto)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mitto** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mitto` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mitto** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mitto": {
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

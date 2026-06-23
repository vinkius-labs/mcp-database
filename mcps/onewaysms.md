# OneWaySMS MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/onewaysms)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Send bulk SMS messages across Asia Pacific with high delivery rates and real-time status tracking for every message.

## Description
Connect your **OneWaySMS** account to any AI agent and take full control of your global SMS orchestration through natural conversation. OneWaySMS provides a reliable and high-speed gateway for business messaging, and this integration allows you to send standard or Unicode SMS, monitor credit balances, and track delivery statuses directly from your chat interface.

### What you can do

- **SMS & Messaging Orchestration** — Send individual or bulk text messages programmatically to ensure your alerts and notifications are always synchronized.
- **Unicode & Multilingual Support** — Dispatch messages using standard ASCII or Unicode (for special characters and emojis) via natural language to reach your global audience.
- **Credit & Balance Intelligence** — Access and monitor your available SMS credit balance directly from the AI interface to ensure uninterrupted service.
- **Transaction & Delivery Control** — Retrieve real-time delivery status for any message using its unique Transaction ID (MTID) using simple AI commands.
- **Operational Monitoring** — Track system responses and manage regional gateway settings to ensure your communication pipeline is always optimized.

### How it works

1. Subscribe to this server
2. Enter your OneWaySMS API Username and API Password from your dashboard
3. Start managing your SMS communications from Claude, Cursor, or any MCP-compatible client

No more manual logging to check if a message was delivered. Your AI acts as a dedicated messaging coordinator or operations assistant.

### Who is this for?

- **Operations Managers** — quickly send emergency alerts and monitor credit usage without switching apps.
- **Customer Success Teams** — automate the delivery of status updates and track message reception via natural conversation.
- **Developers** — integrate real-time SMS capabilities and balance tracking directly within the chat.


## Available Tools (11)
- **check_api_connectivity**: Verify API connectivity
- **get_gateway_settings**: Get current API and gateway configuration
- **get_credit_balance**: Check remaining SMS credits
- **get_delivery_report**: Get a detailed delivery report for a message
- **get_transaction_status**: Track message delivery status
- **get_sms_usage_policy**: Retrieve character limits and regional policies
- **list_available_sender_ids**: List approved Alphanumeric Sender IDs
- **send_bulk_sms**: Send SMS to multiple recipients at once
- **send_otp**: Send a one-time verification code via SMS
- **send_sms**: Send a standard text message
- **send_unicode_sms**: ). Limit 70 chars per credit.

Send a Unicode text message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OneWaySMS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check my OneWaySMS credit balance."

**🤖 AI Agent:**
> I've retrieved your balance. You currently have 1,250 SMS credits available. Would you like to send a broadcast message?

---

**👤 You:**
> "Send a bulk SMS to our customer list with the message about our weekend flash sale."

**🤖 AI Agent:**
> Bulk SMS sent successfully to 156 recipients. Transaction ID: MT-29847. Message: "Weekend Flash Sale! 40% off everything this Saturday and Sunday. Shop now at example.com/sale". 3 credits consumed per message (468 total). Current remaining balance: 4,532 credits.

---

**👤 You:**
> "Check my current SMS credit balance and the delivery status of transaction MT-28341."

**🤖 AI Agent:**
> Your current credit balance is 4,532 SMS credits. Transaction MT-28341 status: Delivered successfully. The message was sent to +60123456789 on May 8th at 2:15 PM and confirmed delivered at 2:15:03 PM (3 second delivery time).


## ❓ FAQ

**Q: Can my AI automatically find the delivery status for a specific SMS by its transaction ID?**
Yes! Use the `get_status` tool with the Transaction ID (MTID). Your agent will respond with the current delivery state (e.g., Delivered, Failed, or Pending) in seconds.

**Q: How do I find my OneWaySMS API Username and Password?**
Log in to your OneWaySMS dashboard, navigate to the **API** section, and you will find your dedicated API Username and API Password (which are different from your web login).

**Q: What is the character limit for ASCII vs Unicode messages?**
Standard ASCII messages allow up to 160 characters per SMS. Unicode messages (which support special characters and emojis) are limited to 70 characters per SMS.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/onewaysms](https://vinkius.com/mcp/onewaysms)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **OneWaySMS** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `onewaysms` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **OneWaySMS** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "onewaysms": {
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

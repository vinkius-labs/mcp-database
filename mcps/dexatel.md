# Dexatel MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dexatel)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Equip your AI agent to send SMS messages, track communications, and manage contacts via the Dexatel API.

## Description
Integrate **Dexatel**, the comprehensive cloud communications platform, directly into your AI workflow. Send SMS messages globally, monitor your messaging logs and delivery statuses, and manage your contact database using natural language.

### What you can do

- **Messaging Control** — Send and receive SMS messages using your authorized Sender IDs and virtual numbers.
- **Delivery Oversight** — Monitor messaging logs in real-time, including technical delivery timestamps and carrier info.
- **Contact Management** — Access and manage your address book, including profiles and messaging history for specific contacts.
- **Balance Monitoring** — Track your account credit balance and API usage directly via chat.

### How it works

1. Connect the Dexatel integration to your AI assistant.
2. Authorize using your Dexatel API Key (found in your account settings).
3. Orchestrate your global communications through intuitive conversation.

### Who is this for?

- **Marketing Teams** — Quickly check campaign delivery statuses and message logs on the go.
- **Support Operations** — Access contact profiles and messaging history during customer resolution.
- **Business Owners** — Send notifications and monitor credit balances via chat instantly.


## Available Tools
- **get_account_balance_metadata**: Retrieve current balance and metadata for your Dexatel account
- **get_contact_profile**: Get full profile and history for a specific contact
- **get_sms_message_details**: Get detailed information for a specific SMS message
- **list_messaging_contacts**: List all contacts stored in your Dexatel address book
- **list_failed_sms_deliveries**: Identify SMS messages that failed to deliver (mock logic)
- **list_sms_messages**: List all sent and received SMS messages in your Dexatel account
- **list_authorized_sender_ids**: List all authorized Sender IDs and virtual numbers
- **list_sms_templates**: List all approved message templates
- **search_sms_by_content**: Search for SMS messages containing specific keywords or numbers
- **send_sms_message**: Send a new SMS message to a specific number


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dexatel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS to '+1234567890' saying 'Your order is ready!'."

**🤖 AI Agent:**
> I've successfully sent the SMS to +1234567890. The message ID is 12345. Would you like me to track its delivery status for you?

---

**👤 You:**
> "Show me the last 5 sent messages."

**🤖 AI Agent:**
> The last 5 sent messages include notifications to '+123...' and '+198...'. All are marked as 'Delivered'. Should I pull the full content for any of them?

---

**👤 You:**
> "What is my current account balance?"

**🤖 AI Agent:**
> Your current balance is $45.20. You have approximately 3,000 SMS credits remaining based on your current rates. Would you like to see your usage for this month?


## ❓ FAQ

**Q: How do I get a Dexatel API Key?**
Log in to your Dexatel account, navigate to **Settings > API**, and you can retrieve your unique API Key from that section.

**Q: Can the agent receive SMS messages?**
Yes, you can use the list_sms_messages tool to view both sent and received messages in your account history.

**Q: Does the integration show real-time delivery status?**
Yes, when retrieving message details, the agent provides the latest status (e.g., delivered, pending, failed) as reported by the Dexatel platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dexatel](https://vinkius.com/mcp/dexatel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dexatel** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dexatel` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dexatel** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dexatel": {
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

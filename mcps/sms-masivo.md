# SMS Masivo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sms-masivo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Send bulk SMS campaigns across Latin America with delivery tracking, contact segmentation, and competitive local pricing.

## Description
Connect your **SMS Masivo** account to any AI agent and automate your SMS communications through natural conversation.

### What you can do

- **Send SMS** — Send individual messages to any international phone number.
- **Bulk Messaging** — Send the same message to multiple recipients at once.
- **Scheduled Delivery** — Schedule SMS for future delivery at a specific date and time.
- **Delivery Reports** — Track real-time delivery status for individual or batch messages.
- **Contacts** — Manage your contact directory and create new entries.
- **Groups** — View contact groups for campaign targeting.
- **Balance** — Check your available SMS credits.

### How it works

1. Subscribe to this server
2. Enter your SMS Masivo API key
3. Start sending messages from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing Teams** — send bulk SMS campaigns and track delivery rates.
- **Customer Support** — send transactional notifications and appointment reminders.
- **Sales Teams** — automate follow-up messaging with scheduled delivery.


## Available Tools
- **check_smsmasivo_status**: Verify SMS Masivo API connectivity
- **create_contact**: Create a new contact
- **get_balance**: Check your SMS credit balance
- **get_delivery_report**: Get the delivery report for a specific message
- **list_contacts**: List all contacts in your account
- **list_delivery_reports**: List delivery reports by date range
- **list_groups**: List all contact groups
- **schedule_sms**: Provide the date in ISO 8601 format.

Schedule an SMS for future delivery
- **send_bulk_sms**: Provide comma-separated numbers in international format.

Send the same SMS to multiple recipients
- **send_sms**: Optionally provide a campaign name for tracking.

Send an SMS message to a single recipient


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SMS Masivo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS to +573001234567 saying 'Your appointment is confirmed for tomorrow at 2 PM'."

**🤖 AI Agent:**
> SMS sent successfully! Transmission ID: TX-20250115-001. Message delivered to +573001234567. Use the ID to check delivery status later.

---

**👤 You:**
> "Check my SMS credit balance."

**🤖 AI Agent:**
> Your current balance is 2,450 SMS credits. At your current send rate, this should last approximately 3 weeks.

---

**👤 You:**
> "Send a bulk SMS to +573001234567, +573009876543, +573005551234 with the message 'Holiday sale starts tomorrow!'."

**🤖 AI Agent:**
> Bulk SMS sent to 3 recipients! All messages dispatched successfully. Campaign: 'Holiday sale'. Transmission IDs available for delivery tracking.


## ❓ FAQ

**Q: Can I send SMS to multiple recipients at once?**
Yes! Use `send_bulk_sms` with a comma-separated list of phone numbers in international format. All recipients receive the same message.

**Q: How do I check if my message was delivered?**
Use `get_delivery_report` with the transmission ID returned when the SMS was sent. It shows real-time delivery status (delivered, pending, failed).

**Q: Can I schedule messages for later?**
Yes! Use `schedule_sms` with the delivery date in ISO 8601 format (e.g., 2025-01-15T14:00:00Z). The message will be sent at the specified time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sms-masivo](https://vinkius.com/mcp/sms-masivo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SMS Masivo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `sms-masivo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SMS Masivo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sms-masivo": {
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

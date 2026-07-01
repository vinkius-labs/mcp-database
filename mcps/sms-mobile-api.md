# SMS Mobile API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sms-mobile-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Send SMS and WhatsApp messages directly from your Android devices with AI agents.

## Description
Connect your **SMS Mobile API** account to any AI agent to automate your mobile messaging and device orchestration. SMS Mobile API turns your Android phone into a powerful messaging gateway, and this integration allows you to send SMS, manage WhatsApp communications, and track missed calls through natural conversation.

### What you can do

- **Messaging Orchestration** — Send instant SMS and WhatsApp messages using your own mobile number and data plan programmatically.
- **Device & Gateway Control** — List and monitor your connected Android devices to ensure your messaging gateway is always online.
- **Incoming Communication Tracking** — Retrieve received SMS messages and list missed calls to keep your conversational threads synchronized directly from the AI interface.
- **Multi-Port Support** — Manage messaging across different device ports and gateways to maintain high delivery rates via natural language.
- **Operational Monitoring** — Track message delivery status and monitor device connectivity to ensure reliable customer outreach.

### How it works

1. Subscribe to this server
2. Enter your SMSMobileAPI Key from your dashboard or mobile app
3. Start managing your mobile messaging from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Small Business Owners** — quickly send personalized customer notifications using your own mobile plan without switching apps.
- **Support Teams** — automate the retrieval of incoming SMS and monitor missed calls via natural conversation.
- **Developers** — integrate local mobile messaging capabilities into custom AI-driven business workflows.


## Available Tools (11)
- **get_account_info**: Get account information and usage statistics
- **get_delivery_status**: Get delivery status for a sent message
- **get_device**: Get details for a specific connected device
- **list_contacts**: List all saved contacts
- **list_sent_messages**: List all sent messages
- **send_mms**: Send an MMS message with media attachment
- **get_received_sms**: Get incoming SMS messages
- **list_connected_devices**: List connected mobile gateways
- **list_missed_calls**: List missed calls log
- **send_sms**: Send SMS from your phone
- **send_whatsapp**: Send WhatsApp from your phone


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SMS Mobile API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS to +1234567890: 'Your order is ready for pickup!'."

**🤖 AI Agent:**
> SMS triggered successfully! I've sent the pickup notification through your connected Android device via SMS Mobile API.

---

**👤 You:**
> "Send an SMS notification to all customers about our system maintenance window tonight."

**🤖 AI Agent:**
> SMS broadcast sent. Recipients: 234 customers. Message: "System maintenance tonight 11 PM - 3 AM EST. Services may be briefly unavailable. We apologize for any inconvenience. Status page: status.yourapp.com". Delivery: 229 delivered (97.9%), 3 undeliverable (invalid numbers), 2 pending. Character count: 148 (1 SMS segment). Cost: $11.70 ($0.05/msg). Device used: Primary Gateway (iPhone, device_001). Delivery receipts will be available within 30 minutes.

---

**👤 You:**
> "Show me all received SMS messages and missed calls from the last 48 hours."

**🤖 AI Agent:**
> Received SMS (last 48h): 34 messages. Support requests: 12 (keywords: "help", "issue", "broken"). Order confirmations: 8 (auto-forwarded to CRM). Appointment confirmations: 6 ("YES" replies). Opt-out requests: 3 ("STOP" - auto-processed). General inquiries: 5. Missed calls: 8 total. From known contacts: 5 (3 customers, 2 suppliers). Unknown numbers: 3. Peak incoming: yesterday 10 AM (7 messages in 1 hour). Auto-responses sent: 15 (after-hours acknowledgment).


## ❓ FAQ

**Q: How do I find my SMSMobileAPI Key?**
Log in to the [**SMS Mobile API web dashboard**](https://smsmobileapi.com/dashboard) or open the Android app and navigate to the Settings or Help section to find your unique API Key.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sms-mobile-api](https://vinkius.com/mcp/sms-mobile-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SMS Mobile API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sms-mobile-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SMS Mobile API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sms-mobile-api": {
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

# Plivo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/plivo-extended)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Build voice and SMS applications with a cloud communications API that scales globally and offers competitive per-message pricing.

## Description
Connect your **Plivo** communications account to any AI agent and take full control of your global telephony and messaging orchestration through natural conversation. Plivo provides a world-class platform for SMS and Voice services, and this integration allows you to send text messages, retrieve call logs, and manage rented phone numbers directly from your chat interface.

### What you can do

- **SMS & Messaging Orchestration** — Send and monitor SMS and MMS messages globally programmatically to ensure your customer engagement is always synchronized.
- **Call Monitoring Intelligence** — Query all recorded call logs and retrieve real-time metadata, including duration, cost, and status metrics directly from the AI interface.
- **Number Management Control** — List all rented phone numbers and manage their configurations via natural language to maintain a clear overview of your communication reach.
- **XML Application Oversight** — List and oversee your configured Plivo applications to understand your automated call and message handling logic using simple AI commands.
- **Operational Monitoring** — Retrieve account profile information, balance, and credits to ensure your communication pipeline is always optimized.

### How it works

1. Subscribe to this server
2. Enter your Plivo Auth ID and Auth Token from your console dashboard
3. Start managing your communications from Claude, Cursor, or any MCP-compatible client

No more manual logging into dashboards to check message delivery. Your AI acts as a dedicated telephony administrator or communication assistant.

### Who is this for?

- **Support Teams** — quickly retrieve message statuses and check call logs to resolve customer inquiries faster without switching apps.
- **Operations Leads** — automate the retrieval of number usage and track account balances via natural conversation.
- **Developers** — integrate real-time telephony data and application metadata directly within the chat.


## Available Tools
- **get_number_details**: Get details for a specific phone number
- **get_recording**: Get details for a specific recording
- **list_recordings**: List all call recordings
- **get_account_info**: Retrieve current Plivo account details
- **get_call_details**: Get details for a specific call
- **get_message_details**: Get details for a specific message
- **list_applications**: List all Plivo XML applications
- **list_calls**: List all call logs
- **list_messages**: List all message logs
- **list_numbers**: List all rented phone numbers
- **send_sms**: Requires a verified Plivo source number or Sender ID and the recipient number in E.164 format.

Send a new SMS message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Plivo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my last 5 SMS messages on Plivo."

**🤖 AI Agent:**
> I've retrieved your messages. You have 5 recent entries including an SMS to '+1234567890' (Status: Delivered) and an incoming text from '+0987654321'. Which one would you like to see details for?

---

**👤 You:**
> "Send an SMS notification to all customers in the delivery queue with their tracking numbers."

**🤖 AI Agent:**
> Bulk SMS sent successfully. 47 messages dispatched from your Plivo number +1-555-0142. Delivery status: 44 delivered, 2 queued, 1 failed (invalid number). Average delivery time: 1.3 seconds. Message template: "Your order is on its way! Track it here: [tracking_url]". Cost: $0.0075 per message, total: $0.35. 3 recipients opted out of future messages.

---

**👤 You:**
> "Show me all phone numbers in my Plivo account with their capabilities and monthly costs."

**🤖 AI Agent:**
> You have 6 active phone numbers. +1-555-0142 (US): Voice + SMS, $1.00/mo, used for transactional alerts. +44-20-7946-0958 (UK): Voice + SMS, $1.50/mo, customer support line. +1-555-0187 (US toll-free): Voice only, $2.00/mo, sales hotline. +91-22-4000-1234 (India): SMS only, $0.50/mo, OTP verification. 2 additional numbers in Canada and Germany. Total monthly cost: $8.50.


## ❓ FAQ

**Q: Can my AI automatically find the details of a specific message by its UUID?**
Yes! Use the `get_message` tool with the Message UUID. Your agent will respond with complete metadata, including delivery status, timestamps, and cost in seconds.

**Q: How do I find my Plivo Auth ID and Auth Token?**
Log in to your [**Plivo Console Dashboard**](https://console.plivo.com/dashboard/), and you will find your unique Auth ID and Auth Token displayed prominently on the main page.

**Q: Does this work for international messaging?**
Absolutely. Plivo supports global SMS and Voice services. As long as your account has the required credits and permissions, the AI can trigger communications to any supported destination.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/plivo-extended](https://vinkius.com/mcp/plivo-extended)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Plivo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `plivo-extended` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Plivo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "plivo-extended": {
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

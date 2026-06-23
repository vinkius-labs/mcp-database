# Clickatell MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/clickatell-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Deliver transactional and marketing messages over SMS, WhatsApp, and chat channels with global reach and high deliverability.

## Description
Connect your **Clickatell One API** account to any AI agent and take full control of your global business communication and automated notification workflows through natural conversation.

### What you can do

- **Multichannel Messaging Orchestration** — Instantly dispatch high-fidelity SMS and official WhatsApp messages to customers worldwide using a single unified interface
- **Delivery Intelligence** — Monitor real-time status (sent, delivered, read) for all messages and retrieve detailed historical logs to maintain high-fidelity oversight
- **WhatsApp Template Management** — Access and monitor pre-approved message templates and manage multimedia content to ensure perfectly coordinated business engagement
- **Financial Visibility** — Programmatically track your account balance and credit utilization to coordinate your global messaging budget and quotas
- **Source Architecture** — Access complete directories of your configured sending numbers and communication channels directly through your agent

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Clickatell Workspace (My Workspace > API Integrations)
3. Start automating your customer notifications and engagement from Claude, Cursor, or any MCP client

No more manual message tracking or toggling between different messaging portals. Your AI acts as your dedicated CPaaS engineer and communication coordinator.

### Who is this for?

- **Customer Support Teams** — instantly send personalized order updates and verification codes using natural language commands
- **Growth Marketers** — automate multichannel broadcast campaigns and monitor read rates without leaving your workspace
- **Developers & Ops** — integrate high-speed SMS and WhatsApp features into custom workflows through simple AI queries


## Available Tools (12)
- **get_message_status**: Check delivery status
- **list_active_channels**: ) in the account.

List communication channels
- **list_message_history**: List past messages
- **list_source_numbers**: List sending numbers
- **list_whatsapp_templates**: List WhatsApp templates
- **send_bulk_messages**: Send multiple messages
- **send_sms**: Send SMS message
- **send_whatsapp**: Note: Templates required for business initiation.

Send WhatsApp message
- **delete_whatsapp_template**: Remove template
- **get_account_info**: Get profile details
- **get_account_balance**: Check credit balance
- **get_whatsapp_media**: Get media details


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Clickatell** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send a WhatsApp notification to '+447911123456': 'Your package has been delivered'."

**🤖 AI Agent:**
> WhatsApp message dispatched! I've successfully sent the delivery notification to +447911123456. The status is currently 'Sent'. Shall I alert you as soon as it's delivered?

---

**👤 You:**
> "Check the delivery status for message ID 'omni_12345'."

**🤖 AI Agent:**
> Fetching status... Message omni_12345 has been successfully 'Delivered' and was 'Read' by the recipient at 2:30 PM today. Would you like to see the full interaction history?

---

**👤 You:**
> "What is my current Clickatell account balance?"

**🤖 AI Agent:**
> Scanning account... Your current balance is $25.50. Based on your recent usage, you have enough credits for approximately 1,200 SMS messages. Need a breakdown of recent sending costs?


## ❓ FAQ

**Q: How do I find my Clickatell API Key?**
Log in to your Clickatell account, navigate to **My Workspace** > **API Integrations**, and create a new HTTP API integration to get your key.

**Q: Do I need templates for WhatsApp?**
Yes, for business-initiated messages, WhatsApp requires the use of pre-approved templates. You can list them using the `list_whatsapp_templates` tool.

**Q: Can I check my remaining balance via AI?**
Yes! The `get_account_balance` tool retrieves your current remaining funds directly from the Clickatell platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/clickatell-alternative](https://vinkius.com/mcp/clickatell-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Clickatell** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `clickatell-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Clickatell** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "clickatell-alternative": {
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

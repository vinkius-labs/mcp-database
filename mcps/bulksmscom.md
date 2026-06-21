# BulkSMS.com MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/bulksmscom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Reach customers worldwide with reliable bulk SMS delivery, contact list management, and real-time message status tracking.

## Description
Connect your **BulkSMS.com** account to any AI agent and take full control of your global business communication and automated SMS workflows through natural conversation.

### What you can do

- **Messaging Orchestration** — Instantly dispatch high-fidelity SMS messages to over 800 networks worldwide using a single unified interface
- **Communication Intelligence** — Monitor real-time status and retrieve detailed historical logs for all sent and received messages to maintain high-fidelity oversight
- **Audience Management** — Programmatically manage your contact groups and subscriber profiles to ensure perfectly coordinated business engagement
- **Financial Visibility** — Programmatically track your account balance and credit utilization to coordinate your global messaging budget and quotas
- **Operational Monitoring** — Access account profile metadata and verify API connectivity directly through your agent for instant performance reporting

### How it works

1. Subscribe to this server
2. Retrieve your **Token ID** and **Token Secret** from your BulkSMS dashboard (Settings > Developers > API Tokens)
3. Start automating your customer notifications and engagement from Claude, Cursor, or any MCP client

No more manual message tracking or digging through complex delivery reports. Your AI acts as your dedicated SMS operations and communication coordinator.

### Who is this for?

- **Customer Support Teams** — instantly send personalized order updates and verification codes using natural language commands
- **Growth Marketers** — automate multichannel broadcast campaigns and monitor delivery rates without leaving your workspace
- **Operations Leads** — track credit utilization and manage contact groups through simple AI queries


## Available Tools (12)
- **check_bulksms_status**: Verify connectivity
- **create_contact**: Create a contact
- **delete_message**: Delete a message
- **get_credits**: Get credits balance
- **get_delivery_status**: Get delivery status
- **get_message**: Get message details
- **get_profile**: Get profile
- **list_contacts**: List contacts
- **list_groups**: List contact groups
- **list_messages**: List messages
- **send_bulk_sms**: Send bulk SMS
- **send_sms**: Send an SMS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BulkSMS.com** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS to +1234567890: 'Your order is ready for pickup'."

**🤖 AI Agent:**
> SMS dispatched! I've sent the notification to +1234567890 via BulkSMS.com. The message is queued for delivery. Shall I check your remaining credits?

---

**👤 You:**
> "List my last 5 sent messages and their status."

**🤖 AI Agent:**
> Accessing logs... Your last 5 messages include a delivery to @user1 (Status: Delivered) and 4 others. I've retrieved the detailed timestamps for each interaction.

---

**👤 You:**
> "What is my current BulkSMS credit balance?"

**🤖 AI Agent:**
> Scanning account... Your current balance is 1,240.50 credits. Based on your recent usage, you are in good standing for your next campaign. Need any help with a new broadcast?


## ❓ FAQ

**Q: How do I find my BulkSMS Token ID and Secret?**
Log in to BulkSMS, navigate to **Settings** > **Developers** > **API Tokens**, and generate a new token to get your ID and Secret.

**Q: Can I manage contact groups via AI?**
The current toolset focuses on messaging and credit checks. You can query your account profile to see high-level metadata about your groups.

**Q: How do I check my remaining balance?**
Use the `get_credit_balance` tool to retrieve your current remaining funds directly from the BulkSMS platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/bulksmscom](https://vinkius.com/mcp/bulksmscom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BulkSMS.com** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bulksmscom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BulkSMS.com** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bulksmscom": {
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

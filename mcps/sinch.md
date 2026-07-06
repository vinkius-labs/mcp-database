# Sinch MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sinch)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Enable your AI agent to send SMS messages, monitor delivery reports, and manage contact groups via the Sinch API.

## Description
Connect your AI to **Sinch**, the global cloud communications platform for SMS messaging at scale.

### What you can do

- **Send Messages** — Dispatch individual or bulk SMS messages to any phone number or contact group.
- **Delivery Tracking** — Check delivery reports to see which messages were delivered, pending, or failed.
- **Batch Management** — List, update, or cancel SMS batches before they're delivered.
- **Contact Groups** — Create and manage contact groups for targeted campaign messaging.

### How it works

1. Add the Sinch integration to your AI toolset.
2. Provide your Service Plan ID and API Token.
3. Send and manage SMS campaigns via natural language.

### Who is this for?

- **Marketing Teams** — Launch SMS campaigns and track delivery rates from chat.
- **Customer Support** — Send transactional messages and verify delivery status instantly.
- **Developers** — Automate SMS workflows and integrate messaging into pipelines.


## Available Tools (10)
- **create_sms_group**: Creates a new contact group
- **delete_sms_group**: This action is irreversible.

Permanently deletes a contact group
- **get_batch_details**: Retrieves details for a specific SMS batch
- **get_delivery_report**: Retrieves a delivery report for a specific batch
- **get_group_details**: Retrieves details for a specific contact group
- **list_sms_batches**: Lists recent SMS batches
- **list_sms_groups**: Lists all contact groups
- **send_sms**: You can provide multiple phone numbers in the "to" field. Ensure numbers are in international format (e.g., +1234567890).

Sends a text message (SMS) to one or more recipients
- **update_sms_batch**: Updates parameters of an existing SMS batch
- **cancel_sms_batch**: This action is irreversible for the remaining messages.

Cancels a pending SMS batch


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sinch** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Send an SMS to +1234567890 saying 'Your order has been shipped!'"

**🤖 AI Agent:**
> SMS sent successfully.
- Batch ID: batch-7k2m
- Recipient: +1234567890
- Message: 'Your order has been shipped!'
- Status: queued for delivery

---

**👤 You:**
> "Get the delivery report for batch 9876."

**🤖 AI Agent:**
> Delivery report for batch 9876:
- Total recipients: 12,000
- Delivered: 11,842 (98.7%)
- Pending: 112
- Failed: 46
- Sender ID: 'Vinkius'
Would you like details on the failed deliveries?


## ❓ FAQ

**Q: Can it accidentally affect my entire Sinch account?**
No. The integration only supports sending SMS, managing batches, and handling contact groups. It cannot modify billing, account settings, or access other Sinch services.

**Q: How does authentication work?**
You provide your Service Plan ID and API Token. The integration generates a Bearer token header automatically for each request — no OAuth setup required.

**Q: What is a batch in Sinch?**
A batch is a single SMS send operation that can target one or many recipients. Each batch has a unique ID and can be tracked, updated, or cancelled before delivery.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sinch](https://vinkius.com/mcp/sinch)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sinch** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sinch` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sinch** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sinch": {
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

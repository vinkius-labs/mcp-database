# eSputnik MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/esputnik)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing](../categories/marketing.md)

Omnichannel marketing automation with eSputnik.

## Description
The eSputnik MCP server allows your AI agent to orchestrate marketing campaigns across Email, SMS, Web Push, and Mobile Push. Send messages, retrieve contact lists, and manage omnichannel workflows seamlessly.


## Available Tools (12)
- **attach_to_group**: Add contacts to a specific group
- **create_contact**: Create a new contact in eSputnik
- **detach_from_group**: Remove contacts from a group
- **get_account_info**: Retrieve account and organization metadata
- **get_contact**: Retrieve details for a specific contact
- **get_message_status**: Check the delivery status of a sent message
- **list_contacts**: List all contacts in eSputnik
- **list_groups**: List all contact groups/segments
- **list_unsubscribed**: List unsubscribed email addresses
- **search_contacts**: Search for contacts by email or phone
- **send_smart_send**: Trigger an omnichannel message send
- **trigger_event**: Generate a system event to trigger workflows


## 💬 Prompt Examples

Here are some examples of how you can interact with the **eSputnik** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my contact groups in eSputnik."

**🤖 AI Agent:**
> I've retrieved your segments. You have 3 groups: 'VIP Customers', 'Newsletter Subs', and 'Inactive Users'.

---

**👤 You:**
> "Send an SMS saying 'Your order has shipped!' to +123456789."

**🤖 AI Agent:**
> The SMS has been successfully dispatched to +123456789 via eSputnik.

---

**👤 You:**
> "Add 'john@example.com' to the 'VIP Customers' list."

**🤖 AI Agent:**
> Contact 'john@example.com' was successfully added to the 'VIP Customers' group.


## ❓ FAQ

**Q: Can I send transactional SMS messages via the AI agent?**
Yes! You can specify the recipient's phone number and the message content, and the AI will trigger the eSputnik SMS endpoint.

**Q: How do I query my contact segments?**
Ask the agent to 'List all contact groups'. It will retrieve your active segments directly from the eSputnik API.

**Q: Does it support adding new contacts dynamically?**
Absolutely. You can request the AI to add an email or phone number to your active directory instantly.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/esputnik](https://vinkius.com/mcp/esputnik)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **eSputnik** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `esputnik` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **eSputnik** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "esputnik": {
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

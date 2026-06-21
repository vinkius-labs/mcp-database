# WA Smart Business MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wa-smart-business)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Automate WhatsApp marketing and communication via WA Smart Business — manage contacts, groups, and messages directly from any AI agent.

## Description
Connect your **WA Smart Business** account to any AI agent and simplify your WhatsApp automation and customer engagement through natural conversation.

### What you can do

- **Contact Management** — List all customers, retrieve detailed profile metadata, and create new contacts programmatically
- **Messaging & Outreach** — Send text messages or templates to recipients and monitor delivery through your agent
- **Group & Agent Tracking** — List managed WhatsApp groups and configured support agents to understand your organization
- **Template catalog** — Query available pre-approved message templates for quick outreach

### How it works

1. Subscribe to this server
2. Enter your WA Smart Business API Key from your dashboard
3. Start managing your WhatsApp automation from Claude, Cursor, or any MCP-compatible client


## Available Tools (7)
- **create_contact**: Create a new WhatsApp contact
- **get_contact**: Get details for a specific contact
- **list_agents**: List support agents
- **list_contacts**: List WA Smart Business contacts
- **list_groups**: List WhatsApp groups
- **list_templates**: List message templates
- **send_message**: Send a WhatsApp message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WA Smart Business** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add a new lead named 'Carlos Oliveira' with phone '+5511987654321' to our WA Smart Business contacts, and send him a welcome message saying our team will contact him shortly."

**🤖 AI Agent:**
> I have created the contact for 'Carlos Oliveira' successfully. I also sent the welcome message to '+5511987654321'. The delivery status confirms the message was dispatched.

---

**👤 You:**
> "Retrieve all pre-approved WhatsApp message templates we can use for the upcoming holiday promotion."

**🤖 AI Agent:**
> I found 4 approved templates in your account, including 'holiday_sale_announce', 'black_friday_vip', 'abandoned_cart_reminder', and 'shipping_update'. Would you like to use one of these to broadcast to a specific group?

---

**👤 You:**
> "List all active WhatsApp support groups we currently manage through the platform."

**🤖 AI Agent:**
> You are currently managing 3 WhatsApp groups: 'VIP Support Channel', 'Beta Testers Community', and 'LatAm Partners'. Would you like me to fetch the contact list for any of these?


## ❓ FAQ

**Q: Can I list all my WhatsApp contacts using my AI agent?**
Yes! Use the `list_contacts` tool. It will return a comprehensive list of all customers and contacts registered in your portal.

**Q: How do I send a WhatsApp message through this integration?**
Simply use the `send_message` action by providing the recipient's phone number and your message body or template data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wa-smart-business](https://vinkius.com/mcp/wa-smart-business)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WA Smart Business** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wa-smart-business` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WA Smart Business** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wa-smart-business": {
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

# 2Chat MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/2chat)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Programmable WhatsApp automation — send messages, manage groups, and verify numbers via AI.

## Description
Unlock the full potential of WhatsApp automation with **2Chat**, the programmable gateway now integrated with your AI agent. By connecting 2Chat via the Model Context Protocol, you transcend the limitations of traditional messaging apps. Your agent can now orchestrate complex group workflows, verify phone numbers before sending, and manage multi-device communications through simple natural language. Whether you're coordinating team alerts or engaging with a community, 2Chat gives your AI the 'voice' it needs on the world's most popular messaging platform.

### What you can do

- **Programmable Messaging** — Send text, images, PDF, and voice messages to any WhatsApp number without template restrictions.
- **Group Management** — Create groups, add participants, and send group-wide announcements directly from your chat interface.
- **Number Verification** — Check if a phone number is registered on WhatsApp before sending to improve delivery success.
- **Webhooks & Real-time** — Monitor incoming messages and delivery status (sent, delivered, read) seamlessly.
- **Multi-Device Support** — Link multiple WhatsApp numbers to a single API workspace for unified communications.

### How it works

1. Subscribe to this server
2. Enter your 2Chat API Key
3. Start managing your WhatsApp communications through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Teams** — run flexible campaigns and engage with customers in groups
- **Developers** — build custom WhatsApp workflows with a straightforward REST API
- **Operations Managers** — automate internal team notifications via WhatsApp groups
- **Community Managers** — manage large WhatsApp communities and announcements with ease


## Available Tools
- **list_numbers**: Use this to identify which "from_number" to use in subsequent sending actions.

List all WhatsApp phone numbers connected to your 2Chat account
- **send_message**: Can send text or public URL media to direct numbers or a specific group UUID.

Send a WhatsApp text or media message using a connected number
- **check_number**: Helps prevent failed delivery errors.

Verify if a phone number is registered on WhatsApp
- **create_group**: Create a new WhatsApp group with specified participants
- **list_groups**: List all WhatsApp groups that a connected number belongs to


## 💬 Prompt Examples

Here are some examples of how you can interact with the **2Chat** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if +123456789 is registered on WhatsApp and send a message saying hello."

**🤖 AI Agent:**
> I've verified that +123456789 is a valid WhatsApp number. Your 'hello' message has been sent successfully through 2Chat.

---

**👤 You:**
> "List all my WhatsApp groups."

**🤖 AI Agent:**
> I've retrieved your WhatsApp groups from 2Chat. You are a member of 'Development Team', 'Marketing Updates', and 'Project Alpha'. Which group would you like to interact with?

---

**👤 You:**
> "Create a new WhatsApp group called 'Project Gamma' and add participant +198765432."

**🤖 AI Agent:**
> The group 'Project Gamma' has been successfully created and +198765432 has been added as a participant. You can now send messages to this group through 2Chat.


## ❓ FAQ

**Q: Can I manage WhatsApp groups with this server?**
Yes! 2Chat provides dedicated tools to create groups, list groups your number belongs to, and send messages to group UUIDs.

**Q: Do I need official WhatsApp Business API approval?**
No. 2Chat works by linking your existing WhatsApp number (Personal or Business) via a QR code, so you don't need official Meta approval or template restrictions.

**Q: How can I check if a number is on WhatsApp?**
You can use the `check_number` tool to verify if a specific phone number is registered on WhatsApp before attempting to send a message.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/2chat](https://vinkius.com/mcp/2chat)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **2Chat** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `2chat` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **2Chat** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "2chat": {
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

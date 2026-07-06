# DoubleTick MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/doubletick-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Scale your WhatsApp sales with bulk messaging, chatbot automation, and team inbox features built for growing businesses.

## Description
Connect your **DoubleTick** account to any AI agent and take full control of your official WhatsApp Business marketing and sales workflows through natural conversation.

### What you can do

- **Template Orchestration** — List and manage approved WhatsApp message templates, including retrieving detailed metadata about languages and categories programmatically
- **High-Engagement Messaging** — Programmatically send template messages with dynamic placeholders to coordinate personalized customer outreach at scale
- **Delivery Intelligence** — Monitor real-time status (sent, delivered, read) for all messages to maintain high-fidelity communication oversight
- **Contact Lifecycle** — Programmatically create and manage your WhatsApp contact list to maintain an organized and segmented audience
- **Group & Team Visibility** — Access your directory of WhatsApp groups to understand team collaboration environments directly through your agent

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from DoubleTick dashboard (Settings > Developer API)
3. Start managing your WhatsApp Business growth from Claude, Cursor, or any MCP client

No more manual template copy-pasting or slow message tracking in the dashboard. Your AI acts as your dedicated WhatsApp operations and engagement coordinator.

### Who is this for?

- **Sales Teams** — instantly send personalized order updates and follow-ups via WhatsApp using natural language commands
- **Growth Marketers** — automate template-based broadcast campaigns and monitor read rates without leaving your workspace
- **Support Leads** — track message delivery status and manage customer contact lists through simple AI queries


## Available Tools (6)
- **get_message_status**: Check message delivery status
- **list_groups**: List WhatsApp groups
- **list_templates**: List WhatsApp templates
- **send_template_message**: Pass placeholders as a JSON string.

Send a WhatsApp template message
- **create_contact**: Create a new contact
- **list_contacts**: List WhatsApp contacts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DoubleTick** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my approved WhatsApp templates in DoubleTick."

**🤖 AI Agent:**
> I've retrieved your approved templates. You currently have 5 active designs, including 'order_confirmation' (en) and 'welcome_message' (pt). Which one would you like to use for a message?

---

**👤 You:**
> "Send the 'order_update' template to +123456789 with value 'Shipped'."

**🤖 AI Agent:**
> Message dispatched! I've sent the 'order_update' template to +123456789 with the placeholder 'Shipped'. The message ID is 'msg_123'. I'll monitor the delivery status for you.

---

**👤 You:**
> "Check the delivery status for message ID 'msg_123'."

**🤖 AI Agent:**
> Fetching status... Message msg_123 has been successfully 'Delivered' and was 'Read' by the recipient at 2:30 PM today. Would you like to view your full sent history?


## ❓ FAQ

**Q: How do I find my DoubleTick API Key?**
Log in to your DoubleTick account, navigate to **Settings** > **Developer API**, and generate or copy your unique access token.

**Q: Do I need approved templates to send messages?**
Yes, for business-initiated conversations, the WhatsApp Business API requires using templates that have been approved by Meta.

**Q: How do I handle template placeholders?**
The `send_template_message` tool accepts a `placeholders_json` string. Provide a JSON array containing the values for your template variables in order.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/doubletick-alternative](https://vinkius.com/mcp/doubletick-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DoubleTick** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `doubletick-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DoubleTick** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "doubletick-alternative": {
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

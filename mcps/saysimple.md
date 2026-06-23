# Saysimple MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/saysimple)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate omnichannel messaging via Saysimple — manage chats, send WhatsApp/SMS, and use templates with AI.

## Description
Connect your **Saysimple** account to any AI agent and take full control of your omnichannel customer communication through natural conversation. Saysimple provides a centralized platform for managing WhatsApp, SMS, and Social Media interactions via its robust v3 API, and this integration allows you to retrieve chat logs, send template-based notifications, and assign conversations directly from your chat interface.

### What you can do

- **Omnichannel Chat Orchestration** — List all active customer conversations and retrieve detailed metadata, including channel types and participant info programmatically.
- **WhatsApp & SMS Intelligence** — Send direct messages or authorized WhatsApp templates directly from the AI interface to ensure consistent customer engagement.
- **Message Template Control** — Access and monitor your approved communication templates to maintain brand compliance via natural language.
- **Conversation Assignment Management** — Assign chats to specific users or departments to optimize your response velocity and team performance.
- **Operational Monitoring** — Track system activity and monitor webhooks to ensure your messaging flows are always synchronized.

### How it works

1. Subscribe to this server
2. Enter your Saysimple API Key and Auth Token from your developer settings
3. Start managing your omnichannel chats from Claude, Cursor, or any MCP-compatible client

No more manual dashboard refreshing or template searching. Your AI acts as a dedicated customer engagement specialist or support coordinator.

### Who is this for?

- **Support Managers** — quickly retrieve chat histories and monitor agent assignments without switching apps.
- **Marketing Professionals** — automate the delivery of WhatsApp templates and track messaging stats via natural conversation.
- **Customer Success Teams** — streamline the retrieval of contact metadata and coordinate multi-channel responses directly within the chat.


## Available Tools (11)
- **assign_chat**: Assign chat to user
- **create_contact**: Create a new contact
- **get_chat**: Get chat details
- **get_contact**: Get details for a specific contact
- **get_template**: Get details for a message template
- **list_channels**: List all messaging channels
- **list_chats**: List all messaging chats
- **list_contacts**: List all contacts
- **list_templates**: List message templates
- **list_webhooks**: List configured webhooks
- **send_message**: Requires a template for starting new WhatsApp conversations. Pass data as a JSON string.

Send a message


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Saysimple** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active WhatsApp chats in Saysimple."

**🤖 AI Agent:**
> I've retrieved your chats. You have 3 active WhatsApp conversations: 'Alice Miller', 'Support Ticket #55', and 'New Lead Request'. Which one would you like to inspect?

---

**👤 You:**
> "Show me all active customer conversations across WhatsApp and SMS channels with response times."

**🤖 AI Agent:**
> 23 active conversations. WhatsApp (18): 12 awaiting agent reply (avg wait: 4.2 min), 6 in active dialogue. SMS (5): 3 awaiting reply, 2 active. By priority: Urgent (3): billing disputes, avg response time 1.8 min. Normal (15): product inquiries, avg 5.3 min. Low (5): general questions, avg 12 min. SLA compliance: 91% (target 95%). Top agent: Sarah with 8 active chats and 2.1 min avg response. 4 conversations auto-assigned via routing rules.

---

**👤 You:**
> "Send a WhatsApp template message to all contacts who purchased in the last 7 days asking for feedback."

**🤖 AI Agent:**
> WhatsApp template broadcast sent. Template: "Post-Purchase Feedback" (approved by Meta). Recipients: 156 contacts (purchased in last 7 days). Message: "Hi [Name], thank you for your recent purchase! We'd love to hear about your experience. Rate us 1-5 by replying to this message." Delivery: 154 delivered (98.7%). 2 failed (opted out). Read rate after 1 hour: 72% (111 contacts). 34 have already replied with ratings. Average rating so far: 4.3/5.


## ❓ FAQ

**Q: Can my AI automatically find the last 5 customer chats across all channels?**
Yes! Use the `list_chats` tool. Your agent will respond with complete metadata for the most recent conversations, including the channel (WhatsApp/SMS) and participant details in seconds.

**Q: How do I find my Saysimple API Key and Auth Token?**
Log in to your Saysimple dashboard, navigate to **Settings** > **API**, and you will find your unique X-API-Key and generate your Bearer Auth Token there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/saysimple](https://vinkius.com/mcp/saysimple)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Saysimple** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `saysimple` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Saysimple** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "saysimple": {
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

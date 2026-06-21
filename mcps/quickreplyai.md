# QuickReply.ai MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/quickreplyai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Automate WhatsApp marketing and customer engagement via QuickReply.ai — manage contacts, messages, and broadcasts directly from any AI agent.

## Description
Connect your **QuickReply.ai** account to any AI agent and simplify your WhatsApp automation and conversational marketing through natural conversation.

### What you can do

- **Contact Management** — List all WhatsApp subscribers, retrieve detailed profile metadata, and track user segments
- **Messaging & Outreach** — Send text messages or templates to recipients and monitor delivery status through your agent
- **Broadcast Campaigns** — Query past and scheduled broadcast campaigns to monitor your marketing reach
- **Usage Tracking** — Record custom user events and actions programmatically to feed your segmentation
- **Template catalog** — Query available pre-approved WhatsApp message templates for consistent outreach

### How it works

1. Subscribe to this server
2. Enter your QuickReply.ai API Key from your dashboard settings
3. Start managing your WhatsApp automation from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **create_contact**: Create a new contact
- **get_broadcast**: Get details for a specific broadcast
- **get_template**: Get details for a specific message template
- **get_contact_details**: Get details for a specific contact
- **list_broadcast_campaigns**: List broadcast campaigns
- **list_contacts**: List QuickReply.ai contacts
- **list_user_segments**: List contact segments
- **list_message_templates**: List WhatsApp templates
- **send_whatsapp_message**: Send a WhatsApp message
- **track_user_event**: Track a custom engagement event
- **update_contact**: Update an existing contact


## 💬 Prompt Examples

Here are some examples of how you can interact with the **QuickReply.ai** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all contacts in QuickReply.ai."

**🤖 AI Agent:**
> I've retrieved your contacts. You have 200 subscribers, including 'John Doe' (+12345) and 'Alice Smith' (+67890).

---

**👤 You:**
> "Show me all WhatsApp broadcast campaigns from this month with delivery and read rates."

**🤖 AI Agent:**
> 7 WhatsApp broadcasts this month. "Product Launch Announcement" reached 4,567 contacts (98.2% delivered, 84% read, 23% clicked). "Flash Sale Alert" sent to 3,200 (97.8% delivered, 79% read, 31% clicked, highest conversion). "Newsletter May" to 5,100 (98.5% delivered, 72% read). "Feedback Request" to 1,800 (97% delivered, 68% read, 45% responded). Total messages: 18,234. Overall read rate: 76%. Opt-out rate: 0.3%.

---

**👤 You:**
> "Send a personalized WhatsApp template message to all contacts in the VIP Customers segment."

**🤖 AI Agent:**
> Template broadcast sent to VIP Customers segment. Recipients: 234 contacts. Template: "Exclusive VIP Offer" (approved by Meta). Personalization: each message includes the contact's first name and their last purchase category. Delivery: 232 delivered (99.1%), 2 failed (invalid numbers). Read rate after 1 hour: 67% (156 contacts). 12 contacts have already replied. Auto-reply bot activated for incoming responses.


## ❓ FAQ

**Q: Can I send a WhatsApp message using my AI agent?**
Yes! Use the `send_whatsapp_message` action. Provide the recipient's phone number and your message body or template data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/quickreplyai](https://vinkius.com/mcp/quickreplyai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **QuickReply.ai** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `quickreplyai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **QuickReply.ai** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "quickreplyai": {
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

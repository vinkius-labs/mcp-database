# ManyChat MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/manychat-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Engage followers on Instagram, WhatsApp, and Messenger with chatbot flows that qualify leads and drive sales conversations.

## Description
Connect your **ManyChat** account to any AI agent and manage chat marketing through natural conversation.

### What you can do

- **Subscriber Management** — Manage subscribers, tags, and custom fields
- **Broadcasts** — Send and track broadcast messages across channels
- **Flow Tracking** — Monitor flow execution and conversion events
- **Sequences** — Manage automated sequences and drip campaigns
- **Live Chat** — Access live chat conversations and respond to users

### How it works

1. Subscribe to this server
2. Enter your ManyChat API Key
3. Start managing your chatbots from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketers** — manage broadcast campaigns and subscriber segments
- **E-commerce** — track chat conversions and automated flows
- **Support Teams** — monitor live chat and handovers


## Available Tools (12)
- **add_tag**: Add tag to user
- **create_subscriber**: Create new contact
- **find_subscriber_by_email**: Search by email
- **find_subscriber_by_name**: Search by name
- **find_subscriber_by_phone**: Search by phone
- **get_subscriber**: Get subscriber details
- **list_custom_fields**: List bot fields
- **list_flows**: List automation flows
- **list_tags**: List bot tags
- **remove_tag**: Remove tag from user
- **trigger_flow**: Start automation
- **set_custom_field**: Update user field


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ManyChat** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show subscriber growth and broadcast analytics."

**🤖 AI Agent:**
> Subscribers: 14,250 total. Growth (30 days): +1,240 new. Active channels: Instagram (8.2K), Messenger (4.5K), WhatsApp (1.5K). Broadcasts (30 days): 8 sent. Top: 'Weekend Sale' (12K sent, 85% open, 22% CTR ⭐). Worst: 'Blog Update' (4.5K sent, 45% open).

---

**👤 You:**
> "Show active flows and conversion events."

**🤖 AI Agent:**
> Active flows: 12. Top flows: 'Welcome Series' (4.2K triggered, 92% completion). 'Abandoned Cart' (890 triggered, 34% recovered ⭐, $12,400 revenue). 'Lead Gen Quiz' (1.5K started, 45% completion). Conversion events: 3 active. 'Purchase' (145 tracked today).

---

**👤 You:**
> "Find subscriber Sarah Chen and update her tags."

**🤖 AI Agent:**
> Subscriber found: Sarah Chen (ID: 890123). Channel: Instagram. Status: Subscribed. Current tags: 'Lead', 'Webinar_Attendee'. Tag added: 'VIP_Customer'. Custom fields: LTV = $450, Last_Purchase = Apr 15. Flow active: 'Post-Purchase Follow-up'.


## ❓ FAQ

**Q: Can I send broadcasts and track flows?**
Yes. Create broadcasts, manage automation flows, and track engagement metrics like open and click rates.

**Q: How does ManyChat authentication work?**
ManyChat uses Bearer authentication against `api.manychat.com/fb` using your API Key.

**Q: Can I manage tags and custom fields?**
Yes. Create tags, update custom fields per subscriber, and use them for advanced segmentation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/manychat-alternative](https://vinkius.com/mcp/manychat-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ManyChat** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `manychat-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ManyChat** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "manychat-alternative": {
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

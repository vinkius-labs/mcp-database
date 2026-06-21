# Wbiztool MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wbiztool)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [communication-messaging](../categories/communication-messaging.md)

Manage your WhatsApp Business account with bulk messaging, contact management, and campaign analytics for marketing teams.

## Description
Connect your **Wbiztool** account to any AI agent and take full control of your WhatsApp marketing orchestration and automated customer messaging through natural conversation.

### What you can do

- **Messaging Portfolio Orchestration** — List and manage all outgoing WhatsApp messages programmatically, retrieving detailed delivery status and timestamps
- **Contact & Group Intelligence** — Programmatically retrieve directories of WhatsApp contacts and groups to coordinate your organizational outreach strategy
- **Campaign Architecture Monitoring** — Access real-time updates for message delivery (e.g., 'Sent', 'Delivered', 'Read') and track engagement results directly through your agent
- **Metadata Management** — Programmatically retrieve high-fidelity message templates and identifiers to maintain a perfectly coordinated communication record
- **Operational Monitoring** — Verify account-level API connectivity and monitor messaging volume directly through your agent for perfectly coordinated service scaling

### How it works

1. Subscribe to this server
2. Retrieve your **API Key** from your Wbiztool dashboard (Settings > API)
3. Start orchestrating your WhatsApp growth from Claude, Cursor, or any MCP client

No more manual typing of customer messages or missing critical read receipts. Your AI acts as your dedicated communications coordinator and WhatsApp architect.

### Who is this for?

- **Marketing Managers** — instantly trigger message broadcasts and monitor delivery results using natural language commands
- **Sales & Support Leads** — verify individual contact interaction and track message status without leaving your creative workspace
- **Developers** — integrate high-speed Wbiztool messaging data into custom CRM and alert systems through simple AI queries


## Available Tools
- **check_wbiztool_status**: Verify connectivity
- **create_contact**: Create a contact
- **get_contact**: Get contact details
- **get_message_history**: Get message history
- **list_contacts**: List contacts
- **list_groups**: List groups
- **list_messages**: List messages
- **list_templates**: List templates
- **search_contacts**: Search contacts
- **send_bulk_message**: Send bulk messages
- **send_message**: Send a message
- **send_template**: Send a template


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wbiztool** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all WhatsApp messages sent today in my Wbiztool account."

**🤖 AI Agent:**
> I've retrieved your messages. You currently have 50 high-fidelity transmissions today, including 'Order Confirmation' to +15550123. Would you like the detailed delivery status for any of them?

---

**👤 You:**
> "Check if 'John Client' (+15550456) has read my last message."

**🤖 AI Agent:**
> Messaging intelligence orchestrated! For +15550456, I've verified that the high-fidelity status is 'READ'. The message was opened at 2:00 PM today. I've retrieved the technical receipt metadata for your records. Need help drafting a follow-up?

---

**👤 You:**
> "Show my Wbiztool orchestration metrics for this month."

**🤖 AI Agent:**
> Operational monitoring orchestrated! This month, your account has processed 10,000 high-fidelity WhatsApp signals, with a 95% delivery rate and 60% read rate. Your API connection is healthy. Shall I retrieve the detailed engagement breakdown by group?


## ❓ FAQ

**Q: How do I find my Wbiztool API Key?**
Log in to your account, navigate to **Settings** > **API**, and copy your unique API Key from the credentials section.

**Q: Can I check read receipts via AI?**
Yes! The `list_wbiz_messages` tool allows your agent to retrieve high-fidelity real-time status metadata for all your WhatsApp communications.

**Q: How do I list my WhatsApp contacts?**
Use the `list_wbiz_contacts` tool to retrieve your complete high-fidelity directory along with the unique phone identifiers for all managed leads.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wbiztool](https://vinkius.com/mcp/wbiztool)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wbiztool** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `wbiztool` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wbiztool** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wbiztool": {
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

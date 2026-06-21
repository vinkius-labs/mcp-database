# JustCall MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/justcall-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-support](../categories/customer-support.md)

Make and receive business calls from any device with a cloud phone system that logs every interaction in your CRM automatically.

## Description
Connect your **JustCall** account to any AI agent and manage phone communications through natural conversation.

### What you can do

- **Call Management** — Make outbound calls, track call logs with duration and status
- **SMS Messaging** — Send text messages to contacts and track delivery
- **Contact Database** — List contacts, create new entries, and inspect profiles
- **Call Recordings** — Access call recordings with metadata
- **Phone Numbers** — List available and assigned phone numbers
- **Agent Monitoring** — Track agent performance, call volumes, and availability

### How it works

1. Subscribe to this server
2. Enter your JustCall API Key and API Secret
3. Start managing calls from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Teams** — make calls, send follow-up SMS, and track communication history
- **Support Teams** — manage call queues and monitor agent performance
- **Operations** — automate phone outreach and SMS campaigns


## Available Tools (12)
- **create_contact**: Create a new contact
- **get_account_profile**: Get my profile
- **get_call_details**: Get call details
- **get_contact**: Get contact details
- **get_message_details**: Get message details
- **list_calls**: List phone calls
- **list_contacts**: List phone contacts
- **list_messages**: List SMS/MMS messages
- **list_account_numbers**: List JustCall numbers
- **list_team_users**: List team members
- **list_webhooks**: List active webhooks
- **send_message**: Send SMS/MMS


## 💬 Prompt Examples

Here are some examples of how you can interact with the **JustCall** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show today's call log and send a follow-up SMS to the last caller."

**🤖 AI Agent:**
> Today's calls: 34 total. Inbound: 22 (avg 4.2 min). Outbound: 12 (avg 6.1 min). Missed: 3. Last caller: Ana Costa (+1-555-0123, 5 min call, 10:15 AM). SMS sent! ✅ To: +1-555-0123. Content: 'Hi Ana, thanks for calling! I wanted to follow up on our conversation about the Pro plan. Happy to schedule a demo at your convenience.' Delivery: confirmed.

---

**👤 You:**
> "List all agents, their call volumes, and available phone numbers."

**🤖 AI Agent:**
> Agents: 6. Sarah Chen — 145 calls this week (avg 5.2 min, available). Mike Torres — 128 calls (avg 4.8 min, on call). Lisa Park — 112 calls (avg 6.1 min, available). 3 others. Phone numbers: 8 assigned, 3 available. US: +1-555-0100 to 0107. UK: +44-20-7123-4567. Available: +1-555-0108, 0109, 0110.

---

**👤 You:**
> "Show call recordings from this week and the contact database."

**🤖 AI Agent:**
> Recordings: 28 this week. Longest: 'Enterprise Deal — Acme Corp' (22 min, Sarah Chen). Shortest: 'Quick Follow-up' (1 min). Total recording time: 4h 15m. Contacts: 456 total. New this week: 12. By tag: Leads (89), Customers (234), Partners (45), Prospects (88). Would you like to play a recording or create a contact?


## ❓ FAQ

**Q: Can I make calls and send SMS through the AI agent?**
Yes. Make outbound calls with destination number and track status. Send SMS messages to any contact with delivery tracking. Use contact management tools to find recipient numbers.

**Q: Does JustCall require two credentials?**
Yes. JustCall uses an **API Key** and **API Secret** pair for authentication. Both are sent as Bearer credentials against `api.justcall.io/v1`.

**Q: Can I listen to call recordings and track agent performance?**
Yes. Access call recordings with duration and metadata. Monitor agent call volumes, average handle time, and availability status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/justcall-alternative](https://vinkius.com/mcp/justcall-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **JustCall** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `justcall-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **JustCall** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "justcall-alternative": {
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

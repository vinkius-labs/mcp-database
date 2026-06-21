# BatchDialer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/batchdialer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sales-automation](../categories/sales-automation.md)

Automate your outbound dialing workflows via BatchDialer — manage campaigns, leads, and call logs directly from any AI agent.

## Description
Connect your **BatchDialer** account to any AI agent and take full control of your sales and outbound calling operations through natural conversation.

### What you can do

- **Campaign Management** — List and inspect all dialing campaigns to monitor active sales operations.
- **Lead & Contact Control** — Add, query, and manage your contacts (leads) to ensure your dialing lists are always up to date.
- **Call Log Analysis** — Retrieve complete call histories, including durations and outcomes (dispositions).
- **Phone Number Management** — Monitor your caller IDs and managed phone numbers directly from the agent.
- **Outcome Tracking** — List and understand call dispositions to categorize lead interactions accurately.

### How it works

1. Subscribe to this server
2. Enter your BatchDialer API Key
3. Start managing your dialing operations from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Sales Managers** — instantly retrieve campaign statuses and lead metrics without opening the BatchDialer app.
- **SDRs & BDRs** — add leads and check call history straight from your workflow tools.
- **Ops Teams** — monitor phone number health and call logs to optimize outbound strategy.


## Available Tools
- **add_lead**: Add a new lead/contact
- **get_call_details**: Get details of a specific call
- **get_campaign**: Get specific campaign details
- **get_lead**: Get specific lead details
- **get_user_profile**: Get authenticated user profile
- **list_call_logs**: List call logs/history
- **list_campaigns**: List all BatchDialer campaigns
- **list_dispositions**: List call outcomes/dispositions
- **list_leads**: List contacts/leads
- **list_phone_numbers**: List managed phone numbers


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BatchDialer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all our active dialing campaigns on BatchDialer."

**🤖 AI Agent:**
> I've fetched your campaigns. You currently have 2 active campaigns: 'Real Estate West' (ID: 5542) and 'Mortgage Leads Q1' (ID: 5560). Which one would you like to drill into?

---

**👤 You:**
> "Add a new lead: John Doe, phone 555-0199, email john@example.com."

**🤖 AI Agent:**
> I've successfully added 'John Doe' as a new lead in your BatchDialer system. They have been assigned ID 992834 and are ready for the next campaign sync.

---

**👤 You:**
> "Show the recent call logs from today."

**🤖 AI Agent:**
> Today's logs show 15 completed calls. Most interactions resulted in 'Voicemail' (8) or 'Follow-up Needed' (4). Would you like to see the details for the follow-up calls?


## ❓ FAQ

**Q: Can my AI automatically add a new lead to BatchDialer?**
Yes! Use the `add_lead` action with the contact's name and phone number. Your agent will register the lead in your BatchDialer system instantly.

**Q: How do I easily list all recent call logs?**
Simply ask the agent to `list_call_logs`. It will compile the history of recent outbound activities, including status and duration.

**Q: Does the integration allow starting an active call from the agent?**
No. For security and operational safety, the current toolset focuses on management and auditing (listing campaigns, managing leads, checking logs). Initiating live calls must be done through the BatchDialer interface.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/batchdialer](https://vinkius.com/mcp/batchdialer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BatchDialer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `batchdialer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BatchDialer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "batchdialer": {
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

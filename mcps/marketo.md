# Marketo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/marketo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Automate marketing workflows via Marketo — manage leads, lists, campaigns, and programs.

## Description
Connect your **Marketo** account to any AI agent and take full control of your marketing automation through natural conversation.

### What you can do

- **Lead Management** — Fetch lead details by ID or email and list leads from static lists
- **Campaigns** — List and inspect marketing campaigns and smart campaigns
- **Asset Management** — Query programs and other marketing assets
- **Activity Tracking** — List recent activities for specific leads

### How it works

1. Subscribe to this server
2. Enter your Marketo Client ID, Client Secret, and Munchkin ID
3. Start managing your marketing automation from Claude, Cursor, or any MCP-compatible client


## Available Tools (11)
- **list_leads_by_list**: List leads in a static list
- **list_programs**: List all programs
- **list_smart_campaigns**: List all smart campaigns
- **list_static_lists**: List static lists
- **get_campaign_by_id**: Get campaign details by ID
- **get_lead_by_email**: Get lead details by email
- **get_lead_by_id**: Get lead details by ID
- **get_program_by_id**: Get program details by ID
- **get_smart_campaign_by_id**: Get smart campaign details by ID
- **list_activities**: List lead activities
- **list_campaigns**: List all campaigns


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Marketo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get lead details for test@example.com."

**🤖 AI Agent:**
> Fetching lead info... I found a lead with ID 12345. Name: John Doe, Status: active.

---

**👤 You:**
> "List all active campaigns."

**🤖 AI Agent:**
> Querying campaigns... You have several campaigns running, including 'Summer Sale' and 'New Lead Nurture'.

---

**👤 You:**
> "Show recent activities for lead ID 12345."

**🤖 AI Agent:**
> Retrieving activities... Lead 12345 recently opened an email and visited the pricing page.


## ❓ FAQ

**Q: How do I find my Marketo credentials?**
Go to Marketo Admin > LaunchPoint to find your Client ID and Secret. Your Munchkin ID is under Admin > Munchkin.

**Q: Can I search for leads by email?**
Yes! Use the `get_lead_by_email` tool to find specific leads using their email address.

**Q: Is the integration secure?**
Your credentials are encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/marketo](https://vinkius.com/mcp/marketo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Marketo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `marketo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Marketo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "marketo": {
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

# Inbox (useinbox.com) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/inbox-useinboxcom)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage email campaigns, contact lists, and newsletters via UseINBOX API.

## Description
Empower your AI agents to manage your email marketing with UseINBOX. This MCP server allows you to list and retrieve campaigns, manage contact lists and subscribers, view newsletters, and track campaign reports directly through the UseINBOX API. Ideal for automating marketing operations and audience engagement.


## Available Tools
- **get_account**: Gets your UseINBOX account details
- **get_campaign_report**: Retrieves the performance report for a specific campaign
- **list_automations**: Lists all marketing automations
- **list_campaigns**: Lists all email campaigns
- **list_contact_lists**: Lists all contact lists
- **list_contacts**: Lists contacts within a specific list
- **list_newsletters**: Lists all newsletters
- **list_senders**: Lists all authorized email senders
- **list_templates**: Lists all email templates
- **list_webhooks**: Lists all configured webhooks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Inbox (useinbox.com)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my email campaigns in UseINBOX."

**🤖 AI Agent:**
> I'll fetch the list of your active and past email campaigns.

---

**👤 You:**
> "Show me the contacts in my 'VIP Customers' list."

**🤖 AI Agent:**
> I'll retrieve the subscribers for that specific contact list.

---

**👤 You:**
> "Get the latest report for campaign ID '456'."

**🤖 AI Agent:**
> I'll look up the performance metrics and results for that campaign.


## ❓ FAQ

**Q: How do I get UseINBOX API credentials?**
Log in to your UseINBOX dashboard, navigate to Settings > Account Settings > API Keys, and generate a new API key.

**Q: Which API base URL is used?**
This MCP uses the INBOX (Email Marketing) API base: https://useapi.useinbox.com/inbox/v1.

**Q: Can I see campaign reports?**
Yes, the get_campaign_report tool provides access to performance data for your specific email campaigns.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/inbox-useinboxcom](https://vinkius.com/mcp/inbox-useinboxcom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Inbox (useinbox.com)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `inbox-useinboxcom` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Inbox (useinbox.com)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "inbox-useinboxcom": {
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

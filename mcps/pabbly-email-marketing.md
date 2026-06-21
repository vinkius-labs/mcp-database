# Pabbly Email Marketing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pabbly-email-marketing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [customer-relationship-management](../categories/customer-relationship-management.md)

Manage email campaigns and subscribers via Pabbly — list campaigns, track subscribers, and monitor automations directly from any AI agent.

## Description
Connect your **Pabbly Email Marketing** account to any AI agent and take full control of your email outreach and automation workflows through natural conversation.

### What you can do

- **Campaign Oversight** — List all email campaigns and retrieve detailed metadata and performance metrics.
- **Subscriber Management** — List, retrieve, and create subscribers across your various mailing lists.
- **List Discovery** — List all subscriber lists and create new ones to organize your audience.
- **Automation Monitoring** — List active automations to stay on top of your automated user journeys.
- **Form & Content Auditing** — List subscription forms and custom fields to verify your lead capture setup.

### How it works

1. Subscribe to this server
2. Enter your Pabbly API Key (from Settings > API)
3. Start managing your email marketing directly from Claude, Cursor, or any MCP client

### Who is this for?

- **Email Marketers** — quickly check campaign status or subscriber counts while reviewing marketing plans.
- **Marketing Operations** — monitor active automations and form metadata directly from your chat interface.
- **Growth Teams** — add new subscribers to specific lists or verify custom field mappings during lead generation.


## Available Tools
- **create_pabbly_list**: Create a new subscriber list
- **create_pabbly_subscriber**: Add a new subscriber to a list
- **get_pabbly_account**: Get account information
- **get_pabbly_campaign**: Get details for a specific campaign
- **list_pabbly_automations**: List all active automations
- **list_pabbly_campaigns**: List all email campaigns
- **list_pabbly_custom_fields**: List all custom fields defined
- **list_pabbly_forms**: List all subscription forms
- **list_pabbly_lists**: List all subscriber lists
- **list_pabbly_subscribers**: List subscribers in a specific list


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pabbly Email Marketing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my email subscriber lists in Pabbly."

**🤖 AI Agent:**
> I've retrieved your lists. You have 4 subscriber lists: 'Weekly Newsletter', 'Customer Onboarding', 'Product Updates', and 'E-book Leads'. Which one would you like to manage?

---

**👤 You:**
> "Add 'user@example.com' to the 'Weekly Newsletter' list (ID: 12345)."

**🤖 AI Agent:**
> The subscriber 'user@example.com' has been successfully added to the 'Weekly Newsletter' list.

---

**👤 You:**
> "Show me the details for my last email campaign."

**🤖 AI Agent:**
> I've fetched the latest campaign details. Your 'October Flash Sale' campaign has been sent to 5,000 recipients with a 22% open rate and a 4% click rate.


## ❓ FAQ

**Q: How do I find my Pabbly API Key?**
Log in to your Pabbly account, go to **Settings** > **API**. There you can find and copy your unique security token.

**Q: Can I add new subscribers to a specific list?**
Yes! Use the `create_pabbly_subscriber` tool. You will need the `list_id` which you can find using the `list_pabbly_lists` tool.

**Q: Does this support checking automated workflows?**
Absolutely. Use the `list_pabbly_automations` tool to retrieve a list of all active and inactive automated email journeys in your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pabbly-email-marketing](https://vinkius.com/mcp/pabbly-email-marketing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pabbly Email Marketing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `pabbly-email-marketing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pabbly Email Marketing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pabbly-email-marketing": {
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

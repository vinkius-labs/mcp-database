# Cakemail MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cakemail)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage email marketing via Cakemail — track campaigns, manage contact lists, and monitor analytics directly from any AI agent.

## Description
Connect your **Cakemail** account to any AI agent and orchestrate your email marketing, subscriber management, and campaign tracking through natural conversation.

### What you can do

- **List Oversight** — List all your contact lists and retrieve detailed metadata, including total contact counts.
- **Campaign Management** — List all email campaigns and retrieve detailed metadata, including subjects and statuses.
- **Subscriber Coordination** — List contacts within specific lists and add new subscribers directly from your workspace.
- **Analytics Tracking** — Retrieve recent analytics logs to monitor your email performance.
- **Account Insights** — Access your core profile information and account settings straight from your workspace.
- **Deep Dives** — Get detailed data for specific list or campaign IDs using natural language.

### How it works

1. Subscribe to this server
2. Enter your Cakemail API Token (Bearer)
3. Start managing your email marketing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — quickly check campaign statuses or subscriber counts without manual dashboard work.
- **Business Owners** — retrieve marketing performance logs and manage contact lists straight from their workflow tools.
- **Developers** — integrate email campaign and list management steps into their environment using natural language.


## Available Tools (10)
- **create_campaign**: Create a new email campaign
- **create_contact**: Add a contact to a list
- **create_contact_list**: Create a new contact list
- **get_account_info**: Retrieve core account information
- **get_analytics**: Retrieve recent analytics logs
- **get_campaign**: Get details of a specific campaign
- **get_contact_list**: Get details of a specific contact list
- **list_campaigns**: List all email campaigns
- **list_contacts**: List contacts in a specific list
- **list_contact_lists**: List all contact lists


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cakemail** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my contact lists in Cakemail."

**🤖 AI Agent:**
> I've retrieved your lists. You have 3 active lists: 'Newsletter' (ID: list_1), 'Customers' (ID: list_2), and 'Leads' (ID: list_3).

---

**👤 You:**
> "Show the last 5 email campaigns."

**🤖 AI Agent:**
> Retrieving campaigns... Your 5 most recent campaigns include 'March Sale' (Sent), 'New Product Launch' (Draft), and 'Weekly Recap' (Scheduled).

---

**👤 You:**
> "Add john.doe@example.com to the 'Newsletter' list."

**🤖 AI Agent:**
> Contact 'john.doe@example.com' has been successfully added to your 'Newsletter' list in Cakemail.


## ❓ FAQ

**Q: Can I check the total number of contacts in a list using the agent?**
Yes! Use the `get_contact_list` tool with the List ID. Your agent will fetch the detailed metadata, which includes the `total_contacts` field for that specific list.

**Q: How do I add a new contact to an existing list?**
Simply ask the agent to `create_contact` and provide the List ID and the email address. The contact will be added to your Cakemail list instantly.

**Q: Does the integration allow creating a new campaign?**
Yes. Use the `create_campaign` action and provide the name and subject. Your agent will create the campaign in your Cakemail account, allowing you to finalize the content later.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cakemail](https://vinkius.com/mcp/cakemail)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cakemail** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cakemail` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cakemail** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cakemail": {
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

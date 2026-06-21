# Mailsoftly MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailsoftly)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [crm-sales](../categories/crm-sales.md)

Manage marketing campaigns and contacts via the Mailsoftly REST API.

## Description
Connect your **Mailsoftly** account to any AI agent to automate your email marketing and audience management. This MCP server enables your agent to manage subscriber lists, create contacts, and trigger campaign sends directly from natural language interfaces.

### What you can do

- **Campaign Management** — List all email campaigns, retrieve detailed metadata, and trigger official dispatches to targeted segments
- **Audience Oversight** — List and manage your subscriber collections (lists) and retrieve their unique identifiers
- **Contact Control** — Create new subscriber records and add contacts to specific lists programmatically
- **Engagement Auditing** — Retrieve a history of sent campaigns and monitor click-through data for performance analysis
- **Database Ingestion** — Sync contact information and manage subscriber data effortlessly via AI commands

### How it works

1. Subscribe to this server
2. Enter your Mailsoftly API Key
3. Start managing your marketing audience from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Email Marketers** — Monitor campaign statuses and manage subscriber lists via simple natural language commands
- **Sales & CRM Teams** — Quickly update contact data and trigger marketing alerts without opening the portal
- **Growth Engineers** — Integrate email automation logic and engagement tracking directly into your development tools


## Available Tools
- **add_contact_to_list**: Requires email and contact_list ID.

Subscribe a contact to a specific list
- **get_campaign_click_data**: Retrieve click engagement for a sent campaign
- **list_marketing_campaigns**: List all marketing campaigns
- **list_subscriber_collections**: List all contact lists
- **create_base_contact**: Requires email.

Add a new contact to the database
- **get_campaign_details**: Get details for a specific campaign
- **send_campaign_to_all**: Trigger the send process for a campaign
- **list_sent_history**: List campaigns that have been sent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mailsoftly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my email campaigns in Mailsoftly."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 5 campaigns, including 'Launch Event 2024 (ID: cp123)', 'Monthly Roundup', and 'Welcome Series'. Would you like to see metadata for any of them?

---

**👤 You:**
> "Add 'user@example.com' to my 'VIP Customers' list (ID: 'list-987')."

**🤖 AI Agent:**
> Successfully added user@example.com to the VIP Customers list. They are now registered and will receive future mailings targeted to this list.

---

**👤 You:**
> "Show click statistics for sent campaign ID 'cp456'."

**🤖 AI Agent:**
> I've retrieved the click data for campaign cp456. It recorded 145 unique clicks from 120 individual subscribers.


## ❓ FAQ

**Q: How do I find my Mailsoftly API Key?**
Log in to your Mailsoftly account and navigate to Account Settings or API to generate and copy your unique authorization token.

**Q: What fields are required to add a contact to a list?**
You must provide the `email` address and the unique `contact_list` ID. Providing a `first_name` is optional but recommended.

**Q: Can I see how many people clicked a link in a sent campaign?**
Yes, use the `get_campaign_click_data` tool with the target campaign ID to retrieve detailed click engagement statistics.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailsoftly](https://vinkius.com/mcp/mailsoftly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mailsoftly** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `mailsoftly` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mailsoftly** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mailsoftly": {
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

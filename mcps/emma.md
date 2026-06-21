# Emma MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/emma)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage email marketing via Emma — track members, groups, and mailings directly from your AI agent.

## Description
Connect your **Emma** (myemma.com) account to your AI agent and take full control of your email marketing audience and campaigns through natural conversation.

### What you can do

- **Member Management** — List all mailing list members and get detailed profiles including custom fields.
- **Group Segments** — Retrieve and create audience groups to organize your subscribers effectively.
- **Mailing History** — Access a complete list of sent and scheduled email campaigns (mailings).
- **Response Analytics** — Fetch summary response metrics (opens, clicks) for specific mailings.
- **Automation & Webhooks** — Monitor your automated workflows and active webhooks.
- **Field Customization** — List all custom and standard member data fields defined in your account.

### How it works

1. Subscribe to this server
2. Enter your Emma Account ID, Public API Key, and Private API Key
3. Start managing your audience from Claude, Cursor, or any MCP client

### Who is this for?

- **Email Marketers** — quickly check group sizes or member details without navigating the Emma UI.
- **Growth Teams** — automate the creation of new segments and monitor subscriber growth.
- **Support Teams** — verify a customer's subscription status and mailing history during assistance.


## Available Tools
- **list_mailings**: List sent and scheduled mailings
- **list_members**: List mailing list members
- **list_webhooks**: List active webhooks
- **create_group**: Create a new member group
- **delete_group**: Members are not deleted.

Delete a member group
- **get_mailing_stats**: ) for a specific mailing ID.

Get response stats for a mailing
- **get_member**: Get specific member details
- **list_automations**: List email automations
- **list_fields**: List custom member fields
- **list_groups**: List Emma member groups


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Emma** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my audience groups in Emma."

**🤖 AI Agent:**
> I've retrieved your audience groups. You have 5 groups: 'Newsletter Subscribers' (Active), 'VIP Clients', 'Product Beta Testers', and 2 others. Shall I list the members for any of these groups?

---

**👤 You:**
> "Get details for member with email test@example.com."

**🤖 AI Agent:**
> I've found the profile for test@example.com. Their status is 'active', they joined on Jan 15th, and they are currently in the 'General' and 'Beta' groups. Would you like to see their custom field values?

---

**👤 You:**
> "What are the response stats for my latest mailing?"

**🤖 AI Agent:**
> Retrieving stats for your latest mailing (ID: 12345)... It had a 25% open rate and 4% click-through rate. 12 members unsubscribed. Shall I provide more detail on the specific link clicks?


## ❓ FAQ

**Q: How do I find my Emma API Keys?**
Log in to your Emma account, click on your name in the top right, go to 'Account Settings', and then select 'API Key'. You will find your Account ID, Public Key, and Private Key there.

**Q: What is the difference between a group and a segment?**
In Emma, a group is a static collection of members you've explicitly added. A segment is a dynamic group based on rules (like 'opened last email'). This server currently focuses on managing static groups.

**Q: Can I see my custom member data fields?**
Yes! Use the `list_fields` tool to retrieve all standard and custom member data fields defined in your account.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/emma](https://vinkius.com/mcp/emma)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Emma** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `emma` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Emma** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "emma": {
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

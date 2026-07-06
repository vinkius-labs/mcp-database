# Patreon (Creator Subscriptions) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/patreon-creator-subscriptions)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your Patreon creator account—list campaigns, track members, and monitor posts directly from your AI agent.

## Description
Connect your **Patreon** creator account to any AI agent to streamline your membership management and content workflow.

### What you can do

- **Campaign Overview** — List and fetch detailed information about your active Patreon campaigns using `list_campaigns` and `get_campaign`.
- **Member Management** — Retrieve lists of members and inspect individual member details with `list_campaign_members` and `get_member` to understand your audience.
- **Content Monitoring** — Access all posts associated with your campaigns via `list_campaign_posts` to stay on top of your content schedule.
- **Webhook Integration** — Create, list, and manage webhooks for real-time notifications on member activity and post updates using `create_webhook`, `list_webhooks`, and `delete_webhook`.
- **Identity Verification** — Quickly check your authenticated profile and associated permissions with `get_identity`.

### How it works

1. Subscribe to this server
2. Enter your Patreon Creator Access Token
3. Start managing your creator ecosystem from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — Get instant summaries of your membership base and post history without leaving your workflow.
- **Community Managers** — Track member growth and engagement metrics through natural language queries.
- **Developers** — Build and test webhook integrations for custom creator tools directly from the IDE.


## Available Tools (10)
- **get_identity**: Can include memberships and campaign data.

Get the authenticated user profile
- **list_campaign_members**: List members for a specific campaign
- **list_campaign_posts**: List all posts for a campaign
- **update_webhook**: Update an existing webhook
- **list_webhooks**: List webhooks created by your client
- **list_campaigns**: List campaigns owned by the user
- **create_webhook**: g., members:create, posts:publish).

Create a new webhook
- **delete_webhook**: Delete a webhook
- **get_campaign**: Get details for a specific campaign
- **get_member**: Get details for a specific member


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Patreon (Creator Subscriptions)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my Patreon campaigns."

**🤖 AI Agent:**
> I've found your campaigns. You have one active campaign: 'Digital Art & Tutorials' (ID: 1234567). Would you like to see the member list or recent posts for this campaign?

---

**👤 You:**
> "Show me the members for campaign ID 1234567."

**🤖 AI Agent:**
> Fetching members for campaign 1234567... I found 150 active members. The most recent joiners include 'Alex Smith' and 'Jordan Doe'. Do you want details on a specific member?

---

**👤 You:**
> "Who am I logged in as on Patreon?"

**🤖 AI Agent:**
> You are currently authenticated as 'CreativeStudio' (email: creator@example.com). Your profile is linked to 1 campaign.


## ❓ FAQ

**Q: Can I list all members of a specific campaign?**
Yes, you can use the `list_campaign_members` tool by providing the specific Campaign ID to retrieve a full list of associated members.

**Q: Is it possible to set up real-time notifications for new members?**
Absolutely. Use the `create_webhook` tool with the `members:create` trigger and your destination URI to start receiving real-time updates.

**Q: Can I see the posts I have published on my campaign?**
Yes, the `list_campaign_posts` tool allows you to fetch all posts associated with a specific campaign ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/patreon-creator-subscriptions](https://vinkius.com/mcp/patreon-creator-subscriptions)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Patreon (Creator Subscriptions)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `patreon-creator-subscriptions` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Patreon (Creator Subscriptions)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "patreon-creator-subscriptions": {
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

# MailerLite MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mailerlite-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Design beautiful emails, grow your subscriber base, and sell digital products with marketing tools that put simplicity first.

## Description
Connect your **MailerLite** account to any AI agent and manage email marketing through natural conversation.

### What you can do

- **Campaign Management** — Create, schedule, and track email campaigns
- **Subscriber Management** — Add, segment, and manage subscriber groups
- **Automation Workflows** — Browse and monitor automated email sequences
- **Analytics** — Track open rates, click rates, and subscriber growth
- **Form & Landing Pages** — Access signup forms and landing page data

### How it works

1. Subscribe to this server
2. Enter your MailerLite API Key and API version
3. Start managing email from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketers** — run email campaigns with advanced analytics
- **Small Businesses** — manage subscriber lists and automations
- **Creators** — grow audiences with landing pages and forms


## Available Tools (10)
- **create_group**: Use this to organize and segment your audience.

Create a new subscriber group
- **get_subscriber**: Get details for a specific subscriber
- **list_campaigns**: Useful for monitoring marketing activity.

List email campaigns
- **list_custom_fields**: Essential for identifying which fields can be mapped during subscriber upserts.

List all custom subscriber fields
- **list_forms**: List all signup forms
- **list_groups**: Groups are used to organize subscribers for targeted mailings.

List all subscriber groups
- **list_segments**: Useful for identifying high-engagement subsets of your audience.

List all subscriber segments
- **list_subscribers**: Includes email addresses, statuses, and basic engagement metadata.

List all email subscribers
- **list_webhooks**: List active account webhooks
- **upsert_subscriber**: Requires the email address and supports optional first/last name fields.

Create or update a subscriber


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MailerLite** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all campaigns and subscriber growth this month."

**🤖 AI Agent:**
> Campaigns: 12 total. Active: 2 ('Weekly Digest', 'Product Update'). Sent this month: 4. Best: 'Feature Announcement' (42% open, 11% click ⭐). Subscribers: 8,450 total. Growth (30 days): +320 new, -45 unsubscribes. Net: +275. Groups: 'Newsletter' (5,200), 'Product Updates' (3,800), 'Beta' (890).

---

**👤 You:**
> "Show automation workflows and their conversion metrics."

**🤖 AI Agent:**
> Automations: 5 active. 'Welcome Series' (7 emails, 48% open, 14% click, 10% conversion ⭐). 'Cart Recovery' (3 emails, 35% open, 18% click). 'Lead Nurture' (5 emails, 32% open, 8% click). 'Re-engagement' (2 emails, 20% open). 'Upgrade Prompt' (1 email, 28% open, 12% conversion). Total triggered (30 days): 1,240.

---

**👤 You:**
> "Create a subscriber segment and show signup form analytics."

**🤖 AI Agent:**
> Segment created! 'Active Buyers' — opened 5+ emails AND clicked 2+ times (30 days): 1,450 subscribers (17% of total). Forms: 4 active. 'Homepage Popup' (340 signups/mo, 4.2% conversion). 'Blog Sidebar' (180, 2.8%). 'Footer' (90, 1.5%). 'Landing Page' (210, 8.5% ⭐).


## ❓ FAQ

**Q: Can I create campaigns and track performance?**
Yes. Create and schedule campaigns, send to groups or segments, and track opens, clicks, bounces, and conversions in real time.

**Q: Does MailerLite require an API version parameter?**
Yes. MailerLite requires an **API Key** and **API Version** (v1 or v2) for configuration. Bearer auth against `api.mailerlite.com/api/v2`.

**Q: Can I manage automation workflows?**
Yes. Browse active automations, monitor trigger rates, and view email sequence performance.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mailerlite-alternative](https://vinkius.com/mcp/mailerlite-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MailerLite** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mailerlite-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MailerLite** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mailerlite-alternative": {
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

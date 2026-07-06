# Maildroppa MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/maildroppa)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Grow your email list and send targeted campaigns with a simple email marketing platform designed for solopreneurs and creators.

## Description
Connect your **Maildroppa** account to any AI agent and manage email marketing through natural conversation.

### What you can do

- **Campaign Management** — Create, send, and track email campaigns
- **Subscriber Lists** — Manage subscriber lists with segmentation
- **Analytics** — Monitor open rates, click rates, and delivery metrics
- **Automation** — Browse automated sequences and drip campaigns
- **Template Management** — Access and manage email templates

### How it works

1. Subscribe to this server
2. Enter your Maildroppa API Key
3. Start managing campaigns from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketers** — run email campaigns with analytics
- **SaaS Teams** — manage subscriber onboarding sequences
- **Creators** — grow and engage mailing lists


## Available Tools (12)
- **create_segment**: Create a new subscriber segment
- **create_subscriber**: Add a new subscriber
- **create_tag**: Create a new tag type
- **get_subscriber_details**: Get details for a specific subscriber
- **list_custom_fields**: List all custom field types
- **list_sign_up_forms**: List sign-up forms
- **list_segments**: List all subscriber segments
- **list_subscribers**: List mailing list subscribers
- **list_tags**: List all available tags
- **update_subscriber_field**: Update a specific field for a subscriber
- **update_subscriber**: Update subscriber information
- **add_tag_to_subscriber**: Apply a tag to a subscriber


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Maildroppa** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all campaigns and performance for the latest one."

**🤖 AI Agent:**
> Campaigns: 8 total. Latest: 'Spring Product Launch' (sent Apr 24). Recipients: 2,400. Opens: 864 (36% ⭐). Clicks: 216 (9%). Bounces: 12 (0.5%). Unsubscribes: 3 (0.1%). Top link: 'Shop Now' (142 clicks). Others: 'Newsletter #12' (32% open), 'Welcome Series' (auto, 45% open).

---

**👤 You:**
> "Show subscriber lists and create a new segment."

**🤖 AI Agent:**
> Lists: 3. 'Main Newsletter' (2,400 subscribers). 'Product Updates' (1,800). 'Beta Testers' (340). Total: 4,540. Growth (30 days): +120. Segment created! 'Engaged Users' — opened 3+ emails in last 30 days: 890 subscribers (37% of Main). Ready for targeting.

---

**👤 You:**
> "Show automation sequences and their conversion rates."

**🤖 AI Agent:**
> Automations: 3 active. 'Welcome Series' (5 emails, 45% open, 12% click, 8% conversion ⭐). 'Abandoned Cart' (3 emails, 38% open, 15% click, 6% conversion). 'Re-engagement' (2 emails, 22% open, 5% click). Total triggered (30 days): 890. Revenue attributed: $4,200.


## ❓ FAQ

**Q: Can I create and track email campaigns?**
Yes. Create campaigns, send to subscriber segments, and track open rates, click rates, bounces, and unsubscribes in real time.

**Q: How does Maildroppa authentication work?**
Maildroppa uses a custom **X-API-Key** header (not Bearer) against `api.maildroppa.com`.

**Q: Can I manage subscriber lists and segments?**
Yes. Create and manage subscriber lists, add/remove subscribers, and build segments with custom conditions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/maildroppa](https://vinkius.com/mcp/maildroppa)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Maildroppa** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `maildroppa` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Maildroppa** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "maildroppa": {
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

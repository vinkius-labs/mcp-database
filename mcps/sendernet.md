# Sender.net MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/sendernet)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Send email and SMS campaigns that convert with an affordable marketing platform built for e-commerce and small businesses.

## Description
Connect your **Sender.net** account to any AI agent and take full control of your email marketing orchestration through natural conversation. Sender.net provides a powerful and affordable platform for managing subscribers, creating automated campaigns, and tracking engagement, and this integration allows you to orchestrate your entire marketing ecosystem without leaving your chat interface.

### What you can do

- **Subscriber & Audience Orchestration** — List all managed subscribers and retrieve detailed profile metadata, including creating and organizing contacts into groups programmatically.
- **Campaign Performance Intelligence** — Retrieve real-time analytics for sent campaigns, including open rates, click-through rates, and subscriber growth via natural language.
- **Group & Segment Control** — Manage your subscriber lists and group associations to ensure your targeted communication is always synchronized directly from the AI interface.
- **Transactional Messaging Management** — Access account profile metadata and monitor campaign delivery statuses using simple AI commands.
- **Operational Monitoring** — Track system activity and monitor audience health to ensure your marketing operations are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Sender.net API access token from your dashboard settings
3. Start managing your email marketing from Claude, Cursor, or any MCP-compatible client

No more manual stat checking or CSV list management. Your AI acts as a dedicated marketing manager or audience coordinator.

### Who is this for?

- **Marketing Managers** — quickly retrieve campaign results and monitor list growth without switching apps.
- **Sales Teams** — automate the ingestion of new leads and organize them into specific groups via natural conversation.
- **E-commerce Owners** — streamline the retrieval of subscriber engagement data and monitor marketing health directly within the chat.


## Available Tools (11)
- **create_campaign**: Create a new email campaign
- **get_group**: Get details for a subscriber group
- **create_subscriber**: Add a new subscriber
- **delete_subscriber**: Remove a subscriber
- **get_user_profile**: Get your Sender.net profile
- **get_campaign_analytics**: Get performance metrics
- **get_subscriber_details**: Get details for a subscriber
- **list_email_campaigns**: List all sent and draft campaigns
- **list_subscriber_groups**: List your contact groups
- **list_subscribers**: Supports filtering by group or status.

List your Sender.net subscribers
- **update_subscriber**: Update subscriber information


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Sender.net** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active campaigns in my Sender.net account."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 5 recent newsletters including 'Monthly Digest' and 'Product Launch'. Which one would you like to see the stats for?

---

**👤 You:**
> "Show me the subscriber analytics with engagement segments and list health metrics."

**🤖 AI Agent:**
> Total subscribers: 12,400. Active (engaged in 30 days): 8,900 (71.8%). Inactive (30-90 days): 2,100 (16.9%). Dormant (90+ days): 1,400 (11.3%). Growth: +345 this month (net, after 89 unsubscribes). By group: "Newsletter" (8,200), "Product Updates" (6,400), "Promotions" (4,800), "Beta Testers" (890). List health score: 78/100. Bounce rate: 1.2% (good). Spam complaint rate: 0.08% (excellent). Recommended: purge 1,400 dormant subscribers to improve deliverability.

---

**👤 You:**
> "Create a new email campaign for the Product Updates group announcing our latest feature release."

**🤖 AI Agent:**
> Campaign created: "New Feature: AI-Powered Analytics Dashboard". Target group: Product Updates (6,400 subscribers). Subject: "Introducing AI Analytics - Your data, intelligently visualized". Preheader: "Discover patterns you never knew existed". Content: hero image, feature highlights (3 key benefits), CTA "Try It Now". A/B test configured: Subject line A vs B (50/50 split, winner after 4 hours). Scheduled: Tomorrow 10:00 AM (optimal send time). Estimated opens: 2,560 (40% based on group history).


## ❓ FAQ

**Q: Can my AI automatically add a new subscriber to a specific group by providing their email?**
Yes! Use the `create_subscriber` tool. Provide the email address and an array of Group IDs, and your agent will create the record and assign them instantly.

**Q: How do I check the performance statistics for a recently sent campaign?**
Simply ask the agent to run the `get_campaign_stats` action with the Campaign ID. It will retrieve the detailed metadata, including opens, clicks, and bounces.

**Q: How do I find my Sender.net API Token?**
Log in to your Sender.net dashboard, navigate to **Settings** > **API access tokens**, and you will find or generate your unique Bearer token there.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/sendernet](https://vinkius.com/mcp/sendernet)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Sender.net** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `sendernet` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Sender.net** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "sendernet": {
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

# Aimtell MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aimtell)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Web push notification orchestration — manage campaigns, segments, and subscribers via AI.

## Description
Connect your **Aimtell** account to your AI agent to unlock professional web push notification management. From sending one-off alerts to specific subscribers to auditing segment criteria and monitoring real-time campaign analytics, your agent handles your re-engagement strategy through natural conversation.

### What you can do

- **Campaign Orchestration** — List and manage push notification campaigns, including one-off, triggered, and API campaigns
- **Subscriber Management** — Retrieve details for specific subscribers and update custom attributes for personalization
- **Segmentation Oversight** — List and audit your subscriber segments to ensure your targeting is always precise
- **Real-time Analytics** — Retrieve granular performance data (clicks, sends, conversions) for any campaign directly from chat
- **Multi-site Support** — List and manage the different websites associated with your Aimtell account

### How it works

1. Subscribe to this server
2. Enter your Aimtell API Key
3. Start managing your push notifications and monitoring performance through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — automate push campaign sends and monitor real-time performance effortlessly
- **Growth Specialists** — audit subscriber segments and manage custom attributes for lifecycle marketing
- **E-commerce Teams** — quickly check triggered campaign statuses (like abandoned cart alerts) via chat
- **Developers** — verify API campaign configurations and inspect subscriber metadata using simple commands


## Available Tools (10)
- **list_sites**: List managed websites
- **list_subscribers**: List site subscribers
- **get_subscriber_details**: Get subscriber metadata
- **list_segments**: List subscriber segments
- **list_campaigns**: List push campaigns
- **send_one_off_notification**: Send an alert
- **list_triggered_campaigns**: List automated campaigns
- **get_campaign_performance**: Get campaign metrics
- **add_subscriber_attribute**: Add custom data to subscriber
- **list_api_campaigns**: List API-triggered campaigns


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aimtell** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active segments in my Aimtell account."

**🤖 AI Agent:**
> I've retrieved your segments. You have 8 active segments, including 'High Intent Buyers', 'Blog Readers', and 'New Signups'. Would you like to see the subscriber count for any of them?

---

**👤 You:**
> "Show me the performance for campaign ID 12345."

**🤖 AI Agent:**
> I've pulled the analytics for campaign 12345. Total sends: 50,000, Total clicks: 1,250 (2.5% CTR), and 15 conversions generated. The performance is currently within your expected range.

---

**👤 You:**
> "Send a one-off push to segment 9876 with title 'Special Offer' and body 'Get 20% off today only!'."

**🤖 AI Agent:**
> I've triggered the one-off notification to segment 9876. The alert is now being delivered to all eligible subscribers. You can check the real-time click statistics in a few minutes.


## ❓ FAQ

**Q: Where do I find my Aimtell API Key?**
Log in to your Aimtell dashboard, navigate to **Settings** > **API Key**. You will find your unique authorization key there. It must be used in the `X-Authorization-Api-Key` header.

**Q: Can I send a notification to a specific segment?**
Yes! Use the `send_one_off_notification` tool and specify the `segmentId`. Your agent will trigger the push alert to all subscribers currently in that segment.

**Q: Does this support tracking custom attributes?**
Yes, you can use the `add_subscriber_attribute` tool to enrich subscriber profiles with custom data (like name or interests), which can then be used for dynamic content in notifications.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aimtell](https://vinkius.com/mcp/aimtell)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aimtell** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aimtell` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aimtell** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aimtell": {
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

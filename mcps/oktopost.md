# Oktopost MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/oktopost)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage B2B social media via Oktopost — track campaigns, posts, and analytics directly from your AI agent.

## Description
Connect your **Oktopost** account to your AI agent and streamline your B2B social media marketing and lead generation through natural conversation.

### What you can do

- **Campaign Management** — List all active and archived social media campaigns and retrieve detailed settings.
- **Profile Oversight** — Access metadata and connection statuses for all your linked social profiles (LinkedIn, Twitter, Facebook, etc.).
- **Post Monitoring** — List scheduled and sent social media messages across all campaigns and check their content.
- **Lead & Contact Tracking** — Retrieve a list of leads and contacts identified through social media engagement.
- **Analytics Reporting** — Fetch aggregated performance reports for specific metrics like clicks and shares.
- **Conversion Tracking** — Monitor successful goal completions and conversions attributed to your social activities.
- **Deep Inspection** — Fetch complete metadata for specific campaigns, messages, or social profiles using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your Oktopost Account ID and API Key
3. Start managing your B2B social strategy from Claude, Cursor, or any MCP client

### Who is this for?

- **Social Media Managers** — quickly check post schedules or campaign statuses without opening the dashboard.
- **Demand Generation Teams** — monitor social-driven leads and conversions in real-time.
- **Marketing Analysts** — automate the retrieval of social analytics reports for performance tracking.


## Available Tools (10)
- **get_analytics_report**: Get social analytics report
- **get_campaign_details**: Get specific campaign info
- **get_message_details**: Get specific message details
- **get_social_profile_details**: Get specific profile info
- **list_campaigns**: List social media campaigns
- **list_social_contacts**: List social leads and contacts
- **list_social_conversions**: List social-driven conversions
- **list_social_messages**: List scheduled and sent messages
- **list_social_profiles**: ) connected to the account.

List connected social profiles
- **list_oktopost_tags**: List organization tags


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Oktopost** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active social media campaigns."

**🤖 AI Agent:**
> Retrieving campaigns... I found 8 active campaigns including 'Q1 Product Launch', 'Webinar Promotion', and 'Customer Success Stories'. Would you like to see the scheduled posts for the Product Launch?

---

**👤 You:**
> "What is the click engagement for the 'Summer Promo' campaign?"

**🤖 AI Agent:**
> Fetching analytics... The 'Summer Promo' campaign has generated 450 clicks and 25 shares so far this week. The engagement rate is 3.2%. Shall I list the specific posts that generated the most traffic?

---

**👤 You:**
> "Show me the latest leads identified from LinkedIn."

**🤖 AI Agent:**
> Retrieving social contacts... I found 5 new leads identified from LinkedIn engagements today. Notable contacts include 'Sarah Miller (Marketing Director)' and 'David Chen (CTO)'. Would you like their profile details and engagement history?


## ❓ FAQ

**Q: How do I find my Oktopost API credentials?**
Log in to your Oktopost account and navigate to App Settings > API to find your Account ID and generate an API Key.

**Q: Can I see leads generated from social media?**
Yes! Use the `list_social_contacts` tool to retrieve a list of individuals who have engaged with your posts and been identified as leads.

**Q: Does this support LinkedIn and Twitter?**
Yes, Oktopost supports major B2B social platforms. Use `list_social_profiles` to see all your connected accounts and their statuses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/oktopost](https://vinkius.com/mcp/oktopost)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Oktopost** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `oktopost` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Oktopost** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "oktopost": {
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

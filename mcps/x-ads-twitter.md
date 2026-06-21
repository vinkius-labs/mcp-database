# X Ads (Twitter) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/x-ads-twitter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Connect your X Ads account to any AI agent — audit campaigns, analyze line item performance, and pull engagement reports through natural conversation.

## Description
Connect your **X Ads** account to any AI agent and manage your entire advertising operation through natural conversation.

### What you can do

#### Campaign Management
- **Ad Accounts** — List every ad account tied to your profile, inspect statuses, and retrieve funding instrument details
- **Campaigns** — Browse active, paused, or draft campaigns and understand their structure at a glance
- **Line Items** — Audit individual line items to review targeting, bidding strategy, and delivery status
- **Ads** — Inspect the ads running under each line item, including creative associations

#### Analytics & Reporting
- **Performance Metrics** — Pull daily engagement, spend, and conversion data for any campaign, line item, or ad
- **Custom Date Ranges** — Specify exact start and end dates to generate reports for any period
- **Metric Groups** — Choose between Engagement, Billing, Web Conversion, Video, and Mobile Conversion metrics

#### Creative Governance
- **Promoted Tweets** — List all promoted tweets tied to an account to verify what content is currently running
- **Funding Instruments** — Review billing methods and payment sources attached to each ad account

### How it works

1. Subscribe to this server
2. Enter your API Key, API Secret, Access Token, and Access Token Secret from the X Developer Portal
3. Start auditing campaigns and pulling reports from Claude, Cursor, or any MCP-compatible client

All requests are signed with OAuth 1.0a at runtime. Your credentials are encrypted at rest and never exposed.

### Who is this for?

- **Performance Marketers** — pull weekly spend and engagement summaries without opening the Ads Manager
- **Ad Operations Teams** — verify campaign configurations and promoted tweet statuses in seconds
- **Growth Leads** — compare line item performance across campaigns to reallocate budget
- **Agencies** — audit multiple client accounts from a single AI interface


## Available Tools (13)
- **get_ad_account**: Use this to verify an account is active before querying campaigns.

Get detailed metadata for a specific X Ads account
- **list_ad_accounts**: Returns account IDs, names, statuses, and approval states. The account ID returned here is required by all other tools.

List all X (Twitter) Ads accounts accessible by the authenticated user
- **list_ads**: Each ad references the line item it belongs to and the creative (tweet) it promotes.

List all individual ads within an X Ads account
- **list_campaigns**: Each campaign includes its name, status, funding instrument, daily budget, and total budget. Use list_ad_accounts first to get the account ID.

List all campaigns within an X Ads account
- **list_funding_instruments**: Useful for verifying billing is set up before launching campaigns.

List payment methods and billing sources attached to an X Ads account
- **list_line_items**: Line items define the targeting and bidding strategy within a campaign.

List all line items across campaigns in an X Ads account
- **get_analytics**: Metric groups: ENGAGEMENT, BILLING, VIDEO, WEB_CONVERSION, MOBILE_CONVERSION. Dates must be ISO 8601 format (e.g., 2026-06-01T00:00:00Z).

Pull performance analytics for campaigns, line items, or ads over a date range
- **get_campaign**: Use list_campaigns first to find the campaign ID.

Get full details for a specific campaign by its ID
- **get_line_item**: Use list_line_items first to find the line item ID.

Get full details for a specific line item by its ID
- **list_media_creatives**: Use this to audit which creative assets are currently active.

List all media creative assets (images and videos) used in an X Ads account
- **list_promoted_tweets**: Use this to verify which tweets are actively being promoted.

List all promoted tweets currently running or paused in an X Ads account
- **list_tailored_audiences**: Useful for understanding retargeting strategy.

List custom audiences (tailored audiences) for retargeting and CRM matching
- **list_targeting_criteria**: Requires both the account ID and line item ID.

List all targeting criteria applied to a specific line item


## 💬 Prompt Examples

Here are some examples of how you can interact with the **X Ads (Twitter)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my X ad accounts and tell me which ones are active."

**🤖 AI Agent:**
> You have 2 ad accounts:

1. **SaaS Growth** (ID: abc123) — Active, funding via credit card ending in 4242
2. **Product Launch Q2** (ID: def456) — Paused since June 3

Would you like me to pull the active campaigns for 'SaaS Growth'?

---

**👤 You:**
> "Show me the engagement metrics for all line items in account abc123, from June 1 to June 14."

**🤖 AI Agent:**
> Here are the engagement metrics for your 3 line items between June 1–14:

| Line Item | Impressions | Clicks | Spend | CTR |
|---|---|---|---|---|
| Retargeting — Webinar | 42,100 | 1,230 | $312 | 2.92% |
| Lookalike — SaaS | 38,500 | 890 | $278 | 2.31% |
| Brand Awareness | 91,200 | 620 | $445 | 0.68% |

The retargeting line item is outperforming by CTR. Would you like a day-by-day breakdown?

---

**👤 You:**
> "Which promoted tweets are running right now on account abc123?"

**🤖 AI Agent:**
> You have 4 promoted tweets active on that account:

1. "Just launched our AI integration..." — Linked to 'SaaS Growth' campaign
2. "Watch the full product demo..." — Linked to 'Video Launch'
3. "Free trial — no credit card..." — Linked to 'Retargeting'
4. "Case study: 3x pipeline in 60 days..." — Linked to 'Lookalike'

Want me to pull engagement stats for any of these?


## ❓ FAQ

**Q: Where do I find the four credentials I need?**
In the [X Developer Portal](https://developer.x.com/), open your App under your Project. Under **Keys and Tokens**, you will find the **API Key** (Consumer Key) and **API Key Secret** (Consumer Secret). Below that, generate your **Access Token** and **Access Token Secret**. All four are required because the X Ads API uses OAuth 1.0a request signing.

**Q: Do I need Ads API approval from X?**
Yes. The X Ads API is access-gated. You need to apply through the [X Developer Portal](https://developer.x.com/) and receive explicit approval before your credentials will work with Ads endpoints. Standard developer accounts only have access to the general X API.

**Q: Can I pull analytics for a specific date range?**
Yes. The analytics tool accepts start and end dates in ISO 8601 format along with metric groups such as Engagement, Billing, or Video. Just ask your agent something like 'show me engagement metrics for campaign X from June 1 to June 15' and it will build the right query.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/x-ads-twitter](https://vinkius.com/mcp/x-ads-twitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **X Ads (Twitter)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `x-ads-twitter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **X Ads (Twitter)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "x-ads-twitter": {
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

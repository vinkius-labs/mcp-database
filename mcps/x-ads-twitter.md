# X Ads (Twitter) MCP Server

Connect your X Ads account to any AI agent — audit campaigns, analyze line item performance, and pull engagement reports through natural conversation.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/x-ads-twitter)

## Overview
**Category:** industry-titans
**Tools Count:** 13

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


## Available Tools
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


## Installation & Usage

To install and use the **X Ads (Twitter)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/x-ads-twitter](https://vinkius.com/mcp/x-ads-twitter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

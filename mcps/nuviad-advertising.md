# Nuviad Advertising MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nuviad-advertising)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nuviad-advertising-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nuviad-advertising-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Manage mobile ad campaigns and RTB via Nuviad — track ads, targeting lists, and performance reports directly from your AI agent.

## Description
Connect your **Nuviad** mobile advertising account to your AI agent and take control of your programmatic campaigns and real-time bidding (RTB) through natural conversation.

### What you can do

- **Campaign Management** — List all active and paused campaigns, and duplicate existing ones for quick scaling.
- **Creative Oversight** — Access your library of ad creatives including banners, videos, and native ad assets.
- **Granular Targeting** — Monitor and manage your targeting lists, including device ID blacklists and whitelists.
- **Performance Reporting** — Request detailed campaign reports, check their generation status, and retrieve the results.
- **Optimization Control** — List and retrieve campaign micro-bids and margin adjustments defined at the exchange or site level.
- **Geographic Intelligence** — Browse available geographic locations for precise global or local targeting.
- **Deep Inspection** — Fetch complete metadata and configuration for specific campaigns or ads using their unique IDs.

### How it works

1. Subscribe to this server
2. Enter your Nuviad API Key (Bearer Token)
3. Start managing your mobile ads from Claude, Cursor, or any MCP client

### Who is this for?

- **Ad Ops Managers** — quickly check campaign statuses or performance summaries without opening the Nuviad portal.
- **Marketing Analysts** — automate the retrieval of campaign reports and micro-bid data for analysis.
- **Growth Teams** — monitor ad distribution and targeting list connectivity in real-time.


## Available Tools
- **get_reports_summary**: Get campaign performance summary
- **list_geo_locations**: List available geographic locations
- **get_report_content**: Retrieve generated report data
- **get_report_status**: Check report request status
- **list_creatives**: List all ad creatives
- **list_campaigns**: List all mobile ad campaigns
- **list_micro_bids**: List campaign micro-bids
- **list_micro_margins**: List campaign micro-margins
- **list_targeting_lists**: List all audience and targeting lists
- **request_campaign_report**: Request a detailed campaign report


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nuviad Advertising** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active mobile ad campaigns."

**🤖 AI Agent:**
> Retrieving campaigns... I found 5 active campaigns including 'Summer Promo 2024', 'Brand Awareness US', and 'App Install Growth'. Would you like the performance summary for the Summer Promo?

---

**👤 You:**
> "Request a performance report for campaign ID 'cmp_98765' for the last 7 days."

**🤖 AI Agent:**
> Report request initiated... The request for campaign cmp_98765 has been submitted (ID: req_12345). I'll check the status for you. It usually takes a few minutes to generate.

---

**👤 You:**
> "Show me the list of ad creatives in my account."

**🤖 AI Agent:**
> Fetching ad creatives... You have 12 assets registered: 8 'Banner' images, 2 'Video' ads, and 2 'Native' components. Shall I list the specific Image Keys for the banners?


## Installation & Usage

To install and use the **Nuviad Advertising** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nuviad-advertising](https://vinkius.com/mcp/nuviad-advertising)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Cometly MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cometly)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cometly-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cometly-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Enable your AI agent to track conversions, retrieve attribution data, and monitor campaigns via the Cometly API.

## Description
Connect your AI to **Cometly**, the ad attribution platform for Meta, Google, TikTok and more.

### What you can do

- **Event Tracking** — Track purchases, leads, and custom events with attribution metadata.
- **Campaign Analytics** — List campaigns and retrieve ROAS, CPA, and conversion stats.
- **Attribution Data** — Query which ads drive your highest-value conversions.

### How it works

1. Add the Cometly integration to your AI toolset.
2. Provide your API Key (Account Settings > API Keys).
3. Track events and query data via natural language.

### Who is this for?

- **Performance Marketers** — Get ROAS breakdowns without logging into dashboards.
- **Growth Teams** — Track conversions and identify top channels from chat.
- **E-commerce Managers** — Monitor purchase attribution across ad platforms.


## Available Tools
- **get_campaign_stats**: Retrieve performance stats for a specific campaign
- **list_ad_accounts**: Retrieve a list of connected ad accounts (Meta, Google, etc.)
- **list_campaigns**: Retrieve a list of all tracked ad campaigns
- **list_contacts**: Retrieve a list of attributed contacts and their customer journey data
- **list_events**: Retrieve a list of tracked events in Cometly
- **track_event**: Send a conversion event (Purchase, Lead, etc.) to Cometly for attribution
- **track_lead**: Quickly track a lead event
- **track_purchase**: Quickly track a purchase event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cometly** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Track a purchase of $99.90 for 'customer@example.com' with order 'ORD-123'."

**🤖 AI Agent:**
> Purchase tracked! Order: ORD-123, $99.90. Attributed to Facebook Ad 'Summer Sale' (camp-4x2k). Syncing to Meta and Google in ~15 min.

---

**👤 You:**
> "Get performance stats for campaign 'camp-xxxx' over the last 30 days."

**🤖 AI Agent:**
> Campaign 'camp-xxxx' (30 days): Spend $4,200 | 186 conversions | Revenue $18,540 | ROAS 4.41x | CPA $22.58. Top ad set: 'Lookalike US' (62%).

---

**👤 You:**
> "List the top 3 best performing active campaigns by ROAS."

**🤖 AI Agent:**
> Top 3 Active Campaigns by ROAS:
1. 'Retargeting Q3' (Google) - ROAS: 6.2x
2. 'Lookalike 1%' (Meta) - ROAS: 4.8x
3. 'Brand Search' (Google) - ROAS: 4.5x


## Installation & Usage

To install and use the **Cometly** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cometly](https://vinkius.com/mcp/cometly)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

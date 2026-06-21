# Everflow Partner Marketing MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/everflow-partner-marketing)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/everflow-partner-marketing-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/everflow-partner-marketing-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to manage marketing offers, track affiliates, and monitor network performance via the Everflow API.

## Description
Integrate **Everflow**, the comprehensive partner marketing platform, directly into your AI workflow. Manage your marketing offers and payouts, track affiliate profiles and performance, monitor advertisers and creative assets, and oversee your entire network performance using natural language.

### What you can do

- **Offer Oversight** — List and retrieve detailed information, payout structures, and targeting rules for all your marketing offers.
- **Affiliate Intelligence** — Monitor affiliate profiles and performance summaries, resolving contact details and organizational tags.
- **Network Performance** — Access real-time network telemetry, resolving total clicks, conversions, and revenue via chat.
- **Network Auditing** — Retrieve high-level summaries of offer volume, affiliate activity, and organizational network health instantly.

### How it works

1. Connect the Everflow integration to your AI assistant.
2. Authorize using your Everflow API Key (found in your account settings).
3. Orchestrate your partner marketing and affiliate management strategy through intuitive conversation.

### Who is this for?

- **Affiliate Managers** — Quickly check offer performance and affiliate payouts on the go.
- **Network Owners** — Research advertiser details and total network revenue via chat.
- **Operations Teams** — Monitor creative usage and organizational network metadata instantly.


## Available Tools
- **get_everflow_network_metadata**: Retrieve metadata and limits for your Everflow network
- **get_affiliate_detailed_profile**: Get detailed profile and performance summary for a specific affiliate
- **get_offer_detailed_data**: Get detailed settings and tracking information for a specific offer
- **get_network_performance_summary**: Get a high-level summary of network performance metrics
- **quick_partner_marketing_audit**: Retrieve a high-level summary of offers, affiliates, and advertisers
- **list_currently_active_offers**: Identify offers that are currently in an "Active" status
- **list_network_advertisers**: List all advertisers configured in your network
- **list_marketing_affiliates**: List all affiliates and partners in your network
- **list_offer_marketing_creatives**: List all creative assets (banners, links) for a specific offer
- **list_marketing_offers**: List all marketing offers in your Everflow account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Everflow Partner Marketing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all active marketing offers."

**🤖 AI Agent:**
> I've found 12 active offers, including 'Summer Sale Promo' and 'VIP Loyalty Reward'. 8 offers are currently generating conversions. Would you like to see the payout details for the Summer Sale?

---

**👤 You:**
> "Show me the performance for affiliate ID 12345."

**🤖 AI Agent:**
> Affiliate ID 12345 ('Top Partner Media') has generated 1,500 clicks and 85 conversions this week, totaling $4,250 in revenue. Their current payout is $850. Should I pull their detailed conversion log?

---

**👤 You:**
> "What is the network performance summary for today?"

**🤖 AI Agent:**
> Today across the network, you have 15,000 total clicks and 450 conversions (3% CR). Gross revenue is $12,500 with a total network payout of $2,500. Performance is up 5% compared to yesterday. Should I check which advertiser is leading?


## Installation & Usage

To install and use the **Everflow Partner Marketing** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/everflow-partner-marketing](https://vinkius.com/mcp/everflow-partner-marketing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

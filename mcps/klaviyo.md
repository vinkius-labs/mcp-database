# Klaviyo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/klaviyo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/klaviyo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/klaviyo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Drive revenue with email and SMS marketing powered by customer data that personalizes every message to increase lifetime value.

## Description
Connect your **Klaviyo** account to any AI agent and manage email marketing through natural conversation.

### What you can do

- **List Management** — Browse, create, and manage subscriber lists and segments
- **Campaign Tracking** — View campaigns with open rates, click rates, and delivery stats
- **Profile Management** — Browse and inspect subscriber profiles with engagement data
- **Flow Monitoring** — Track automated email flows and their performance
- **Metrics & Analytics** — Access performance metrics, revenue attribution, and trends
- **Template Access** — Browse email templates and their configurations

### How it works

1. Subscribe to this server
2. Enter your Klaviyo Private API Key
3. Start managing email marketing from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Teams** — manage campaigns and analyze performance
- **E-commerce** — track revenue attribution and customer engagement
- **Growth Teams** — monitor flows, segments, and subscriber growth


## Available Tools
- **create_profile**: Create a new profile
- **get_profile**: Get profile details
- **list_campaigns**: List sent campaigns
- **list_automated_flows**: List automated flows
- **list_marketing_lists**: List marketing lists
- **list_metrics**: List tracking metrics
- **list_profiles**: List all customer profiles
- **list_segments**: List dynamic segments
- **list_tags**: List account tags
- **list_email_templates**: List email templates
- **list_webhooks**: List active webhooks
- **track_event**: g. "Viewed Product").

Record a customer event


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Klaviyo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show all campaigns from this month with open rates and revenue."

**🤖 AI Agent:**
> This month: 8 campaigns sent. Best performers: 1) 'Flash Sale — 40% Off' — 45K sent, 32% open, 8.2% click, $12.4K revenue. 2) 'New Arrivals' — 38K, 28% open, 5.6% click, $8.1K. 3) 'Loyalty Rewards' — 22K, 35% open, 9.1% click, $6.8K. Total revenue attributed: $42.3K. Average open rate: 29%. Average click rate: 6.4%.

---

**👤 You:**
> "List all subscriber lists and the top-performing automated flows."

**🤖 AI Agent:**
> Lists: 6. Newsletter (45K subscribers), VIP Customers (8.2K), New Signups (12K), Inactive (5.4K), Cart Abandonment (3.1K), Product Interest (15K). Flows: 5 active. 'Welcome Series' (3 emails, 42% open, $2.1K/mo). 'Cart Abandonment' (2 emails, 38% open, $8.4K/mo ⭐). 'Post-Purchase' (4 emails, 35% open, $3.2K/mo). 'Win-Back' (2 emails, 22% open, $1.1K/mo). 'Birthday' (1 email, 48% open).

---

**👤 You:**
> "Show the profile for sarah@company.com and her engagement history."

**🤖 AI Agent:**
> sarah@company.com — Lists: VIP Customers, Newsletter. Joined: Jan 15, 2024. Emails received: 48. Open rate: 42% (above avg). Click rate: 12%. Last opened: yesterday. Revenue attributed: $1,245. Orders: 4. Last purchase: Apr 20 ($189). Segments: High-Value, Active Buyer, Tech Interest. Predicted CLV: $2,100.


## Installation & Usage

To install and use the **Klaviyo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/klaviyo](https://vinkius.com/mcp/klaviyo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

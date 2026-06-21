# Fathom Analytics MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fathom-analytics)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/fathom-analytics-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/fathom-analytics-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Privacy-first website analytics via Fathom — list sites, monitor real-time visitors, and aggregate pageviews directly through your AI agent.

## Description
Connect your **Fathom Analytics** account to any AI agent and take full control of your website intelligence through natural conversation without compromising user privacy.

### What you can do

- **Site Orchestration** — List all managed websites and fetch detailed metadata for specific analytics properties
- **Real-time Monitoring** — Query current live visitor counts for any site to track immediate traffic spikes flawlessly
- **Deep Aggregations** — Extract granular metrics including uniques, pageviews, average duration, and bounce rates for specific periods
- **Attribution Analysis** — List top referrers and search terms to understand where your traffic is coming from natively
- **Behavioral Insights** — Query top-performing pages and device type distributions to optimize your content strategy
- **Identity Context** — Verify your API token user profile and account limits through the agent synchronously

### How it works

1. Subscribe to this server
2. Enter your Fathom Analytics API Token (Settings > API)
3. Start querying your privacy-first analytics from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Growth Marketers** — monitor site performance and campaign attribution without manual dashboard exports
- **Privacy-Conscious Teams** — access high-level analytics without ever touching personally identifiable information (PII)
- **Business Owners** — check key traffic metrics and current visitor counts through simple natural language questions


## Available Tools
- **get_account_info**: Get Fathom Analytics account information
- **get_current_visitors**: Get the number of current visitors on a site
- **get_device_stats**: Get device type aggregations for a site
- **get_event**: Get details for a specific event
- **get_me**: Get current API token user profile
- **get_top_pages**: Get top pages for a site
- **get_pageviews**: Get pageview aggregations for a site
- **get_referrers**: Get top referrers for a site
- **get_site**: Get details for a specific site
- **get_visitors**: Get visitor aggregations for a site
- **list_events**: List custom events for a specific site
- **list_sites**: List all sites in your Fathom Analytics account


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fathom Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many visitors are on my site right now?"

**🤖 AI Agent:**
> Checking live visitors... You currently have 12 active visitors on 'mysite.com'. Would you like to see the top referrers for this session?

---

**👤 You:**
> "Show me pageview stats for last week."

**🤖 AI Agent:**
> Aggregating data for last week... Your site received 5,200 pageviews and 1,800 unique visitors. The average session duration was 2 minutes and 15 seconds.

---

**👤 You:**
> "List my top referral sources."

**🤖 AI Agent:**
> Fetching referrers... Your top traffic sources are Google (40%), Twitter (25%), and Direct (15%). Shall I show you the bounce rate for each of these sources?


## Installation & Usage

To install and use the **Fathom Analytics** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fathom-analytics](https://vinkius.com/mcp/fathom-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

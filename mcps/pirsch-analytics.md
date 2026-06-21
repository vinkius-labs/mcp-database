# Pirsch Analytics MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pirsch-analytics)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pirsch-analytics-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pirsch-analytics-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Privacy-friendly web analytics — track hits, events, and retrieve detailed statistics for your domains directly from your AI agent.

## Description
Connect **Pirsch Analytics** to your AI agent to monitor your website traffic and user behavior without compromising privacy. This MCP server allows you to collect data and query complex statistics through natural language.

### What you can do

- **Traffic Monitoring** — Retrieve overview, visitor, and page statistics for any of your domains using specific date ranges.
- **Event Tracking** — Send individual or batch hits and events to track user conversions and interactions in real-time.
- **Domain Management** — List all configured domains and create new ones directly through the API.
- **Referrer & Source Analysis** — Analyze where your traffic is coming from with detailed referrer and UTM source statistics.
- **Real-time Insights** — Access active visitor counts and goal completion metrics to stay on top of your site's performance.

### How it works

1. Subscribe to this server
2. Enter your Pirsch Access Token (Client Secret)
3. Start querying your analytics from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Marketing Managers** — get instant reports on campaign performance and visitor trends without opening a dashboard.
- **Developers** — integrate tracking hits and events into automated workflows or check site health from the CLI/IDE.
- **Data Analysts** — extract raw statistics and overview metrics for custom reporting and performance audits.


## Available Tools
- **create_domain**: Create a new domain
- **list_domains**: List all domains
- **send_event_batch**: Send a batch of events
- **send_event**: Send an event to Pirsch
- **send_hit_batch**: Send a batch of page views (hits)
- **send_hit**: Send as much information as possible for accurate analytics.

Send a page view (hit) to Pirsch
- **get_statistics_active**: Get active visitors statistics
- **get_statistics_events**: Get events list statistics
- **get_statistics_goals**: Get conversion goals statistics
- **get_statistics_overview**: Get overview statistics for a domain
- **get_statistics_page**: Get page statistics
- **get_statistics_referrer**: Get referrer statistics
- **get_statistics_utm_source**: Get UTM source statistics
- **get_statistics_visitor**: Get visitor statistics


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pirsch Analytics** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get visitor statistics for domain ID 'abc-123' from 2023-10-01 to 2023-10-31."

**🤖 AI Agent:**
> I've retrieved the visitor data for domain 'abc-123'. During October, you had 1,250 unique visitors with an average session duration of 2 minutes and 15 seconds.

---

**👤 You:**
> "Track a page view for 'https://example.com/pricing' from IP 1.2.3.4."

**🤖 AI Agent:**
> The hit for the pricing page has been successfully sent to Pirsch using the `send_hit` action. It is now being processed in your analytics dashboard.

---

**👤 You:**
> "List all my domains configured in Pirsch."

**🤖 AI Agent:**
> Fetching your domains... I found 3 domains: 'example.com' (ID: abc-123), 'blog.example.com' (ID: def-456), and 'shop.example.com' (ID: ghi-789).


## Installation & Usage

To install and use the **Pirsch Analytics** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pirsch-analytics](https://vinkius.com/mcp/pirsch-analytics)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

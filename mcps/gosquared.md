# GoSquared MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gosquared)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/gosquared-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/gosquared-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Monitor real-time web traffic and analyze historical trends via AI.

## Description
Connect your **GoSquared** account to your AI agent and get instant, conversational access to your web analytics. Query real-time active visitors, track marketing campaign performance, and analyze historical traffic trends directly from your workflow.

### What you can do

- **Real-Time Analytics (Now API)** — Check exactly how many visitors are on your site right now, what pages they are viewing, and where they came from
- **Historical Trends (Trends API)** — Analyze past traffic data, including page views, traffic sources, and campaign effectiveness over specific date ranges
- **Audience Insights** — Understand your visitors' technology preferences with detailed breakdowns of browsers and devices

### How it works

1. Subscribe to this server
2. Enter your GoSquared Site Token and API Key (found in your account settings)
3. Start querying your web analytics from Claude, Cursor, or any MCP-compatible client

Your AI agent acts as a dedicated web analyst, transforming complex dashboards into simple, actionable answers.

### Who is this for?

- **Marketing Teams** — instantly check how much live traffic a new campaign or newsletter is generating
- **Product Managers** — analyze historical page view trends to understand feature adoption and user behavior
- **Website Owners** — keep a pulse on your site's performance without constantly logging into an analytics dashboard


## Available Tools
- **get_now_campaigns**: Get active campaigns currently driving traffic
- **get_now_overview**: Get a top-level overview of concurrent active visitors
- **get_now_pages**: Get a list of pages currently being viewed
- **get_now_sources**: Get active traffic sources (referrers)
- **get_now_visitors**: Get a list of individual visitors currently online
- **get_trends_browsers**: Get historical browser breakdown data
- **get_trends_campaigns**: Get historical campaign performance data
- **get_trends_devices**: Get historical device breakdown data
- **get_trends_overview**: Get historical aggregate data overview
- **get_trends_pages**: Get historical aggregate data for pages
- **get_trends_sources**: Get historical traffic sources data


## 💬 Prompt Examples

Here are some examples of how you can interact with the **GoSquared** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many visitors are on the site right now?"

**🤖 AI Agent:**
> Checking real-time analytics... You currently have 142 active visitors on your site. 85 of them are actively engaging with the content.

---

**👤 You:**
> "What were our top traffic sources yesterday?"

**🤖 AI Agent:**
> Retrieving trends... Yesterday, your top traffic sources were:
1. Google (Organic): 1,200 visits
2. Direct: 850 visits
3. Twitter / X: 420 visits
4. LinkedIn: 150 visits

---

**👤 You:**
> "Tell me what percentage of visitors today are using mobile phones."

**🤖 AI Agent:**
> Checking technology insights... So far today, 62% of your site traffic is originating from mobile devices, predominantly iOS.


## Installation & Usage

To install and use the **GoSquared** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gosquared](https://vinkius.com/mcp/gosquared)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

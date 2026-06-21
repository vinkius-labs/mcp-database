# Umami Cloud MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/umami-cloud)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/umami-cloud-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/umami-cloud-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Privacy-focused web analytics alternative to Google Analytics.

## Description
The Umami Cloud MCP Server connects AI agents to the Umami Analytics API. It allows agents to retrieve real-time and historical website statistics, fetch pageviews, analyze active users, and export events dynamically while preserving end-user privacy.


## Available Tools
- **users**: Get the number of active users on a website
- **websites**: Get specific metrics (urls, browsers, os, devices) for a website


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Umami Cloud** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the top 5 pages by pageviews on my main website for the last 7 days."

**🤖 AI Agent:**
> Here are the top pages: 1. /home (5,000 views), 2. /pricing (1,200 views)...

---

**👤 You:**
> "Analyze the bounce rate and absolute session duration from mobile users on the pricing page today."

**🤖 AI Agent:**
> Fetching Umami metrics ('get_page_metrics')...
Mobile Traffic (URL: `/pricing` - Today):
- Unique Visitors: 1,840 
- Bounce Rate: 54.2%
- Average Session Duration: 1m 42s

---

**👤 You:**
> "List the top 4 referral traffic sources matching 'social' for this month."

**🤖 AI Agent:**
> Querying referral patterns on Umami Cloud ('get_referrers')...
Top 'Social' Referrers:
1. Twitter/X: 4,112 visits
2. LinkedIn: 2,890 visits
3. HackerNews: 1,140 visits
4. Reddit: 885 visits


## Installation & Usage

To install and use the **Umami Cloud** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/umami-cloud](https://vinkius.com/mcp/umami-cloud)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

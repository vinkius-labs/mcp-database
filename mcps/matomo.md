# Matomo MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/matomo)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/matomo-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/matomo-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Open-source web analytics via Matomo — track visits, goals, and user behavior directly from any AI agent.

## Description
Connect your **Matomo** analytics instance to any AI agent and gain deep insights into your website traffic through natural conversation.

### What you can do

- **Visits Summary** — Get aggregated metrics on visits, actions, and bounce rates
- **Real-time Monitoring** — See the latest visitor details and actions as they happen
- **Top Content** — Identify your most visited pages, referring websites, and social networks
- **Visitor Profiles** — Inspect complete history and behavior for specific visitor IDs
- **Goal Tracking** — List and monitor conversion goals configured in your instance

### How it works

1. Subscribe to this server
2. Enter your Matomo URL, Token Auth, and Site ID
3. Start querying your web analytics from Claude, Cursor, or any MCP-compatible client


## Available Tools
- **get_goals**: Get the list of goals
- **get_live_last_visits**: Get last visits in real-time
- **get_site_details**: Get details for a specific website
- **get_top_pages**: Get the most visited pages
- **get_top_referrers**: Get the top referrer types
- **get_top_socials**: Get the top referring social networks
- **get_top_websites**: Get the top referring websites
- **get_visitor_profile**: Get a detailed profile for a visitor
- **get_visits_summary**: Get a summary of visits
- **list_sites**: List all websites in Matomo


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Matomo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me a summary of visits for today."

**🤖 AI Agent:**
> Retrieving summary... Today you had 1,250 visits with an average of 3 actions per visit.

---

**👤 You:**
> "What are the top pages on my site this week?"

**🤖 AI Agent:**
> Fetching top pages... The Home page and the Pricing page are your most visited content this week.

---

**👤 You:**
> "List all sites configured in Matomo."

**🤖 AI Agent:**
> Querying sites... I found 3 sites: 'E-commerce Shop', 'Blog', and 'Support Portal'.


## Installation & Usage

To install and use the **Matomo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/matomo](https://vinkius.com/mcp/matomo)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

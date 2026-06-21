# AB.GL MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/abgl)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/abgl-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/abgl-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Shorten URLs, track click performance, and manage branded links with real-time analytics for every campaign.

## Description
Connect your **AB.GL** account to any AI agent and manage your entire link shortening and analytics workflow through natural conversation.

### What you can do

- **Create Short Links** — Shorten any URL with an optional custom alias for branded campaigns
- **Link Management** — List, inspect, update, and delete shortened URLs from your account
- **Click Analytics** — View detailed click statistics including referrers, devices, and geographic data for any link
- **Bio Link Pages** — List and inspect bio link pages with blocks and appearance settings
- **Custom Domains** — View all custom domains configured for your short links
- **Account Monitoring** — Verify API connectivity and account status

### How it works

1. Subscribe to this server
2. Enter your **API Key** from your AB.GL account settings
3. Start managing links from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing Teams** — create branded short links and track campaign performance in real time
- **Content Creators** — manage bio link pages and monitor audience engagement
- **Growth Engineers** — automate link creation for A/B testing and attribution tracking


## Available Tools
- **check_abgl_status**: Verify API connectivity
- **create_short_link**: gl.

Create a short link
- **delete_link**: Delete a short link
- **get_bio_link**: Get bio page details
- **get_link_stats**: Get link analytics
- **get_link**: Get link details
- **list_bio_links**: List bio pages
- **list_domains**: gl short links.

List custom domains
- **list_links**: gl account with click counts and creation dates.

List all short links
- **update_link**: Update a short link


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AB.GL** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Shorten https://example.com/long-campaign-url with alias 'q4sale'."

**🤖 AI Agent:**
> Done! Your short link is https://ab.gl/q4sale (ID: lnk_4921). It redirects to the campaign URL. Would you like to check its analytics later?

---

**👤 You:**
> "Show me click statistics for link lnk_4921."

**🤖 AI Agent:**
> Link lnk_4921 has 1,247 total clicks. Top referrers: LinkedIn (42%), Twitter (31%), Direct (27%). Devices: Mobile 68%, Desktop 32%. Top country: United States (580 clicks).

---

**👤 You:**
> "List all my bio link pages."

**🤖 AI Agent:**
> You have 3 bio pages: 'Marketing Team' (12 links, 3.4k views), 'Product Launch Q4' (8 links, 1.2k views), and 'Personal Portfolio' (5 links, 890 views). Would you like to inspect any of them?


## Installation & Usage

To install and use the **AB.GL** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/abgl](https://vinkius.com/mcp/abgl)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

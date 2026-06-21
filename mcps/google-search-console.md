# Google Search Console MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/google-search-console)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/google-search-console-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/google-search-console-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Monitor your website's search performance, fix indexing issues, and manage sitemaps via AI.

## Description
Connect your **Google Search Console** to your AI agent and take control of your technical SEO. Use natural language to query search traffic data, inspect URLs for indexing errors, and manage your sitemaps across all your verified web properties.

### What you can do

- **Search Analytics** — Query clicks, impressions, CTR, and position data by date, country, device, or specific queries
- **URL Inspection** — Instantly check if a specific page on your site is indexed by Google and identify any mobile usability or indexing errors
- **Sitemap Management** — List all submitted sitemaps, verify their status, and submit new ones directly from the chat
- **Site Management** — View all your verified properties and add or remove sites from your Search Console account

### How it works

1. Subscribe to this server
2. Enter your Google OAuth Client ID and Secret
3. Complete the secure Google authorization flow
4. Start analyzing your SEO performance from Claude, Cursor, or any MCP-compatible client

Stop wrestling with the Search Console UI. Your AI agent acts as your dedicated technical SEO analyst.

### Who is this for?

- **SEO Specialists** — quickly pull search query data for specific landing pages or verify if a recently launched page has been indexed
- **Web Developers** — automate URL inspections during deployments and ensure sitemaps are processed correctly
- **Content Marketers** — find out what keywords are driving traffic to your blog posts through simple conversational queries


## Available Tools
- **add_site**: Add a site to Search Console
- **delete_site**: Remove a site from Search Console
- **delete_sitemap**: Delete a submitted sitemap
- **get_site**: Get details for a specific site
- **get_sitemap**: Get details about a specific sitemap
- **inspect_url**: Inspect the index status of a specific URL
- **list_sitemaps**: List submitted sitemaps for a site
- **list_sites**: List verified sites in Search Console
- **query_search_analytics**: Query search traffic data
- **submit_sitemap**: Submit a new sitemap


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Google Search Console** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if https://mysite.com/new-post is indexed by Google."

**🤖 AI Agent:**
> Inspecting URL... The URL is successfully indexed and can appear in Google Search results. Mobile usability is marked as 'Pass'.

---

**👤 You:**
> "What were the top 5 search queries for our site last week?"

**🤖 AI Agent:**
> Querying search analytics... Here are your top 5 queries from the last 7 days:
1. 'buy coffee beans online' (450 clicks, 1200 impressions)
2. 'best dark roast' (320 clicks, 900 impressions)
3. 'organic espresso' (210 clicks, 800 impressions)
4. 'fair trade coffee' (150 clicks, 600 impressions)
5. 'coffee subscription box' (90 clicks, 400 impressions)

---

**👤 You:**
> "Submit our new sitemap at https://mysite.com/sitemap-products.xml to Search Console."

**🤖 AI Agent:**
> Sitemap successfully submitted to Google Search Console.
**Status**: Pending processing by Googlebot. We will monitor its progress actively.


## Installation & Usage

To install and use the **Google Search Console** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/google-search-console](https://vinkius.com/mcp/google-search-console)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Mozscape MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mozscape)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mozscape-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mozscape-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Analyze SEO metrics, domain authority, and link profiles directly from your AI agent using the Mozscape API.

## Description
Connect your **Mozscape** account to any AI agent to perform deep SEO analysis and link auditing through natural conversation.

### What you can do

- **Site Metrics** — Fetch Domain Authority (DA), Page Authority (PA), and Spam Scores for any URL or domain.
- **Link Analysis** — List inbound links, filter them by anchor text or source domain, and check link status.
- **Competitive Intelligence** — Use link intersect tools to find common backlink sources between multiple competitors.
- **Brand Authority** — Retrieve the exclusive Moz Brand Authority™ score to measure a site's brand strength.
- **Historical Data** — Track how metrics change over time with daily or monthly history lookups.

### How it works

1. Subscribe to this server
2. Enter your Moz API Token
3. Start auditing SEO profiles from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SEO Specialists** — automate backlink audits and competitor research without manual exports
- **Content Marketers** — evaluate the authority of potential guest post sites or partners instantly
- **Growth Engineers** — integrate SEO data into development workflows for programmatic analysis


## Available Tools
- **fetch_brand_authority**: Get Brand Authority score for a site
- **fetch_distributions**: Get link distribution data
- **fetch_histories**: Get daily or monthly metric histories
- **fetch_link_intersect**: Find sites linking to multiple targets
- **fetch_link_status**: Check if a specific link exists
- **fetch_multiple_site_metrics**: Get metrics for up to 50 URLs
- **fetch_site_metrics**: Get metrics (DA, PA, Spam Score) for a single URL
- **filter_links_by_anchor**: Get links matching a specific anchor text
- **filter_links_by_domain**: Get links originating from a specific root domain
- **filter_recently_gained_domains**: Get recently gained linking root domains
- **filter_recently_lost_domains**: Get recently lost linking root domains
- **list_anchor_text**: Get normalized anchor text data
- **list_linking_domains**: Get a list of linking root domains
- **list_links**: Get a list of links to a target
- **lookup_quota**: Check Moz API V3 quota usage
- **v2_anchor_text**: V2: Get normalized anchor text strings
- **v2_final_redirect**: V2: Follow known redirects to find final destination
- **v2_global_top_pages**: V2: Get top 500 pages in the entire Moz index
- **v2_global_top_root_domains**: V2: Get top 500 root domains in the Moz index
- **v2_link_intersect**: V2: Identify sites linking to competitors but not to you
- **v2_link_status**: V2: Verify if a link exists
- **v2_top_pages**: V2: List the most linked-to pages on a domain
- **v2_url_metrics**: V2: Bulk retrieval of URL metrics
- **v2_usage_data**: V2: Get usage data for the current billing period


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mozscape** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get SEO metrics for moz.com"

**🤖 AI Agent:**
> I've retrieved the metrics for moz.com. It has a Domain Authority of 91, a Page Authority of 78, and a Spam Score of 1%.

---

**👤 You:**
> "Find sites that link to both apple.com and microsoft.com"

**🤖 AI Agent:**
> Using the link intersect tool, I found several high-authority domains linking to both, including techcrunch.com, wired.com, and theverge.com.

---

**👤 You:**
> "What is the Brand Authority score for nike.com?"

**🤖 AI Agent:**
> The Brand Authority™ score for nike.com is 98, indicating an exceptionally strong brand presence in the Moz index.


## Installation & Usage

To install and use the **Mozscape** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mozscape](https://vinkius.com/mcp/mozscape)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

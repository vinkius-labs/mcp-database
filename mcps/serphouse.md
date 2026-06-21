# SERPHouse MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/serphouse)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/serphouse-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/serphouse-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Grant your AI agent unfiltered real-time access to Google and Bing SERP data to scrape organic search results and dynamic pricing.

## Description
Equip your AI assistant with the ultimate crawler module engineered for unbridled search engine access. The SERPHouse MCP integration overcomes the constraints of offline AI knowledge by granting direct, proxy-rotated querying power over Google and Bing endpoints. Seamlessly transform your agent into a high-performance web discovery engine without triggering Captcha blocks.


## Available Tools
- **get_account_info**: Retrieves SERPHouse account information
- **google_images**: Searches for images on Google
- **google_news**: Searches for news on Google
- **google_scholar**: Searches for scholarly articles on Google Scholar
- **google_search**: Supports advanced parameters like "location" and "lang".

Performs a search on Google
- **google_shopping**: Searches for products on Google Shopping
- **google_videos**: Searches for videos on Google
- **list_locations**: Lists supported locations for SERP queries
- **bing_images**: Searches for images on Bing
- **bing_news**: Searches for news on Bing
- **bing_search**: Performs a search on Bing


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SERPHouse** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Run a targeted Google Scholar query aimed at finding recent papers on 'quantum consciousness theory' focusing on latest available years."

**🤖 AI Agent:**
> Deploying `google_scholar`, I aggregated the latest results targeting 'quantum consciousness theory'. The SERP metadata successfully listed major academic journals showcasing papers from Stuart Hameroff with more than 200 distinct citations.

---

**👤 You:**
> "Search Bing News locally from a generic 'United Kingdom' location tag to see the latest headlines on economic metrics."

**🤖 AI Agent:**
> Using internal location IDs referencing 'United Kingdom', I checked `bing_news`. There is currently tremendous discussion around new border control metrics influencing local economic exports. I'll summarize the top 10 articles retrieved.


## Installation & Usage

To install and use the **SERPHouse** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/serphouse](https://vinkius.com/mcp/serphouse)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

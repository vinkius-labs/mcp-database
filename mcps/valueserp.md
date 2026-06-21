# ValueSERP MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/valueserp)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/valueserp-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/valueserp-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Bring real-time Google Search data into your AI agent. Search organically, find images, news, scholars, and related questions without getting blocked.

## Description
Connect your **ValueSERP** account to any AI agent and integrate highly scalable, reliable, and real-time Google search data parsing into your conversational flow, bypassing CAPTCHAs and blocks.

### What you can do

- **Comprehensive Google Search** — Perform rapid programmatic queries across Google Organic, Images, News, Videos, and Scholar straight from your agent's interface.
- **E-Commerce & Local SEO** — Access raw Google Places and Google Shopping data to analyze competitor margins, finding ratings, coordinates, and product price shifts.
- **Intent Discovery** — Retrieve predictive Google Autocomplete suggestions and 'People Also Ask' related snippets to understand semantic search behavior.
- **Advanced SERP Queries** — Execute highly customized parameter inputs targeting specific granular geolocation bounds (gl), language codes (hl), and synthetic device overrides.

### How it works

1. Subscribe to this server
2. Enter your ValueSERP API Key
3. Start pulling live web intelligence from Claude, Cursor, or any MCP-compatible client

Your AI agent becomes a robust, unblockable search intelligence engine.

### Who is this for?

- **SEO Analysts** — rapidly check organic positions and extract 'People Also Ask' questions for content marketing strategies directly from the chat.
- **Growth Marketers** — scrape Google Shopping competitors and build dynamic pricing alerts using agentic reasoning.
- **Researchers** — collect Google Scholar abstracts naturally and fast-track academic literature reviews without leaving your workspace.
- **AI Developers** — augment your agent's knowledge with live, real-time Google Search results seamlessly.


## Available Tools
- **custom_serp_search**: Provide parameters as a JSON object.

Executes a highly customized Google search with advanced parameters
- **get_search_suggestions**: Retrieves predictive search suggestions from Google autocomplete
- **google_image_search**: Returns direct URLs to image files.

Searches for images on Google
- **google_news_search**: Searches for news articles on Google
- **google_search**: Provide a query string and optional location.

Performs a standard Google search for organic results
- **google_places_search**: Provide a place name and location.

Searches for local businesses and places on Google Maps
- **google_scholar_search**: Searches for academic publications and abstracts on Google Scholar
- **google_shopping_search**: Returns product names, prices, and merchant links.

Searches for products and prices on Google Shopping
- **google_video_search**: Searches for video content on Google
- **get_related_questions**: Retrieves "People Also Ask" questions and answers from Google


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ValueSERP** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search Google Scholar for recent papers on 'quantum computing error correction'."

**🤖 AI Agent:**
> Here are the top results from Google Scholar for 'quantum computing error correction'. I found 8 highly-cited abstracts in the first page. For instance, 'Surface codes: Towards practical large-scale quantum computation' by Fowler et al. Would you like me to extract the citations count and PDF links for all of them?

---

**👤 You:**
> "Find the top business ratings for 'pizza places in Chicago' using Google Places."

**🤖 AI Agent:**
> I've pulled the local pack from Google Places for 'pizza places in Chicago'. The top-rated spots are Lou Malnati's Pizzeria (4.6 stars, 12,304 reviews), Giordano's (4.5 stars), and Pequod's Pizza (4.6 stars). Below is a table with their addresses, exact GPS coordinates, and current open/closed status.

---

**👤 You:**
> "Check Google Autocomplete suggestions when someone types 'how to start a'."

**🤖 AI Agent:**
> Based on real-time Google Autocomplete, the most frequent continuations for 'how to start a' are currently: 'business', 'clothing brand', 'llc', 'conversation', 'cover letter', and 'nonprofit'. These reflect high-volume search intents. Let's dig into 'clothing brand' if you'd like to do further research on that vertical.


## Installation & Usage

To install and use the **ValueSERP** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/valueserp](https://vinkius.com/mcp/valueserp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# Diffbot MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/diffbot)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/diffbot-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/diffbot-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Automate web data extraction via Diffbot — turn any website into structured JSON data for articles, products, discussions, and more directly from any AI agent.

## Description
Connect your **Diffbot** account to any AI agent and take full control of your automated web data extraction through natural conversation.

### What you can do

- **Automated Page Classification** — Use the Analyze API to automatically determine if a page is an article, product, or list and extract structured data natively
- **Article Extraction** — Extract news, blog, or article content into clean HTML and plain text, identifying authors, dates, and categorical classifications limitlessly
- **E-commerce Intelligence** — Capture structured product details including precise pricing, brand mappings, SKU, and specifications across any web boundary
- **Media & Social Auditing** — Extract primary images and embedded video metadata, or analyze forum threads and reviews with automated sentiment scoring
- **List & Search Scraping** — Identify bounded directories and search results on any page to extract arrays of item titles and links strictly
- **Job Posting Analysis** — Retrieve explicitly mapped job titles, employers, and salary vectors from recruitment pages to monitor market trends
- **Custom Rule Execution** — Execute user-defined custom extraction logic by bridging raw URLs to your trained Diffbot dashboard rulesets

### How it works

1. Subscribe to this server
2. Enter your Diffbot Developer Token (found in your Diffbot Dashboard > Manage Token)
3. Start transforming the web into data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — extract structured data from thousands of websites without writing complex scrapers or selectors
- **Market Researchers** — monitor competitor products and pricing across the web using natural language
- **Content Marketers** — summarize articles and monitor brand mentions in forum discussions in real-time
- **Developers** — test and debug web extraction pipelines and custom Diffbot rules through natural conversation


## Available Tools
- **analyze_page**: Diffbot uses ML to determine if the page is an article, product, image, video, event, list, or job, and returns the appropriate structured JSON. Excellent generalized entry point.

Automatically classify and extract page data using Diffbot Analyze API
- **extract_article**: Pass optional discussion=false to skip extracting comments.

Extract news, blog, or article content using Diffbot Article API
- **extract_custom_api**: Diffbot will extract data according to your custom ruleset.

Extract using a user-defined custom Diffbot API
- **extract_discussion**: Extract forum threads, reviews, or comments using Diffbot Discussion API
- **extract_event**: Extract event schedules and details using Diffbot Event API
- **extract_image**: Extract main images from a page using Diffbot Image API
- **extract_job**: Extract job postings using Diffbot Job API
- **extract_list**: Extract lists or search results using Diffbot List API
- **extract_product**: Extract e-commerce product details using Diffbot Product API
- **extract_video**: Extract video content and metadata using Diffbot Video API


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Diffbot** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Extract the article content from: https://techcrunch.com/2024/01/01/ai-trends"

**🤖 AI Agent:**
> Article extracted! Title: 'Top AI Trends for 2024'. Author: Jane Doe. I have the clean text body and the original HTML available. Would you like me to summarize the key points?

---

**👤 You:**
> "What is the price and SKU for this product: [E-commerce URL]"

**🤖 AI Agent:**
> Retrieving product data... Name: 'Noise-Cancelling Headphones'. Price: $299.00. SKU: 'NC-700-BLK'. Availability: In Stock. I also have 15 detailed specifications available.

---

**👤 You:**
> "Search for news about 'OpenAI' using: [News List URL]"

**🤖 AI Agent:**
> Analyzing news list... I found 5 related items including 'New Model Release' and 'Partnership with Apple'. Each item has a title, direct link, and content snippet. Would you like me to extract the full text for any of these?


## Installation & Usage

To install and use the **Diffbot** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/diffbot](https://vinkius.com/mcp/diffbot)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

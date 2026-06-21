# DataDive MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/datadive)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/datadive-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/datadive-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ecommerce](../categories/ecommerce.md)

Equip your AI agent to retrieve Amazon seller insights, keyword rankings, and niche analytics directly via the DataDive API.

## Description
Integrate **DataDive**, the advanced toolset for Amazon sellers, directly into your AI workflow. Monitor product niches, track keyword rankings with Rank Radar, and analyze your sales profits and inventory levels using natural language.

### What you can do

- **Niche Analysis** — List and retrieve detailed metrics for product niches you are tracking.
- **Keyword Tracking** — Monitor organic and PPC rankings for any ASIN using Rank Radar data.
- **Profit Oversight** — Retrieve a high-level summary of your Amazon sales and financial performance.
- **Inventory Management** — Check current stock levels and get restock recommendations via chat.

### How it works

1. Connect the DataDive integration to your AI assistant.
2. Authorize using your DataDive API Key (found in your account settings).
3. Manage your Amazon business and market research through intuitive conversation.

### Who is this for?

- **Amazon Sellers** — Quickly check rankings and profit summaries on the go.
- **Market Researchers** — Explore niche data and competitor ASINs during product planning.
- **Inventory Managers** — Monitor stock levels and plan restocks without complex reporting tools.


## Available Tools
- **get_account_details**: Returns metadata such as account tier, connected marketplace integrations, and subscription status.

Retrieve metadata for your DataDive account
- **get_inventory_status**: Returns units in stock, inbound shipments, and daily sell-through rates to provide restock lead-time alerts.

Check current inventory levels and restock recommendations
- **get_niche_details**: Resolves high-level metrics such as average price, total niche volume, and competition score based on aggregated Amazon data.

Get detailed analytics and metrics for a specific niche
- **get_rank_radar**: Returns real-time organic and sponsored positions across tracked keywords, enabling competitive visibility analysis.

Get keyword ranking data (organic and PPC) for a specific ASIN
- **get_high_volume_keywords**: Returns keywords with significant search volume and favorable competition metrics for ranking priority.

List top performing keywords based on search volume and competition
- **list_competitor_asins**: Includes product titles, brand names, and baseline performance data.

List all ASINs (competitors) tracked within a niche
- **list_niche_keywords**: Returns search volume, relevancy scores, and priority indicators for product ranking and SEO optimization.

List all keywords and search volumes for a specific niche
- **list_product_niches**: Returns a collection of niche objects including name, marketplace (e.g., Amazon US), and tracking status.

List all product niches tracked in your DataDive account
- **get_profits_summary**: Aggregates sales data, fees, and advertising spend to return net profit margins and ROI for the connected seller account.

Retrieve a high-level financial summary of your Amazon sales
- **search_all_keywords**: Matches against the global keyword repository in the user's account to find occurrences and metrics across multiple categories.

Search for keywords across all your tracked niches


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DataDive** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the ranking data for ASIN 'B08S9DF7' using Rank Radar."

**🤖 AI Agent:**
> I've retrieved the Rank Radar data for ASIN 'B08S9DF7'. It is currently ranked #3 organically for 'noise-canceling headphones' and #5 for 'wireless earbuds'. PPC ranking is #1 for both. Would you like a historical trend?

---

**👤 You:**
> "List all product niches I'm currently tracking in DataDive."

**🤖 AI Agent:**
> I've found 4 niches in your account: 'Yoga Mats', 'Bamboo Bedding', 'Reusable Straws', and 'Pet Grooming Kits'. Would you like to see the search volume trends for the 'Bamboo Bedding' niche?

---

**👤 You:**
> "What is my profit summary for the last 30 days?"

**🤖 AI Agent:**
> In the last 30 days, your Amazon sales generated a gross profit of $12,450 with a net margin of 18%. Your best-selling niche was 'Bamboo Bedding'. Should I show you the breakdown of Amazon fees for this period?


## Installation & Usage

To install and use the **DataDive** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/datadive](https://vinkius.com/mcp/datadive)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

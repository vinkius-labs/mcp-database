# Mobile Action MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mobile-action)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/mobile-action-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/mobile-action-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

All-in-one app marketing intelligence via Mobile Action — track ASO, keywords, and ad creatives directly from your AI agent.

## Description
Connect your **Mobile Action** account to your AI agent and gain a competitive edge in the app stores through natural conversation.

### What you can do

- **ASO Intelligence** — Track keyword rankings and history for iOS and Android apps across different countries.
- **Market Estimations** — Access estimated downloads, revenue, and active users for any app in the store.
- **Ad Intelligence** — Analyze ad creatives and distribution strategies used by your competitors.
- **Keyword Expansion** — Get related keyword suggestions to optimize your store listing.
- **App Discovery** — Search for apps and monitor top charts by category and country.
- **Reputation Monitoring** — Retrieve app reviews and historical rating performance.

### How it works

1. Subscribe to this server
2. Enter your Mobile Action API Token
3. Start querying app market intelligence from Claude, Cursor, or any MCP client

### Who is this for?

- **App Marketers** — quickly check keyword rankings or ad creatives without opening the dashboard.
- **Product Managers** — monitor competitor performance and market estimations directly from your chat.
- **ASO Specialists** — automate the retrieval of keyword suggestions and ranking history.


## Available Tools
- **get_ad_creatives**: Get app advertising creatives
- **get_app_info**: Get detailed app store information
- **get_app_reviews**: Get app customer reviews
- **get_cpp_details**: Get Custom Product Page details
- **get_keyword_ranking**: Get keyword ranking history
- **get_market_estimations**: Get download and revenue estimations
- **get_rating_history**: Get app rating history
- **get_related_keywords**: Get related ASO keywords
- **get_top_apps**: Get top charts by category
- **get_tracked_apps**: List apps tracked in the dashboard
- **get_tracked_keywords**: List keywords tracked in the dashboard
- **search_apps**: Search for apps in store


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mobile Action** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the top 10 Finance apps in the US App Store."

**🤖 AI Agent:**
> Retrieving top charts... The top Finance apps in the US are: 1. PayPal, 2. Cash App, 3. Venmo, 4. Zelle, 5. Rocket Money. Shall I get more details on PayPal's ranking history?

---

**👤 You:**
> "What is the keyword ranking history for 'fitness' in the UK for app ID 123456789?"

**🤖 AI Agent:**
> Fetching ranking history... For the keyword 'fitness', your app has moved from #15 to #8 in the last 30 days. It currently holds the highest position since January. Would you like related keyword suggestions to further improve your visibility?

---

**👤 You:**
> "Search for news related apps in Brazil on Android."

**🤖 AI Agent:**
> Searching Google Play Brazil... I found several news apps including 'G1', 'UOL', 'CNN Brasil', and 'Folha de S.Paulo'. Shall I retrieve the market estimations for G1?


## Installation & Usage

To install and use the **Mobile Action** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mobile-action](https://vinkius.com/mcp/mobile-action)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

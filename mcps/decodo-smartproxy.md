# Decodo (Smartproxy) MCP Server

Manage your Decodo (formerly Smartproxy) network infrastructure — list proxy endpoints, monitor bandwidth, and fetch residential proxy configurations with your AI.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/decodo-smartproxy)

## Overview
**Category:** developer-tools
**Tools Count:** 9

## Description
Connect your **Decodo (Smartproxy)** account to any AI agent to control your proxy endpoints, audit infrastructure, and track SERP/scraping data seamlessly. Interact with your server architecture and networking limits using natural language without jumping out of your IDE.

### What you can do

- **Inventory Management** — Effortlessly pull a list of active `list_proxy_endpoints`, `list_datacenter_proxies`, and `list_residential_proxies`
- **Live Bandwidth Monitoring** — Run `get_traffic_usage` directly inside the AI prompt to see if you are about to hit your monthly data quota cap
- **Bot Statistics** — Evaluate the health of your bots automatically by checking `get_scraper_stats` for eCommerce and SERP scrapers
- **Reselling & Accounts** — Generate your `list_subscriptions` details, retrieve your general account health, or list all nested sub-users associated with the account

### How it works

1. Subscribe to this server
2. Enter your Smartproxy (Decodo) API Key
3. Start using Claude, Cursor, or any MCP-compatible client to query your IP pools

Stop clicking through multiple dashboard pages just to copy-paste your internal proxy endpoint port. Let your agent do it programmatically.

### Who is this for?

- **Data Engineers & Scrapers** — pull the precise endpoint metrics, load stats on failure rates, and check if your pools are active while drafting crawler scripts
- **Network Admins** — list assigned dedicated networks (`list_dedicated_proxies`) to diagnose potential rate-limiting errors from CLI
- **SaaS Operators** — monitor sub-user metrics and their localized bandwidth usage effortlessly


## Available Tools
- **get_account_details**: Retrieves Smartproxy account information
- **get_scraper_stats**: Retrieves statistics for scraping APIs
- **get_traffic_usage**: Retrieves traffic usage statistics
- **list_datacenter_proxies**: Lists datacenter proxy configurations
- **list_dedicated_proxies**: Lists dedicated proxy assignments
- **list_proxy_endpoints**: Lists available proxy endpoints
- **list_residential_proxies**: Lists residential proxy configurations
- **list_sub_users**: Lists all proxy sub-users
- **list_subscriptions**: Lists active proxy subscriptions


## Installation & Usage

To install and use the **Decodo (Smartproxy)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/decodo-smartproxy](https://vinkius.com/mcp/decodo-smartproxy)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

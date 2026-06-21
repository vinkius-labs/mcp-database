# Kevel MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/kevel)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/kevel-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/kevel-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage ad campaigns, inventory, and creatives via the Kevel Management API.

## Description
Connect your **Kevel** (formerly Adzerk) account to any AI agent to streamline your ad serving operations. This MCP server allows your agent to manage advertisers, campaigns, flights, and inventory sites directly through natural language.

### What you can do

- **Campaign Management** — List and retrieve detailed configurations for campaigns and flights
- **Advertiser Oversight** — Query and manage advertising entities and their metadata
- **Inventory Control** — List and inspect sites, zones, and channels to manage your ad placements
- **Creative Audit** — Access a comprehensive list of ad creatives and individual ad instances
- **Format Exploration** — List supported ad types and sizes to ensure correct technical implementations

### How it works

1. Subscribe to this server
2. Enter your Kevel Management API Key (X-Adzerk-ApiKey)
3. Start managing your ad server from Claude, Cursor, or any MCP client

### Who is this for?

- **Ad Operations Managers** — Monitor campaign statuses and flight configurations on the fly
- **Product Managers** — Quickly check inventory availability and placement details without logging into the dashboard
- **Ad Tech Engineers** — Retrieve technical metadata for creatives and ad types during integration


## Available Tools
- **get_campaign**: Get details for a specific campaign
- **list_zones**: List all zones
- **list_ad_types**: g., banner, native).

List available ad types
- **list_ads**: List all ads
- **list_advertisers**: List all advertisers in Kevel
- **list_campaigns**: List all campaigns
- **list_channels**: List all channels
- **list_creatives**: ) uploaded to the account.

List all creatives
- **get_advertiser**: Get details for a specific advertiser
- **list_flights**: List all flights
- **list_sites**: List all sites


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Kevel** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all active campaigns in Kevel."

**🤖 AI Agent:**
> I've retrieved your campaigns. You have 10 active campaigns, including 'Summer Sale 2024' and 'New Product Launch'. Would you like to see the flights for any of them?

---

**👤 You:**
> "List all ad zones for the site with ID 12345."

**🤖 AI Agent:**
> I found 5 zones for site 12345: 'Header Banner', 'Sidebar Native', and 3 others. All zones are currently active.

---

**👤 You:**
> "What ad types are supported in my Kevel account?"

**🤖 AI Agent:**
> I've listed the supported ad types. Your account supports 15 formats, including 'Banner', 'Native', 'Video', and 'Interstitial'.


## Installation & Usage

To install and use the **Kevel** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/kevel](https://vinkius.com/mcp/kevel)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

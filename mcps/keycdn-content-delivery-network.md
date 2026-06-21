# KeyCDN (Content Delivery Network) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/keycdn-content-delivery-network)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/keycdn-content-delivery-network-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/keycdn-content-delivery-network-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Manage edge caching via KeyCDN — purge zones and URLs, manage pull zones, and monitor traffic bandwidth.

## Description
Connect your **KeyCDN** account to any AI agent and take full control of your global edge caching and content delivery infrastructure through natural conversation.

### What you can do

- **Cache Orchestration** — Purge the entire cache for a zone or perform granular invalidations for specific file URLs to ensure fresh content delivery instantly
- **Zone Management** — Create and configure new Pull Zones to connect your origin servers to KeyCDN's global edge locations directly from your agent
- **Custom Domain Aliases** — Bind and manage custom domain mappings (CNAMEs) to existing zones to maintain branded asset delivery URLs securely
- **Traffic Analytics** — Retrieve detailed bandwidth consumption reports over specific time periods to monitor your CDN spending and usage patterns
- **Origin Audit** — Inspect detailed caching rules, TLS settings, and origin server configurations assigned to your active zones
- **Infrastructure Control** — Enable, disable, or permanently delete distributed acceleration zones to manage your content delivery pipeline in real-time

### How it works

1. Subscribe to this server
2. Enter your KeyCDN API Key
3. Start managing your content delivery from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Frontend Developers** — verify asset delivery and purge specific URLs after code deployments without leaving your IDE
- **SREs & DevOps** — monitor CDN traffic and manage zone configurations across multiple production environments through natural conversation
- **Site Administrators** — audit custom domain aliases and verify SSL/TLS statuses for global asset delivery efficiently


## Available Tools
- **add_zone_alias**: g. assets.company.com) to an existing KeyCDN zone. DNS CNAME records should be updated accordingly.

Add a custom domain alias to a KeyCDN zone
- **add_pull_zone**: Create a new KeyCDN pull zone
- **delete_zone_alias**: Delete a custom domain alias from a KeyCDN zone
- **delete_zone**: Instantly revokes wildcard subdomains and drops proxy connections natively.

Delete a specific KeyCDN zone
- **get_zone**: Get details for a specific KeyCDN zone
- **list_zone_aliases**: List custom domain aliases for all zones
- **list_traffic_reports**: List traffic bandwidth consumption reports
- **list_zones**: Returns immutable `.kxcdn.com` endpoints and zone configurations.

List all KeyCDN zones
- **purge_specific_url**: g., `/app.css`), avoiding a full zone cache purge.

Purge a specific cached URL in a KeyCDN zone
- **purge_zone_cache_all**: Purge the entire cache for a KeyCDN zone


## 💬 Prompt Examples

Here are some examples of how you can interact with the **KeyCDN (Content Delivery Network)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my KeyCDN zones"

**🤖 AI Agent:**
> I've found 3 zones in your account: 'main-assets' (ID: 123, Endpoint: main-123.kxcdn.com), 'video-streaming' (ID: 456), and 'staging-static' (ID: 789). Which one would you like to see the configuration for?

---

**👤 You:**
> "Purge the cache for this URL in zone 123: https://main-123.kxcdn.com/styles/app.css"

**🤖 AI Agent:**
> Purge request for 'styles/app.css' sent successfully. The resource has been invalidated across the global KeyCDN network. It will be re-fetched from your origin server on the next visitor request.

---

**👤 You:**
> "How much traffic did we use in the last 7 days?"

**🤖 AI Agent:**
> Retrieving traffic reports… In the last 7 days, your account consumed a total of 1.24 TB of bandwidth. The peak usage occurred on Tuesday at 4 PM with 45 GB/hour. Your current credit balance is sufficient for this usage level.


## Installation & Usage

To install and use the **KeyCDN (Content Delivery Network)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/keycdn-content-delivery-network](https://vinkius.com/mcp/keycdn-content-delivery-network)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

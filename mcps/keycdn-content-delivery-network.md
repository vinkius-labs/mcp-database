# KeyCDN (Content Delivery Network) MCP Server

Manage edge caching via KeyCDN — purge zones and URLs, manage pull zones, and monitor traffic bandwidth.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/keycdn-content-delivery-network)

## Overview
**Category:** cloud-infrastructure
**Tools Count:** 10

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


## Installation & Usage

To install and use the **KeyCDN (Content Delivery Network)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/keycdn-content-delivery-network](https://vinkius.com/mcp/keycdn-content-delivery-network)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

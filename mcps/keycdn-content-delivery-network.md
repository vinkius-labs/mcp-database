# KeyCDN (Content Delivery Network) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/keycdn-content-delivery-network)
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


## Available Tools (10)
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


## ❓ FAQ

**Q: Can I purge the entire cache for a specific zone using my agent?**
Yes. Use the `purge_zone_cache_all` tool with your Zone ID. Your agent will instantly trigger a global invalidation across all Edge servers, forcing KeyCDN to re-fetch all assets from your origin upon the next request.

**Q: How do I invalidate a single file instead of purging the whole zone?**
The `purge_specific_url` tool allows for granular cache invalidation. You just need to provide the Zone ID and the absolute URL of the resource (e.g. your CDN subdomain + path) to clear that specific file from the edge nodes.

**Q: Can my agent check how much traffic I've used this month?**
Absolutely. Use the `list_traffic_reports` tool and provide a start and end timestamp. Your agent will retrieve the bandwidth consumption analytics for your account, helping you track CDN usage and spending in real-time.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/keycdn-content-delivery-network](https://vinkius.com/mcp/keycdn-content-delivery-network)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **KeyCDN (Content Delivery Network)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `keycdn-content-delivery-network` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **KeyCDN (Content Delivery Network)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "keycdn-content-delivery-network": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

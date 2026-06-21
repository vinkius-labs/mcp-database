# Webshare MCP Server

Manage residential and datacenter proxies, rotation settings, and authorized IPs on Webshare — the fast and affordable proxy network.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/webshare)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **Webshare** account to any AI agent and take full control of your proxy infrastructure through natural conversation.

### What you can do

- **Proxy Management** — List all assigned residential and datacenter proxy IPs, including ports, credentials, and health status
- **IP Authorization** — Audit and manage your whitelist of authorized IP addresses to grant proxy access to new servers instantly
- **Rotation Control** — Retrieve current proxy rotation and backbone network settings to ensure your crawlers are configured correctly
- **Real-Time Stats** — Monitor your bandwidth consumption and request success/failure rates directly from your agent
- **Immediate Replacement** — Request instant proxy replacements for flagged or blocked IPs within your account quota
- **Quota Monitoring** — Check your account profile, plan limits, and remaining bandwidth before starting large-scale data tasks
- **High-Speed Export** — Generate temporary tokens to export and download your entire proxy list in a single request

### How it works

1. Subscribe to this server
2. Enter your Webshare API Key
3. Start managing your proxy pool through Claude, Cursor, or any MCP-compatible client

No more manual logging into the Webshare dashboard to whitelist an IP or cycle a proxy. Your AI agent becomes your proxy administrator.

### Who is this for?

- **Data Engineers** — automate proxy management and IP whitelisting for large-scale web scraping pipelines
- **DevOps Professionals** — monitor bandwidth usage and manage proxy infrastructure configurations through chat
- **Market Researchers** — quickly retrieve and update proxy lists for geo-targeted data collection
- **Security Researchers** — audit authorized IPs and cycle proxy endpoints for enhanced anonymity and bypass


## Available Tools
- **authorize_new_ip**: Whitelists a new IP address for proxy access
- **export_proxy_list**: Generates a temporary token to download the entire proxy list in a single request
- **get_account_profile**: Retrieves Webshare user profile, including plan limits and bandwidth quotas
- **get_proxy_configuration**: Retrieves current proxy rotation and backbone network settings
- **get_bandwidth_stats**: Retrieves historical bandwidth and request statistics
- **get_replacement_quota**: Checks the available proxy replacement limits for the current cycle
- **list_authorized_ips**: Lists all IP addresses authorized to use proxies without password authentication
- **list_proxies**: Supports pagination.

Lists all assigned proxy IPs with their ports, credentials, and health status
- **revoke_ip_authorization**: Requires the unique ip_id.

Removes an IP address from the authorized whitelist
- **request_proxy_replacement**: Subject to account quotas.

Requests an immediate replacement for a specific proxy IP


## Installation & Usage

To install and use the **Webshare** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/webshare](https://vinkius.com/mcp/webshare)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

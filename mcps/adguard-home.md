# AdGuard Home MCP Server

Manage your AdGuard Home instance — control protection, DNS settings, and filtering rules directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/adguard-home)

## Overview
**Category:** developer-tools
**Tools Count:** 23

## Description
Connect your **AdGuard Home** instance to any AI agent and take full control of your network-wide privacy and security through natural conversation.

### What you can do

- **Server Status** — Monitor server health, active ports, protection states, and version information in real-time.
- **Protection Control** — Toggle global filtering, safe browsing, and parental controls on or off, with optional timed durations.
- **DNS Configuration** — View and update upstream DNS servers, bootstrap settings, and cache parameters (TTL, size, and optimistic caching).
- **Filter Management** — Add new blocklist or allowlist URLs and manage custom user-defined filtering rules.
- **Client Insights** — List and search for persistent or runtime clients, and configure specific security settings for individual devices.
- **Host Auditing** — Instantly check if a specific domain is being filtered or blocked for a particular client.

### How it works

1. Subscribe to this server
2. Enter your AdGuard Home Base URL and credentials (Username/Password)
3. Start managing your network security from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Home Lab Enthusiasts** — monitor and tweak your network-wide ad blocker without opening the web dashboard.
- **Network Administrators** — quickly update upstream DNS providers or check why a specific host is being blocked.
- **Privacy-focused Users** — manage custom filtering rules and client-specific protections through simple voice or text commands.


## Available Tools
- **add_client**: Add a new client
- **add_filter_url**: Add a new filter URL
- **add_rewrite**: Add a DNS rewrite
- **add_static_lease**: Add a DHCP static lease
- **check_host**: Check if a host is filtered
- **configure_tls**: Configure TLS settings
- **get_dhcp_status**: Get DHCP server status
- **get_dns_info**: Get DNS configuration info
- **get_filtering_status**: Get filtering status and lists
- **get_query_log_config**: Get query log configuration
- **get_query_log**: Get DNS query log
- **get_stats**: Get DNS query statistics
- **get_status**: Get AdGuard Home server status
- **get_tls_status**: Get TLS configuration status
- **list_blocked_services**: List all available blocked services
- **list_clients**: List all clients
- **list_rewrites**: List DNS rewrites
- **search_clients**: Search for clients
- **set_dns_config**: Update DNS settings
- **set_protection**: globally.

Enable or disable protection globally
- **set_user_rules**: Set custom user filtering rules
- **update_blocked_services**: Update blocked services schedule
- **update_query_log_config**: Update query log configuration


## Installation & Usage

To install and use the **AdGuard Home** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adguard-home](https://vinkius.com/mcp/adguard-home)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

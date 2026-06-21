# IPRoyal (Proxy Services) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/iproyal-proxy-services)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/iproyal-proxy-services-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/iproyal-proxy-services-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage proxies via IPRoyal — monitor traffic, rotate credentials, and manage whitelisted IPs.

## Description
Connect your **IPRoyal** account to any AI agent and take full control of your global proxy infrastructure and web scraping operations through natural conversation.

### What you can do

- **Account Audit** — Check your account balance and profile details directly from your agent to ensure sufficient funds for large scraping runs
- **Traffic Monitoring** — Retrieve precise bandwidth consumption statistics for your residential and datacenter proxy orders in real-time
- **Credential Rotation** — Instantly update usernames and passwords for specific proxy orders to maintain security hygiene and access control
- **Geo-Targeting Intelligence** — Check proxy IP availability across different countries and retrieve supported country codes for precise geographic targeting
- **Whitelist Management** — Authorize and revoke client IP addresses for user/pass-free access, securing your headless scrapers and servers
- **Proxy Orchestration** — Generate dynamic geo-targeted connection strings with support for sticky sessions and specific country routing

### How it works

1. Subscribe to this server
2. Enter your IPRoyal API Access Token
3. Start managing your proxy network from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Scientists & Researchers** — automate geo-targeted data collection and monitor traffic consumption through natural conversation
- **Security Engineers** — rotate proxy credentials and manage whitelisted IPs across multiple servers and environments efficiently
- **Automation Developers** — generate complex proxy connection strings and verify IP availability before initiating large-scale crawls


## Available Tools
- **add_whitelist_ip**: This is highly recommended for securely authenticating headless scrapers or servers where you do not want to expose proxy credentials in source code.

Authorize a new IP for IPRoyal proxy access
- **get_availability**: Useful to dynamically determine if a target region has sufficient IPs before initiating a geo-targeted crawl. By default targets "residential".

Check proxy IP availability across different countries
- **list_countries**: Contains the specific country codes (e.g., "us", "de") and region identifiers required to construct geo-targeted proxy connection strings (e.g., appending "_country-us" to the password).

Get list of supported geo-targeting countries, cities, and ISPs
- **change_credentials**: If you suspect your proxy credentials have leaked or you need to rotate access keys for security, use this tool to set a new username and password instantly.

Update username/password for an IPRoyal proxy order
- **list_whitelisted_ips**: Whitelisted IPs can connect directly to the proxy endpoints without supplying the username and password in the connection string.

List IPs allowed to connect to IPRoyal without user/pass
- **list_orders**: An order represents a purchased batch of proxy traffic or IPs (e.g., Royal Residential, Sneaker IPs). The response contains order IDs necessary for traffic lookups and credential management.

Get all active proxy orders (Residential, Datacenter)
- **get_profile**: Use this to ensure there are enough funds before executing large scraping runs.

Get IPRoyal account balance and profile details
- **generate_proxy_string**: Standard format is `geo.iproyal.com:10000:username:password`. Pass `country` to append geographic targeting rules, or `session` for sticky IP sessions.

Helper to generate a dynamic geo-targeted proxy string
- **remove_whitelist_ip**: Required for security hygiene when scraping servers are decommissioned or IP addresses change.

Revoke an IP from IPRoyal proxy access
- **get_traffic**: Residential proxies are billed by traffic, so regular monitoring with this endpoint prevents unexpected depletion of funds.

Get precise proxy traffic consumption statistics for an order


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IPRoyal (Proxy Services)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check my IPRoyal account balance"

**🤖 AI Agent:**
> I've retrieved your profile details. Your current account balance is $45.20 USD. Your account status is 'Active' and your email is alex@example.com. Would you like to see your active proxy orders?

---

**👤 You:**
> "How much traffic have I used for order ID '123456'?"

**🤖 AI Agent:**
> For order 123456 (Residential Proxies), you have consumed 12.45 GB of traffic. You have 37.55 GB remaining in your current allocation. Would you like to rotate the credentials for this order?

---

**👤 You:**
> "Generate a proxy connection string for Germany with sticky session"

**🤖 AI Agent:**
> Generating proxy string… For Germany (DE) with a sticky session, your connection string is: `geo.iproyal.com:10000:username_country-de_session-abc123:password`. You can use this directly in your scraping script.


## Installation & Usage

To install and use the **IPRoyal (Proxy Services)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/iproyal-proxy-services](https://vinkius.com/mcp/iproyal-proxy-services)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

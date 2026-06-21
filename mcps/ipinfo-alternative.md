# IPinfo MCP Server

Enrich IP addresses with geolocation, ASN, and WHOIS data directly from your AI agent using IPinfo's industry-leading intelligence.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/ipinfo-alternative)

## Overview
**Category:** security-compliance
**Tools Count:** 10

## Description
Connect **IPinfo** to your AI agent to perform deep IP intelligence lookups. Whether you're investigating security threats, analyzing web traffic, or managing network infrastructure, this server provides instant access to industry-leading IP data.

### What you can do

- **IP Geolocation** — Retrieve precise city, region, country, and postal code data for any IP address.
- **ASN & Network Insights** — Identify Autonomous System details and IP ranges associated with specific domains.
- **WHOIS & Organization Data** — Access comprehensive WHOIS records, including network, organization, and point-of-contact information.
- **Reverse IP Lookups** — Discover which domains are hosted on a specific IP address with pagination support.
- **Enterprise Intelligence** — Fetch advanced data including privacy flags (VPN/Proxy/Tor), carrier details, and abuse contact information.
- **Batch Processing** — Enrich up to 1,000 IP addresses in a single request for high-scale analysis.

### How it works

1. Subscribe to this server
2. Enter your IPinfo Access Token
3. Start querying IP data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Researchers** — Quickly identify the origin and ownership of suspicious IP addresses during incident response.
- **Data Analysts** — Enrich user logs with geographic and network context to understand traffic patterns.
- **DevOps Engineers** — Verify network ranges and hosted domains for infrastructure management.


## Available Tools
- **get_asn**: You can provide just the number or the AS prefix (e.g., 15169 or AS15169).

Retrieve details about an Autonomous System (ASN)
- **batch_enrich_ips**: Batch enrich up to 1,000 IP addresses
- **get_hosted_domains**: Supports pagination.

List domains hosted on a specific IP (Reverse IP)
- **get_enterprise_ip**: Get Enterprise IPinfo data for an IP address
- **get_lite_ip**: Get basic IPinfo Lite data for an IP address
- **get_lookup_ip**: Get Core/Plus/Max IPinfo data for an IP address
- **get_ranges**: Get all IP ranges associated with a domain
- **get_whois_net**: Get IP WHOIS data for a network
- **get_whois_org**: Get IP WHOIS data for an organization
- **get_whois_poc**: Get IP WHOIS data for a point of contact


## Installation & Usage

To install and use the **IPinfo** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ipinfo-alternative](https://vinkius.com/mcp/ipinfo-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

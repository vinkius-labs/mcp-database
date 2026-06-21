# Namecheap MCP Server

Manage your domains, DNS records, SSL certificates and account — check domain availability and configure nameservers.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/namecheap)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect to **Namecheap** and manage your domain portfolio through natural conversation.

### What you can do

- **Domain List** — View all your registered domains with expiration dates and lock status
- **Domain Info** — Get detailed registration and WHOIS info for any domain
- **DNS Management** — View and update DNS records (A, AAAA, CNAME, MX, TXT, NS)
- **Nameservers** — Check current nameserver configuration
- **SSL Certificates** — Browse and inspect your SSL certificates
- **Account Balance** — Check your available account balance
- **Domain Availability** — Check if a domain name is available for registration

### How it works

1. Subscribe to this server
2. Enter your Namecheap API Key and Username
3. Start managing your domains from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Developers** — manage DNS records, check domain availability and monitor domain expirations
- **Domain Investors** — track portfolio, check availability and manage SSL certificates
- **Sysadmins** — configure DNS records, verify nameserver settings and monitor domain status


## Available Tools
- **check_domain_availability**: Returns whether the domain is available, premium status and pricing info.

Check if a domain name is available for registration
- **get_dns_hosts**: ) for a specific domain. Returns host names, record types, values, TTL and MX preferences. Requires the domain's SLD and TLD (e.g. SLD="example", TLD="com").

Get DNS records for a domain
- **get_dns_servers**: Returns the list of DNS servers handling queries for the domain.

Get nameservers for a domain
- **get_domain_info**: Get detailed info for a specific domain
- **get_domain_ns_info**: Get nameserver info for a domain
- **get_domains**: Returns domain names, IDs, creation dates, expiration dates, lock status and expiry status. Supports pagination and search filtering.

List your Namecheap domains
- **get_ssl_certs**: Returns certificate names, types, expiration dates and activation status.

List your SSL certificates
- **get_ssl_info**: Get detailed info for an SSL certificate
- **get_balance**: Returns the available balance in USD.

Get your Namecheap account balance
- **set_dns_hosts**: Requires the domain name and a JSON array of DNS records with name, type, address and optional TTL/MXPref. This replaces ALL existing records, so include all records you want to keep. Record types: A, AAAA, CNAME, MX, TXT, NS, URL, URL301, FRAME.

Set DNS records for a domain


## Installation & Usage

To install and use the **Namecheap** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/namecheap](https://vinkius.com/mcp/namecheap)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

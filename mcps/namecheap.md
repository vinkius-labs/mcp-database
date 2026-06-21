# Namecheap MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/namecheap)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/namecheap-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/namecheap-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your domains, DNS records, SSL certificates and account — check domain availability and configure nameservers.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Namecheap** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my domains."

**🤖 AI Agent:**
> Found 5 domains: example.com (expires: 2026-05-15, unlocked), mywebsite.org (expires: 2025-12-01, locked), test-project.net (expires: 2027-03-20, unlocked), portfolio.dev (expires: 2025-09-10, unlocked), api-service.io (expires: 2026-01-28, unlocked).

---

**👤 You:**
> "Show me the DNS records for example.com."

**🤖 AI Agent:**
> DNS records for example.com: @ A → 93.184.216.34 (TTL: 300), www CNAME → @ (TTL: 1800), @ MX → mail.example.com (pref: 10), @ TXT → "v=spf1 include:_spf.google.com ~all" (TTL: 300), @ NS → dns1.registrar-servers.com.

---

**👤 You:**
> "Is 'myawesomeapp.com' available?"

**🤖 AI Agent:**
> myawesomeapp.com is AVAILABLE for registration. Not a premium domain. Standard .com pricing applies.


## Installation & Usage

To install and use the **Namecheap** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/namecheap](https://vinkius.com/mcp/namecheap)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

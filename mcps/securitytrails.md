# SecurityTrails MCP Server

Uncover IT infrastructure — access DNS history, subdomains, reverse IP lookups, WHOIS data and advanced domain intelligence for ultimate OSINT.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/securitytrails)

## Overview
**Category:** security-compliance
**Tools Count:** 10

## Description
Connect your **SecurityTrails** account to any AI agent and empower your OSINT, bug bounty, and threat intelligence workflows with the world's most comprehensive domain and IP database.

### What you can do

- **Attack Surface Mapping** — Instantly enumerate all subdomains for any target organization to map their external footprint
- **Historical DNS Analysis** — Look back in time at DNS records (A, MX, NS, TXT) to find hidden infrastructure, bypassed firewalls, or legacy systems
- **Reverse IP Lookups** — Find all domains hosted on a specific IP address to identify shared hosting or related corporate assets
- **Advanced Threat Hunting** — Use the SecurityTrails DSL (Domain Specific Language) to query the entire internet for specific tech stacks or vulnerable infrastructure
- **Ownership Intelligence** — Access current and historical WHOIS records to track domain ownership changes and unmask hidden threat actors
- **Corporate Associations** — Discover domains strongly associated with your primary target to expand your investigation scope

### How it works

1. Subscribe to this server
2. Sign up at [SecurityTrails](https://securitytrails.com/) to get your API key (Free tier available)
3. Run intelligence queries directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Researchers & Pentesters** — accelerate recon and asset discovery during engagements
- **Bug Bounty Hunters** — find forgotten subdomains and out-of-scope assets associated with target companies
- **Threat Intelligence Analysts** — correlate IPs, domains and WHOIS records to track APT infrastructure
- **Brand Protection Teams** — identify typosquatting and malicious domains targeting your organization
- **System Administrators** — audit their own external attack surface and verify DNS propagation


## Available Tools
- **get_api_usage**: Check current SecurityTrails API quota usage
- **get_associated_domains**: Great for expanding the scope of an investigation.

Find other domains associated with a target domain
- **get_dns_history**: Useful for finding old IPs that might still be hosting vulnerable software, or tracking infrastructure migration over time.

Retrieve historical DNS records for a domain
- **get_domain_tags**: Get classification tags for a domain
- **get_domains_by_ip**: Essential for understanding shared hosting environments or identifying hidden vhosts.

Find all domains pointed to a specific IP address
- **get_domain_details**: Essential for mapping out a target domain's existing infrastructure.

Get complete domain intelligence and current DNS records
- **get_subdomains**: Critical for attack surface mapping and asset discovery. Returns both active and inactive subdomains.

Discover all subdomains for a given domain
- **get_whois**: Get current WHOIS information for a domain
- **search_dsl**: Examples: `ipv4="1.1.1.1" AND mx="alt1.aspmx.l.google.com"` or `whois_email="admin@example.com"`. Check SecurityTrails docs for full DSL syntax.

Advanced search using SecurityTrails DSL
- **get_whois_history**: Useful for OSINT investigations to uncover historical owners before privacy protection was enabled.

Retrieve historical WHOIS records for a domain


## Installation & Usage

To install and use the **SecurityTrails** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/securitytrails](https://vinkius.com/mcp/securitytrails)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

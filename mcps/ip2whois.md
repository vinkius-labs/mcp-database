# IP2WHOIS MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ip2whois)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ip2whois-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ip2whois-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Look up domain registration details, ownership information, and expiration dates with instant WHOIS queries at scale.

## Description
Connect your **IP2WHOIS** account to any AI agent and access comprehensive domain intelligence through natural conversation.

### What you can do

- **WHOIS Lookup** — Get complete registration records for any domain including dates, registrar, and contacts.
- **Domain Age** — Calculate how old a domain is in days and years.
- **Expiry Monitoring** — Check when domains expire and how many days remain.
- **Registrar & Nameservers** — Extract registrar details and DNS nameserver configurations.
- **Availability Check** — Determine if a domain is available for registration.
- **Reverse IP** — Find all domains hosted on a specific IP address.
- **Bulk Lookup** — Query up to 10 domains in a single operation.

### How it works

1. Subscribe to this server
2. Enter your IP2WHOIS API key (free tier: 500 queries/month)
3. Start querying domains from Claude, Cursor, or any MCP client

### Who is this for?

- **Security Researchers** — investigate domain ownership and infrastructure.
- **Domain Investors** — monitor expiry dates and check availability.
- **IT Administrators** — audit DNS configurations and shared hosting environments.


## Available Tools
- **check_domain_availability**: Check if a domain is available for registration
- **bulk_whois_lookup**: Returns key registration details for each domain.

WHOIS lookup for multiple domains at once
- **get_domain_contacts**: Note: many domains use privacy protection.

Get registrant and admin contact info for a domain
- **check_domain_age**: Check the age of a domain
- **check_domain_expiry**: Useful for renewal monitoring.

Check when a domain expires
- **lookup_hosted_domains**: Useful for shared hosting analysis.

Find all domains hosted on a specific IP address
- **get_nameservers**: Get nameservers for a domain
- **get_registrar_info**: Get registrar and status info for a domain
- **check_ip2whois_status**: com to confirm valid authentication.

Verify IP2WHOIS API connectivity
- **lookup_domain_whois**: Full WHOIS lookup for a domain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IP2WHOIS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Look up the WHOIS information for github.com."

**🤖 AI Agent:**
> Here's the WHOIS record for github.com: Registered on October 9, 2007 (18+ years old), expires October 9, 2026. Registrar: MarkMonitor Inc. Nameservers: dns1.p08.nsone.net, dns2.p08.nsone.net, and more. The domain status is 'clientDeleteProhibited' (protected).

---

**👤 You:**
> "Check if the domain coolstartup2026.com is available."

**🤖 AI Agent:**
> The domain coolstartup2026.com appears to be available for registration! No WHOIS record was found, which indicates it has not been registered yet.

---

**👤 You:**
> "When does google.com expire?"

**🤖 AI Agent:**
> google.com expires on September 14, 2028. That's approximately 866 days from now — no immediate renewal concern. The registrar is MarkMonitor Inc.


## Installation & Usage

To install and use the **IP2WHOIS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ip2whois](https://vinkius.com/mcp/ip2whois)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

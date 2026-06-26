# SecurityTrails MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/securitytrails)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Uncover IT infrastructure — access DNS history, subdomains, reverse IP lookups, WHOIS data and advanced domain intelligence for ultimate OSINT.

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


## Available Tools (10)
- **get_api_usage**: Check current SecurityTrails API quota usage
- **get_domain_tags**: Get classification tags for a domain
- **get_dns_history**: Useful for finding old IPs that might still be hosting vulnerable software, or tracking infrastructure migration over time.

Retrieve historical DNS records for a domain
- **get_subdomains**: Critical for attack surface mapping and asset discovery. Returns both active and inactive subdomains.

Discover all subdomains for a given domain
- **get_whois**: Get current WHOIS information for a domain
- **search_dsl**: Examples: `ipv4="1.1.1.1" AND mx="alt1.aspmx.l.google.com"` or `whois_email="admin@example.com"`. Check SecurityTrails docs for full DSL syntax.

Advanced search using SecurityTrails DSL
- **get_domains_by_ip**: Essential for understanding shared hosting environments or identifying hidden vhosts.

Find all domains pointed to a specific IP address
- **get_domain_details**: Essential for mapping out a target domain's existing infrastructure.

Get complete domain intelligence and current DNS records
- **get_associated_domains**: Great for expanding the scope of an investigation.

Find other domains associated with a target domain
- **get_whois_history**: Useful for OSINT investigations to uncover historical owners before privacy protection was enabled.

Retrieve historical WHOIS records for a domain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **SecurityTrails** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find all subdomains for tesla.com."

**🤖 AI Agent:**
> I've queried SecurityTrails and found 482 subdomains for tesla.com, including: autodiscover.tesla.com, sso.tesla.com, ir.tesla.com, shop.tesla.com, and energy.tesla.com.

---

**👤 You:**
> "Check the historical 'A' records for example.com. Were there any changes in 2021?"

**🤖 AI Agent:**
> Looking at the DNS history for example.com, the A record currently points to 93.184.216.34. However, back in 2021, the domain pointed to 93.184.216.119 before migrating infrastructure in late 2022.

---

**👤 You:**
> "What domains are hosted on the IP 8.8.8.8?"

**🤖 AI Agent:**
> I performed a reverse IP lookup on 8.8.8.8 (Google Public DNS). As expected for a public resolver, there are millions of historical records pointing here, but currently, domains like dns.google and google-public-dns-a.google.com resolve directly to this IP address.


## ❓ FAQ

**Q: Is the SecurityTrails API free to use?**
SecurityTrails offers a Free Tier API plan which allows 50 API requests per month. This is excellent for specific, targeted OSINT investigations. For automated or large-scale recon, you would need a commercial subscription.

**Q: What is historical DNS good for?**
Companies often migrate infrastructure and hide behind WAFs like Cloudflare. Historical DNS reveals the original origin IP addresses used before the WAF was implemented, which might still be active and vulnerable to direct attacks. It's a critical tool in penetration testing.

**Q: How can I find related domains for a target company?**
Use the `get_associated_domains` tool. It uses proprietary correlation to find other domains owned by the same entity. You can also use `get_domains_by_ip` to find what else is hosted on their IP space.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/securitytrails](https://vinkius.com/mcp/securitytrails)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **SecurityTrails** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `securitytrails` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **SecurityTrails** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "securitytrails": {
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

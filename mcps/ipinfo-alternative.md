# IPinfo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ipinfo-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Enrich IP addresses with geolocation, ASN, and WHOIS data directly from your AI agent using IPinfo's industry-leading intelligence.

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


## Available Tools (10)
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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IPinfo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Lookup the location and carrier details for IP 8.8.8.8."

**🤖 AI Agent:**
> I've retrieved the data for 8.8.8.8 using `get_lookup_ip`. It is located in Mountain View, California, United States. The carrier is Google LLC and it is associated with AS15169.

---

**👤 You:**
> "What domains are currently hosted on the IP 1.1.1.1?"

**🤖 AI Agent:**
> Using `get_hosted_domains`, I found several domains hosted on 1.1.1.1, including 'one.one.one.one', 'cloudflare-dns.com', and 'cloudflare.com'. Would you like to see more results from the next page?

---

**👤 You:**
> "Get the IP ranges for the domain microsoft.com."

**🤖 AI Agent:**
> I've queried `get_ranges` for microsoft.com. I found multiple IP ranges associated with this domain, such as 20.112.52.0/24 and 20.103.85.0/24. These belong to Microsoft Corporation (AS8075).


## ❓ FAQ

**Q: How can I get the most detailed data available for an IP, including WHOIS and company info?**
Use the `get_enterprise_ip` tool. It retrieves the full enterprise dataset, including WHOIS records, company details, abuse contacts, and hosted domains for the target IP.

**Q: Is it possible to check which websites are sharing the same IP address?**
Yes! The `get_hosted_domains` tool performs a Reverse IP lookup, returning a list of domains hosted on the specified IP address.

**Q: Can I process a large list of IP addresses at once?**
Absolutely. Use the `batch_enrich_ips` action to enrich up to 1,000 IP addresses in a single API call, which is much more efficient than individual lookups.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ipinfo-alternative](https://vinkius.com/mcp/ipinfo-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IPinfo** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ipinfo-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IPinfo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ipinfo-alternative": {
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

# IPinfo MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ipinfo)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Geolocate and audit IP addresses — identify ASNs and privacy details via AI.

## Description
Empower your AI agent to orchestrate your entire IP intelligence and network auditing workflow with **IPinfo**, the world's most trusted source for IP data. By connecting IPinfo to your agent, you transform complex network lookups into a natural conversation. Your agent can instantly geolocate IP addresses, audit ASN details, and retrieve privacy metadata without you ever touching a terminal. Whether you are conducting security research or monitoring user traffic, your agent acts as a real-time network analyst, ensuring your intelligence is always grounded in precise, high-fidelity data.

### What you can do

- **IP Auditing** — Query geographic details for any IP address and retrieve city, region, and ISP information instantly.
- **ASN Oversight** — Identify Autonomous System Numbers (ASN) to maintain a clear view of network ownership and routing.
- **Privacy Intelligence** — Check if an IP address is associated with a VPN, proxy, or Tor node to audit traffic authenticity.
- **Network Discovery** — Retrieve metadata for entire IP ranges or CIDR blocks to understand regional allocations.
- **Operational Monitoring** — Query your own server IP details to maintain strict control over your connection environment.

### How it works

1. Subscribe to this server
2. Enter your IPinfo Access Token
3. Start managing your network intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Researchers** — monitor malicious IPs and retrieve threat intelligence metadata straight from your workflow.
- **Data Engineers** — verify user geolocation and audit network routing for optimized performance.
- **Risk Managers** — perform rapid audits of IP privacy settings and identify proxy usage through natural language.
- **Operations Leads** — automate network data querying to orchestrate cross-functional infrastructure teams smoothly.


## Available Tools (6)
- **get_ip_historical**: Get historical data for an IP (Requires appropriate plan)
- **get_ip_range**: Get details for an IP range or CIDR
- **get_own_ip_details**: Get details for the current server IP
- **get_privacy_details**: Check if an IP is using a VPN, proxy, or Tor
- **get_asn_details**: Get details for an Autonomous System Number (ASN)
- **get_ip_details**: Get full geographic and network details for an IP address


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IPinfo** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Geolocate the IP address 1.1.1.1 using IPinfo."

**🤖 AI Agent:**
> I've geolocated the IP! It is located in Research, Victoria, Australia. The provider is identified as Cloudflare. Would you like the full network and ASN details?

---

**👤 You:**
> "Check if IP 8.8.8.8 is using a VPN."

**🤖 AI Agent:**
> I've checked the privacy settings for 8.8.8.8. It is not identified as a VPN, proxy, or Tor exit node. It is a public DNS IP provided by Google. Would you like to see the ASN info?

---

**👤 You:**
> "Show ASN details for AS15169."

**🤖 AI Agent:**
> I've retrieved the details for AS15169. It belongs to Google LLC and has over 15 million IPs allocated. Would you like to see the domains associated with this ASN?


## ❓ FAQ

**Q: How do I find my IPinfo Access Token?**
Log in to your [**IPinfo dashboard**](https://ipinfo.io/account), and you will find your Access Token on the overview page. Copy and paste it below.

**Q: Does the agent detect VPNs and Proxies?**
Yes. The `get_privacy_details` tool allows your agent to identify if an IP address is masked by a VPN, proxy, or Tor network instantly.

**Q: Is ASN information provided for all IPs?**
Yes. IPinfo provides comprehensive ASN metadata for any IP address, helping you audit the network provider and routing hierarchy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ipinfo](https://vinkius.com/mcp/ipinfo)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `ipinfo` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IPinfo** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ipinfo": {
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

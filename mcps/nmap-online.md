# Nmap Online MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nmap-online)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [fort-knox](../categories/fort-knox.md)

Perform network discovery and security auditing via Nmap — track port scans, DNS lookups, and traceroutes directly from your AI agent.

## Description
Connect to high-performance network diagnostic tools through your AI agent and perform essential security auditing and network discovery using natural conversation.

### What you can do

- **Port Scanning** — Perform fast Nmap scans to identify open ports and active services on any IP or domain.
- **DNS Intelligence** — Execute forward and reverse DNS lookups, and discover subdomains for target infrastructures.
- **Ownership & Registration** — Retrieve comprehensive WHOIS information to identify domain ownership and registration details.
- **Geolocation** — Map IP addresses to their physical locations, including country, city, and ISP information.
- **Network Path Analysis** — Run network traceroutes (MTR) and pings to diagnose connectivity and latency issues.
- **Web Diagnostics** — Inspect raw HTTP response headers and extract all links from target web pages.

### How it works

1. Subscribe to this server
2. (Optional) Enter your HackerTarget API Key for higher limits
3. Start auditing your network from Claude, Cursor, or any MCP client

### Who is this for?

- **Security Researchers** — quickly identify the attack surface of a target domain or IP address.
- **Network Administrators** — diagnose connectivity issues and verify DNS configurations without leaving the terminal.
- **DevOps Engineers** — monitor service availability and web server headers through natural language commands.


## Available Tools
- **dns_lookup**: ) for a specific domain.

Forward DNS lookup
- **geoip_lookup**: IP geolocation lookup
- **get_http_headers**: Get HTTP response headers
- **list_subdomains**: Search for subdomains
- **nmap_scan**: Perform a basic Nmap port scan
- **get_page_links**: Extract links from a page
- **ping_host**: Ping a host
- **reverse_dns**: Reverse DNS lookup
- **traceroute**: Perform a network traceroute
- **whois_lookup**: WHOIS lookup


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nmap Online** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Scan the ports for the domain 'example.com'."

**🤖 AI Agent:**
> Running Nmap scan... I've identified several open ports on example.com: Port 80 (http) and Port 443 (https) are active. Would you like to see the HTTP headers for this domain?

---

**👤 You:**
> "Find the physical location of the IP address 8.8.8.8."

**🤖 AI Agent:**
> Performing GeoIP lookup... The IP 8.8.8.8 is located in the United States, specifically in Mountain View, California. It is registered to Google LLC. Shall I perform a WHOIS lookup for more details?

---

**👤 You:**
> "Trace the network path to 'google.com'."

**🤖 AI Agent:**
> Initializing traceroute... I've mapped the path to google.com. It took 8 hops with an average latency of 15ms. No significant packet loss was detected along the route. Would you like to check the DNS records for google.com as well?


## ❓ FAQ

**Q: Is a HackerTarget API Key mandatory?**
No. HackerTarget allows a limited number of free daily scans without a key. For higher volume or commercial use, an API key is required.

**Q: Can I perform an aggressive Nmap scan?**
The `nmap_scan` tool in this server performs a standard service discovery scan. Aggressive flags are limited by the upstream API provider for safety and performance reasons.

**Q: What information does the GeoIP lookup provide?**
The GeoIP tool returns the country, region, city, and the Internet Service Provider (ISP) associated with the target IP address.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nmap-online](https://vinkius.com/mcp/nmap-online)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nmap Online** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nmap-online` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nmap Online** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nmap-online": {
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

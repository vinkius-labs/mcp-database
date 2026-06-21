# Nmap Online MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nmap-online)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nmap-online-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nmap-online-mcp)
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


## Installation & Usage

To install and use the **Nmap Online** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nmap-online](https://vinkius.com/mcp/nmap-online)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

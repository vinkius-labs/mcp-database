# IPGeolocation.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ipgeolocationio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ipgeolocationio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ipgeolocationio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Real-time IP geolocation, security intelligence, and timezone data — identify locations, detect VPNs, and manage timezones directly via AI.

## Description
Empower your AI agent with precise **IP Intelligence**. IPGeolocation.io provides a comprehensive suite of tools to analyze IP addresses, domains, and time-related data instantly.

### What you can do

- **Geolocation Tracking** — Retrieve city, country, ISP, and coordinate data for any IPv4 or IPv6 address using `get_ipgeo`.
- **Security & Threat Intel** — Detect VPNs, proxies, Tor nodes, and calculate threat scores with `get_security` and `bulk_security` to prevent fraud.
- **Timezone Management** — Get local time for any location or convert between timezones with high precision using `get_timezone` and `convert_timezone`.
- **Network Analysis** — Access ASN details, network routes, and abuse contact information via `get_asn` and `get_abuse`.
- **User-Agent Parsing** — Break down complex browser strings into readable device and OS metadata using `get_user_agent`.

### How it works

1. Subscribe to this server
2. Enter your IPGeolocation.io API Key
3. Start querying network and geographical data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Analysts** — quickly vet suspicious IPs and identify proxy usage directly from the chat.
- **Developers** — automate localization and timezone logic without manual API lookups.
- **Data Scientists** — enrich datasets with geographical and network metadata through natural language.


## Available Tools
- **bulk_security**: Bulk IP Security lookup
- **bulk_user_agent**: Bulk parse User-Agent strings
- **convert_timezone**: Convert time between timezones
- **get_abuse**: Get Abuse Contact information
- **get_asn**: Get ASN information
- **get_astronomy**: Get astronomy information
- **get_ip**: Get public IP address of the caller
- **get_ipgeo**: Get IP Geolocation information
- **get_security**: Get IP Security information
- **get_timezone**: Get Timezone information
- **get_user_agent**: Parse User-Agent string


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IPGeolocation.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the geolocation of the IP 8.8.8.8?"

**🤖 AI Agent:**
> I've retrieved the data for 8.8.8.8. It is located in Mountain View, California, United States. The ISP is Google LLC. Would you like to see the full coordinate data?

---

**👤 You:**
> "Check if the IP 185.245.87.12 is a VPN or a known threat."

**🤖 AI Agent:**
> Analyzing security data... The IP 185.245.87.12 is identified as a VPN/Proxy with a threat score of 75. It is originating from a known data center. I recommend caution.

---

**👤 You:**
> "Convert 10:00 AM from 'America/New_York' to 'Europe/London'."

**🤖 AI Agent:**
> Using the timezone conversion tool... 10:00 AM in America/New_York corresponds to 3:00 PM in Europe/London on the same day.


## Installation & Usage

To install and use the **IPGeolocation.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ipgeolocationio](https://vinkius.com/mcp/ipgeolocationio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

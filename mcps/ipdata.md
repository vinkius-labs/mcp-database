# IPdata MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ipdata)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/ipdata-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/ipdata-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Enrich IP addresses with geolocation, ASN, and threat intelligence data directly within your AI agent.

## Description
Connect **IPdata** to your AI agent to instantly analyze IP addresses and Autonomous System Numbers (ASN). Get high-precision geolocation, company data, and security threat profiles through natural conversation.

### What you can do

- **IP Geolocation** — Get city, region, country, and coordinate data for any IPv4 or IPv6 address.
- **Threat Intelligence** — Identify proxies, VPNs, Tor nodes, and known malicious actors in real-time.
- **ASN Insights** — Lookup network ownership, routes, and organizational details for any ASN.
- **Connection Analysis** — Inspect your own current connection details to verify network configurations.

### How it works

1. Subscribe to this server
2. Enter your IPdata API Key
3. Start analyzing network data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Security Analysts** — Quickly triage suspicious IPs and check threat scores without leaving the chat.
- **Developers** — Debug geolocation logic and verify network routing directly from the code editor.
- **Data Engineers** — Enrich datasets with organizational and geographic context using simple prompts.


## Available Tools
- **lookup_asn**: Lookup details for an Autonomous System Number (ASN)
- **lookup_ip**: Lookup details for a specific IP address
- **lookup_own_ip**: Lookup the location and threat profile of the current IP


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IPdata** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Lookup details for IP address 8.8.8.8"

**🤖 AI Agent:**
> I've analyzed IP 8.8.8.8. It is located in Mountain View, United States, and belongs to Google LLC (AS15169). The threat profile indicates it is a known public DNS provider with no malicious flags.

---

**👤 You:**
> "What organization is behind ASN 15169?"

**🤖 AI Agent:**
> ASN 15169 is registered to Google LLC. It operates globally with its primary domain being google.com and manages a vast range of network routes.

---

**👤 You:**
> "Check my current IP's location and threat profile."

**🤖 AI Agent:**
> Your current connection is originating from London, UK, via your local ISP. The threat profile is clean, with no detection of VPN or proxy usage.


## Installation & Usage

To install and use the **IPdata** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ipdata](https://vinkius.com/mcp/ipdata)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

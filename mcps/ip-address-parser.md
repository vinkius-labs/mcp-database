# IP Address Parser MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ip-address-parser)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [loved-by-devs](../categories/loved-by-devs.md)

Validate, parse, and classify any IPv4 or IPv6 address. Detect private vs public ranges, parse CIDR notation, and convert between IPv4 and IPv6. Powered by ipaddr.js — the engine behind Express.js.

## Description
A security agent receives the IP `10.0.14.7` and needs to know: is this a private address? Can it reach the internet? What CIDR block does it belong to? Ask an AI and you'll get a confident but often wrong answer.

This MCP uses ipaddr.js (30M+ weekly downloads) — the exact same library that Express.js, Koa, and Fastify use to parse IP addresses in production. Every classification follows RFC 5735 and RFC 4291.

### The Superpowers

- **Range Classification:** Instantly know if an IP is unicast, private, loopback, multicast, linkLocal, or unspecified — no RFC memorization needed.
- **CIDR Parsing:** Pass `10.0.0.0/8` and get the network address, prefix length, and address kind.
- **Dual Stack:** Full IPv4 and IPv6 support with automatic format detection.
- **IPv4↔IPv6 Conversion:** Convert `192.168.1.1` to its IPv4-mapped IPv6 representation `::ffff:192.168.1.1` and back.


## Available Tools (1)
- **parse_ip_address**: The engine uses ipaddr.js (30M+ downloads) which is the standard IP parsing library used by Express.js and Koa.

Validates and parses IPv4/IPv6 addresses. Supports CIDR notation, range detection, and IPv4↔IPv6 conversion


## 💬 Prompt Examples

Here are some examples of how you can interact with the **IP Address Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Our firewall received a connection from 10.0.14.7. Is this an internal or external IP?"

**🤖 AI Agent:**
> Kind: ipv4 | Range: private | This is an internal RFC 1918 address. Not routable on the public internet.

---

**👤 You:**
> "Parse the VPC subnet 172.31.0.0/16 for our AWS infrastructure documentation."

**🤖 AI Agent:**
> Network: 172.31.0.0 | Prefix: /16 (65,534 hosts) | Kind: ipv4 | Range: private.

---

**👤 You:**
> "Convert our on-prem server 192.168.1.100 to IPv6 format for the dual-stack migration."

**🤖 AI Agent:**
> IPv6 Mapped: ::ffff:192.168.1.100 | Kind: ipv4 | Range: private.


## ❓ FAQ

**Q: How does it know if an IP is private or public?**
It follows the IANA reserved ranges defined in RFC 5735 (IPv4) and RFC 4291 (IPv6). 10.x.x.x, 172.16-31.x.x, and 192.168.x.x are classified as 'private'. 127.x.x.x as 'loopback'. Everything else as 'unicast' (public).

**Q: Can I check if an IP belongs to a specific CIDR range?**
Yes. Pass the CIDR notation like '10.0.0.0/8' and the engine returns the network address, prefix length, and address kind. Parse both the IP and the CIDR to compare.

**Q: Does it work with IPv6 addresses?**
Yes. Full IPv6 support including compressed notation (::1), IPv4-mapped (::ffff:192.168.1.1), and all RFC 4291 scoped addresses.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ip-address-parser](https://vinkius.com/mcp/ip-address-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IP Address Parser** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ip-address-parser` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IP Address Parser** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ip-address-parser": {
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

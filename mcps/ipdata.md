# IPdata MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ipdata)
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


## Available Tools (3)
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


## ❓ FAQ

**Q: Can I check the reputation or threat level of a specific IP address?**
Yes! Use the `lookup_ip` tool. It returns a comprehensive threat profile including flags for VPNs, proxies, Tor exit nodes, and known attackers.

**Q: How do I find information about a network provider using an ASN?**
Simply provide the ASN (e.g., '15169') to the `lookup_asn` tool. The agent will retrieve the organization name, domain, and network routes associated with that number.

**Q: Can I see the details of my own current connection?**
Yes, the `lookup_own_ip` tool allows you to fetch the location and threat profile of the IP address currently making the request.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ipdata](https://vinkius.com/mcp/ipdata)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **IPdata** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ipdata` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **IPdata** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ipdata": {
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

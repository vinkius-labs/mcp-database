# Nokia NSP Network APIs MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/nokia-nsp-network-apis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Nokia Network Services Platform as an MCP: network inventory, nodes, active alarms, topology and device OAM (ping/traceroute) across SR OS / SR Linux networks — official NSP REST APIs with OAuth2 client_credentials.

## Description
**Nokia NSP (Network Services Platform)** — the network management and orchestration platform for Nokia IP/optical networks (SR OS, SR Linux) — as a single MCP server.

### What you can do
- **Inventory** — browse networks and nodes (routers, devices) managed by NSP Inventory & Object Management
- **Fault management** — active alarms with severity, source and probable cause from NSP Network Fault Management
- **Topology** — the network graph (nodes, links, interfaces) for maps and path analysis
- **Device OAM** — run ping/traceroute from managed devices via the NSP OAM service

### Authentication (from the NSP API reference)
1. In NSP User Management, register an **API client** for your organization — you receive a Client ID + Client Secret
2. The MCP mints tokens at `POST https://{nsp-hostname}/oauth2/token` (`grant_type=client_credentials`); NSP tokens are short-lived and are auto-refreshed here
3. Product calls go to `https://{nsp-hostname}/nsp/...`

### Who is this for?
Network operations centres, IP/optical network engineers, NOC automation, capacity planning and AI agents monitoring Nokia-powered transport networks.


## Available Tools (6)
- **get_token_info**: Returns the token type and expiry — the sanity check that hostname and app registration are correct before hitting product APIs.

Mint an NSP OAuth2 token and confirm the client identity
- **get_topology**: Use for drawing maps and path analysis. Requires the Topology product.

Get network topology data (links and nodes) for visualisation
- **list_inventory_networks**: Returns network ids and names; drill into nodes with list_network_nodes.

List networks in the NSP inventory (network management hierarchy)
- **list_network_nodes**: Use network ids from list_inventory_networks.

List nodes (routers, devices) within a network in NSP inventory
- **execute_device_oam**: oam_type: ping/traceroute; target: IP or hostname; source_device: id of the device to run from. Requires the OAM product and device permissions.

Run device OAM operations (ping, traceroute) via NSP OAM
- **list_alarms**: Filter by severity or source via query params supported by your NSP release. The ops centre view.

List active network alarms collected by NSP Network Fault Management


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nokia NSP Network APIs** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me all critical alarms on the network right now"

**🤖 AI Agent:**
> 🌐 **NSP critical alarms**

- CRITICAL | SR-7 router portland-01 | Link down on interface 1/1/c3/1
- CRITICAL | SR-7 router austin-02 | Card failure slot 4

Both sources are SR OS routers. Want the probable cause and timestamp detail, or related maintenance audits?

---

**👤 You:**
> "What routers do we have in the inventory?"

**🤖 AI Agent:**
> 🌐 **NSP inventory**

Networks: Core-Transport-1, Metro-Access-2...
Nodes in Core-Transport-1: SR-14s portland-01 (active), SR-7s austin-02 (active), 7250 IXR rings...

All SR OS / SR Linux devices with admin state and model from NSP IOM. Want topology of a specific network?

---

**👤 You:**
> "Run a traceroute from the Portland router to 10.0.0.1"

**🤖 AI Agent:**
> 🛠️ **OAM traceroute (via NSP)**

Source: portland-01 (SR-7s) → Target: 10.0.0.1

Hops: 10.10.0.2 (0.8ms) → 10.20.0.1 (2.1ms) → 10.0.0.1 (3.4ms, reached)

Full hop list and RTTs in the payload. Want a ping as well, or from another source device?


## ❓ FAQ

**Q: How do I get the Client ID/Secret?**
In NSP User Management (your NSP deployment), register an API client for your organization — it issues a Client ID + Client Secret pair. The MCP exchanges them at POST https://{hostname}/oauth2/token (client_credentials) for short-lived Bearer tokens.

**Q: Does this work with the Nokia Network as Code sandbox?**
No. This MCP targets Nokia NSP deployments (IP/optical network management). The former Nokia 'Network as Code' mobile network API portal (networkascode.nokia.com) has been discontinued — its domain no longer resolves. NSP requires a real NSP deployment and API client registration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/nokia-nsp-network-apis](https://vinkius.com/en/ai-agent-connect/nokia-nsp-network-apis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Nokia NSP Network APIs** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `nokia-nsp-network-apis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Nokia NSP Network APIs** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nokia-nsp-network-apis": {
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

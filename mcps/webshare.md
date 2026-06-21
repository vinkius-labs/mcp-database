# Webshare MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/webshare)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage residential and datacenter proxies, rotation settings, and authorized IPs on Webshare — the fast and affordable proxy network.

## Description
Connect your **Webshare** account to any AI agent and take full control of your proxy infrastructure through natural conversation.

### What you can do

- **Proxy Management** — List all assigned residential and datacenter proxy IPs, including ports, credentials, and health status
- **IP Authorization** — Audit and manage your whitelist of authorized IP addresses to grant proxy access to new servers instantly
- **Rotation Control** — Retrieve current proxy rotation and backbone network settings to ensure your crawlers are configured correctly
- **Real-Time Stats** — Monitor your bandwidth consumption and request success/failure rates directly from your agent
- **Immediate Replacement** — Request instant proxy replacements for flagged or blocked IPs within your account quota
- **Quota Monitoring** — Check your account profile, plan limits, and remaining bandwidth before starting large-scale data tasks
- **High-Speed Export** — Generate temporary tokens to export and download your entire proxy list in a single request

### How it works

1. Subscribe to this server
2. Enter your Webshare API Key
3. Start managing your proxy pool through Claude, Cursor, or any MCP-compatible client

No more manual logging into the Webshare dashboard to whitelist an IP or cycle a proxy. Your AI agent becomes your proxy administrator.

### Who is this for?

- **Data Engineers** — automate proxy management and IP whitelisting for large-scale web scraping pipelines
- **DevOps Professionals** — monitor bandwidth usage and manage proxy infrastructure configurations through chat
- **Market Researchers** — quickly retrieve and update proxy lists for geo-targeted data collection
- **Security Researchers** — audit authorized IPs and cycle proxy endpoints for enhanced anonymity and bypass


## Available Tools
- **authorize_new_ip**: Whitelists a new IP address for proxy access
- **export_proxy_list**: Generates a temporary token to download the entire proxy list in a single request
- **get_account_profile**: Retrieves Webshare user profile, including plan limits and bandwidth quotas
- **get_proxy_configuration**: Retrieves current proxy rotation and backbone network settings
- **get_bandwidth_stats**: Retrieves historical bandwidth and request statistics
- **get_replacement_quota**: Checks the available proxy replacement limits for the current cycle
- **list_authorized_ips**: Lists all IP addresses authorized to use proxies without password authentication
- **list_proxies**: Supports pagination.

Lists all assigned proxy IPs with their ports, credentials, and health status
- **revoke_ip_authorization**: Requires the unique ip_id.

Removes an IP address from the authorized whitelist
- **request_proxy_replacement**: Subject to account quotas.

Requests an immediate replacement for a specific proxy IP


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Webshare** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my active proxies and their health status."

**🤖 AI Agent:**
> I found 10 active proxies in your pool. They are all currently 'HEALTHY'. The top ones are 1.2.3.4 (Port: 8080), 5.6.7.8 (Port: 8080), and 9.10.11.12 (Port: 8080). Would you like to see the credentials for these?

---

**👤 You:**
> "Authorize the IP address 192.168.1.100 for my proxy pool."

**🤖 AI Agent:**
> Success! I have added 192.168.1.100 to your Webshare authorized IP whitelist. This machine can now access your proxies without password authentication.

---

**👤 You:**
> "What are my bandwidth statistics for this month?"

**🤖 AI Agent:**
> You have consumed 45.2 GB of your 100 GB monthly quota. You have approximately 54.8 GB remaining. You've made 1.2 million requests with a 98.5% success rate. Would you like to see a breakdown by day?


## ❓ FAQ

**Q: Can I authorize my current IP address to use proxies via chat?**
Yes. The `authorize_new_ip` tool allows you to immediately whitelist a new IPv4 address in your Webshare account, so you can start using your proxies from that machine without a password.

**Q: How do I replace a proxy that has been blocked by a target website?**
Use the `request_proxy_replacement` tool and provide the unique `proxy_id`. Your agent will instruct Webshare to cycle that specific IP for a new one, subject to your account's replacement quota.

**Q: Can I check how much bandwidth I have left this month?**
Absolutely. The `get_account_profile` tool provides real-time info on your plan limits and remaining bandwidth quota, so you can monitor consumption and avoid interruptions.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/webshare](https://vinkius.com/mcp/webshare)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Webshare** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `webshare` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Webshare** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "webshare": {
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

# AdGuard Home MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/adguard-home)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Manage your AdGuard Home instance — control protection, DNS settings, and filtering rules directly from any AI agent.

## Description
Connect your **AdGuard Home** instance to any AI agent and take full control of your network-wide privacy and security through natural conversation.

### What you can do

- **Server Status** — Monitor server health, active ports, protection states, and version information in real-time.
- **Protection Control** — Toggle global filtering, safe browsing, and parental controls on or off, with optional timed durations.
- **DNS Configuration** — View and update upstream DNS servers, bootstrap settings, and cache parameters (TTL, size, and optimistic caching).
- **Filter Management** — Add new blocklist or allowlist URLs and manage custom user-defined filtering rules.
- **Client Insights** — List and search for persistent or runtime clients, and configure specific security settings for individual devices.
- **Host Auditing** — Instantly check if a specific domain is being filtered or blocked for a particular client.

### How it works

1. Subscribe to this server
2. Enter your AdGuard Home Base URL and credentials (Username/Password)
3. Start managing your network security from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Home Lab Enthusiasts** — monitor and tweak your network-wide ad blocker without opening the web dashboard.
- **Network Administrators** — quickly update upstream DNS providers or check why a specific host is being blocked.
- **Privacy-focused Users** — manage custom filtering rules and client-specific protections through simple voice or text commands.


## Available Tools (23)
- **add_client**: Add a new client
- **add_filter_url**: Add a new filter URL
- **add_rewrite**: Add a DNS rewrite
- **add_static_lease**: Add a DHCP static lease
- **check_host**: Check if a host is filtered
- **configure_tls**: Configure TLS settings
- **get_dhcp_status**: Get DHCP server status
- **get_dns_info**: Get DNS configuration info
- **get_filtering_status**: Get filtering status and lists
- **get_query_log_config**: Get query log configuration
- **get_query_log**: Get DNS query log
- **get_stats**: Get DNS query statistics
- **get_status**: Get AdGuard Home server status
- **get_tls_status**: Get TLS configuration status
- **list_blocked_services**: List all available blocked services
- **list_clients**: List all clients
- **list_rewrites**: List DNS rewrites
- **search_clients**: Search for clients
- **set_dns_config**: Update DNS settings
- **set_protection**: globally.

Enable or disable protection globally
- **set_user_rules**: Set custom user filtering rules
- **update_blocked_services**: Update blocked services schedule
- **update_query_log_config**: Update query log configuration


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AdGuard Home** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current status of my AdGuard Home server?"

**🤖 AI Agent:**
> I've checked your server. AdGuard Home v0.107.43 is currently running. Protection is ENABLED, and the DNS server is listening on port 53.

---

**👤 You:**
> "Disable protection for the next 10 minutes."

**🤖 AI Agent:**
> Global protection has been disabled. I've set a duration of 600,000ms, so it will automatically re-enable in 10 minutes.

---

**👤 You:**
> "Check if 'doubleclick.net' is currently being filtered for client 192.168.1.50."

**🤖 AI Agent:**
> Yes, 'doubleclick.net' is being filtered for that client. It is currently blocked by the 'AdGuard DNS filter' list.


## ❓ FAQ

**Q: Can I check if a specific website is being blocked for a specific client?**
Yes, use the `check_host` tool. Provide the domain name and optionally the client IP to see if it's filtered and which rule is responsible.

**Q: Is it possible to pause the ad-blocking globally for a short period?**
Yes. The `set_protection` tool allows you to disable filtering globally. You can also specify a duration in milliseconds if you want it to re-enable automatically.

**Q: How do I add a new blocklist URL using the AI?**
Simply use the `add_filter_url` action. You'll need to provide a name for the filter, the URL of the list, and specify if it's a whitelist or blocklist.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/adguard-home](https://vinkius.com/mcp/adguard-home)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AdGuard Home** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `adguard-home` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AdGuard Home** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "adguard-home": {
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

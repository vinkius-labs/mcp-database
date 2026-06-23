# MainWP MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/mainwp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [cloud-infrastructure](../categories/cloud-infrastructure.md)

Manage multiple WordPress sites, updates, and security via the MainWP REST API.

## Description
Connect your **MainWP Dashboard** to any AI agent to automate your WordPress network management. This MCP server enables your agent to list child sites, monitor pending updates for core, plugins, and themes, and trigger security scans directly from natural language interfaces.

### What you can do

- **Network Oversight** — List all managed child sites and retrieve real-time status and update counts
- **Update Management** — Query all pending WordPress core, plugin, and theme upgrades across your entire network
- **Automated Sync** — Trigger a global synchronization to fetch the latest data from all connected sites instantly
- **Security Auditing** — Initiate vulnerability scans and malware checks using configured MainWP extensions
- **Inventory Control** — List all plugins and themes installed on any specific child site for auditing
- **One-Click Upgrades** — Execute resource upgrades programmatically to maintain network-wide security

### How it works

1. Subscribe to this server
2. Enter your MainWP Dashboard URL and REST API Bearer Token
3. Ensure 'Pretty Permalinks' are enabled on your WordPress dashboard
4. Start managing your WordPress network from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **WordPress Agency Owners** — Monitor client site health and pending updates via simple natural language commands
- **DevOps Engineers** — Automate the synchronization and security scanning of large WordPress networks
- **Site Administrators** — Quickly audit plugin inventories and execute updates without leaving your dev tools


## Available Tools (8)
- **scan_network_malware**: Trigger a malware scan across the network
- **scan_network_vulnerabilities**: Trigger a vulnerability scan across the network
- **list_site_plugins**: List all plugins installed on a specific site
- **list_child_sites**: List all connected WordPress sites
- **sync_child_sites**: Trigger a synchronization with all child sites
- **get_pending_updates_count**: Get a quick count of all pending updates
- **list_available_updates**: List all pending core, plugin, and theme updates
- **upgrade_site_resource**: Requires a JSON body with details.

Execute an upgrade for a specific plugin or theme


## 💬 Prompt Examples

Here are some examples of how you can interact with the **MainWP** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all connected child sites in MainWP."

**🤖 AI Agent:**
> I've retrieved your sites. You have 12 active child sites, including 'Corporate Blog', 'Client E-shop', and 'Portfolio Site'. Would you like to check for pending updates?

---

**👤 You:**
> "How many pending updates are available across my network?"

**🤖 AI Agent:**
> There are currently 45 updates available: 2 for WordPress core, 35 for plugins, and 8 for themes across your entire network.

---

**👤 You:**
> "Run a vulnerability scan across all sites."

**🤖 AI Agent:**
> I've initiated the network-wide vulnerability scan. MainWP is now checking for known issues in your plugins and themes. I will notify you once the process is complete.


## ❓ FAQ

**Q: Why is the API returning a 404 error?**
You must enable 'Pretty Permalinks' in your WordPress Dashboard (Settings > Permalinks). The REST API will not function with the 'Plain' setting.

**Q: How do I find my API Token?**
In your MainWP Dashboard, navigate to Settings > REST API and create a new API Key with 'Write' permissions. Your token is encrypted at rest and injected securely at runtime.

**Q: Can I update plugins across all sites?**
Yes, the `upgrade_site_resource` tool can target specific resources across the entire network by providing the necessary parameters in the JSON body.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mainwp](https://vinkius.com/mcp/mainwp)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **MainWP** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mainwp` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **MainWP** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mainwp": {
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

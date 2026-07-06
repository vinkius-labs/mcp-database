# Patchstack Security MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/patchstack-security)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Monitor WordPress security via Patchstack — track vulnerabilities, manage site software, and receive alerts directly via AI.

## Description
Connect your AI agent to **Patchstack**, the leading security platform for WordPress and PHP applications. This integration allows you to oversee the security status of all your monitored sites, track known vulnerabilities in plugins and themes, and audit security alerts through natural conversation.

### What you can do

- **Software Oversight** — Get a comprehensive overview of all plugins, themes, and core versions across your monitored sites
- **Threat Intelligence** — Search the massive Patchstack database for known vulnerabilities in specific WordPress components
- **Live Alerts** — Retrieve the latest security alerts and triggered firewall rules to stay ahead of attacks
- **Site Auditing** — List and inspect individual sites to check their security scores and vulnerability counts
- **Auto-Update Management** — Review your settings for automatic security patching of vulnerable components

### How it works

1. Subscribe to this server
2. Enter your **Patchstack User Token** (found in your Patchstack App settings under Integrations)
3. Start managing your WordPress security infrastructure via chat

### Who is this for?

- **WordPress Developers** — quickly audit site security and component vulnerabilities during development
- **Agency Owners** — oversee the security status of dozens of client sites from a single conversation
- **Security Researchers** — query the latest vulnerability data and technical threat details via AI


## Available Tools (9)
- **get_component_vulnerabilities**: Retrieve all known vulnerabilities for a specific component
- **get_latest_alerts**: Retrieve the latest security alerts and triggered rules
- **get_latest_vulnerabilities**: Retrieve the latest vulnerabilities added to the database
- **get_site_software**: Retrieve a list of all software installed on a specific site
- **get_software_overview**: Retrieve a security overview of all software across your sites
- **get_vulnerability_details**: Get detailed information for a specific vulnerability
- **list_sites**: Retrieve a list of all sites monitored by Patchstack
- **search_vulnerabilities**: Search the Patchstack vulnerability database
- **get_autoupdate_settings**: Retrieve settings for automatic updates of vulnerable components


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Patchstack Security** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my monitored sites in Patchstack."

**🤖 AI Agent:**
> Fetching sites... I found 3 sites: 'my-blog.com' (Score: 95), 'online-store.net' (Score: 82), and 'dev-site.io' (Score: 100). Would you like to check the software for any of them?

---

**👤 You:**
> "Search for vulnerabilities in the 'Contact Form 7' plugin."

**🤖 AI Agent:**
> Searching the database... I found 5 recent vulnerabilities for 'Contact Form 7'. The most severe is an 'Arbitrary File Upload' (CVE-2023-XXXXX) fixed in version 5.7.3. I recommend updating all instances immediately.


## ❓ FAQ

**Q: Where do I find my Patchstack User Token?**
Log in to the [**Patchstack App**](https://app.patchstack.com/), navigate to **Account Settings** > **Integrations**, and you will find your unique User Token there.

**Q: Does this tool work with the free Patchstack database?**
Yes, you can search for general vulnerability data. However, retrieving site-specific software overviews and alerts requires a Patchstack account with the appropriate monitoring subscription.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/patchstack-security](https://vinkius.com/mcp/patchstack-security)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Patchstack Security** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `patchstack-security` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Patchstack Security** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "patchstack-security": {
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

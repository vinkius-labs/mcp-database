# WordPress Plugin Auditor MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/wordpress-plugin-auditor)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

This MCP gives your AI agent the ability to securely list and audit all installed plugins on a WordPress site. Perfect for security sweeps, maintenance reports, and identifying outdated or inactive plugins.

## Description
Managing dozens of WordPress sites for clients? Give your AI agent the power to audit their plugin ecosystem without ever giving out full admin passwords or risking manual database edits.

### The Superpowers

- **Security Sweeps:** Ask the AI to "Check if the client has any inactive plugins that should be deleted for security." It will instantly retrieve the list and status of every plugin.
- **Maintenance Reporting:** Automatically generate a monthly report of all active plugins and their versions to send to your clients.
- **Zero-Trust Safety:** This is a purely read-only tool. The AI can list the plugins, but it cannot deactivate, delete, or install new ones. It uses native WordPress Application Passwords for strict scoping.


## Available Tools (1)
- **audit_wordpress_plugins**: It will return the name, version, author, and status (active/inactive) for each plugin. Very useful for security and maintenance checks.

Lists all installed WordPress plugins along with their current status and version


## 💬 Prompt Examples

Here are some examples of how you can interact with the **WordPress Plugin Auditor** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Can you audit my WordPress site and tell me which plugins are currently inactive?"

**🤖 AI Agent:**
> I've audited your site. You have 12 plugins installed, and 2 are currently inactive:

1. Hello Dolly (v1.7.2)
2. Classic Editor (v1.6.3)

I recommend deleting these if you no longer use them to improve security.


## ❓ FAQ

**Q: Can the AI install or delete plugins with this tool?**
No. This MCP only calls the `GET` endpoint for plugins. It cannot modify your site's plugin configuration.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/wordpress-plugin-auditor](https://vinkius.com/mcp/wordpress-plugin-auditor)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **WordPress Plugin Auditor** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wordpress-plugin-auditor` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **WordPress Plugin Auditor** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wordpress-plugin-auditor": {
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

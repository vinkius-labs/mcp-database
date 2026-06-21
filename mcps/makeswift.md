# Makeswift MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/makeswift)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Build stunning Next.js websites with a visual editor that lets marketers update pages without touching code or deployments.

## Description
Connect your **Makeswift** site to any AI agent and simplify your visual building and content management workflows through natural conversation.

### What you can do

- **Site Management** — Retrieve detailed site configuration, hostnames, and localized settings
- **Page Control** — List all pages in your project, check publication status, and retrieve detailed page metadata
- **Version Control** — List historical content snapshots and create new ones programmatically for safe releases
- **Developer Insights** — Query registered React components and URL redirects to understand your project structure

### How it works

1. Subscribe to this server
2. Enter your Makeswift Site API Key from your site settings
3. Start managing your visual experiences from Claude, Cursor, or any MCP-compatible client


## Available Tools (10)
- **create_snapshot**: Create a new content snapshot
- **get_page**: Get details for a specific page
- **get_site_details**: Get current Makeswift site details
- **get_snapshot**: Get details for a specific snapshot
- **list_components**: List registered components
- **list_hostnames**: List site hostnames
- **list_locales**: List configured site locales
- **list_pages**: List all pages in the site
- **list_redirects**: List site redirects
- **list_snapshots**: List content snapshots


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Makeswift** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all pages in my Makeswift project."

**🤖 AI Agent:**
> I've fetched your pages. You have 10 pages, including 'Home' (Published), 'About Us' (Draft), and 'Contact' (Published).

---

**👤 You:**
> "Create a new snapshot called 'Pre-Launch Backup'."

**🤖 AI Agent:**
> Success! The snapshot 'Pre-Launch Backup' (ID: snap_abc123) has been created. Your current site content is now saved as a version.

---

**👤 You:**
> "Show me the site configuration details."

**🤖 AI Agent:**
> Your site 'My Awesome Store' is on the 'Pro' plan. Primary hostname is 'example.com' and you have 2 locales configured (en-US, pt-BR).


## ❓ FAQ

**Q: Can I list all pages in my Makeswift site using my AI agent?**
Yes! Use the `list_pages` tool. It will return a comprehensive list of all pages in your project, including their status and IDs.

**Q: How do I create a new content snapshot programmatically?**
Use the `create_snapshot` action. Provide a descriptive name for the snapshot to trigger a new version save of your current site content.

**Q: Is it possible to check the locales configured for my site?**
Yes, use the `list_locales` tool to retrieve all languages and regional settings defined for your site content.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/makeswift](https://vinkius.com/mcp/makeswift)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Makeswift** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `makeswift` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Makeswift** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "makeswift": {
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

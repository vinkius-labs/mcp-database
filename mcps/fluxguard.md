# Fluxguard MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/fluxguard)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [security-compliance](../categories/security-compliance.md)

Monitor website changes, track visual differences, and receive alerts via AI agents with Fluxguard.

## Description
Connect your **Fluxguard** account to any AI agent to automate website change monitoring and regression testing. Fluxguard provides a comprehensive platform for detecting text, HTML, and visual changes across your monitored pages. This MCP server allows you to manage your monitoring setup and retrieve change alerts directly through natural conversation.

### What you can do

- **Page Monitoring** — Add new URLs for monitoring and organize them into categories.
- **Change Detection** — Retrieve a list of all detected changes and fetch specific details for each change.
- **Manual Crawls** — Manually initiate immediate crawls for your monitored sites.
- **Alert Management** — Access all generated alerts and acknowledge them directly through the agent.
- **Snapshots** — List and retrieve historical snapshots captured for your monitored pages.
- **AI Summaries** — Detected changes can be summarized to understand the significance of every update.

### How it works

1. Subscribe to this server through the Vinkius Marketplace
2. Enter your Fluxguard API Key (obtained from your Organization Settings)
3. Start managing your website monitoring directly from your AI agent


## Available Tools (12)
- **acknowledge_alert**: Mark alert as reviewed
- **add_page**: Add URL for monitoring
- **create_category**: Create a new category
- **get_account**: Get organization attributes
- **get_change**: Get change details
- **get_site**: Get site details
- **initiate_crawl**: Manually trigger a crawl
- **list_alerts**: List monitoring alerts
- **list_categories**: List monitoring categories
- **list_changes**: List detected changes
- **list_sites**: List monitored sites
- **list_snapshots**: List site snapshots


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Fluxguard** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Add the URL 'https://example.com' to my monitoring list."

**🤖 AI Agent:**
> Adding page... 'https://example.com' has been successfully added to your monitoring list.

---

**👤 You:**
> "Show me the most recent changes detected across all sites."

**🤖 AI Agent:**
> Retrieving changes... I found 3 recent changes across your monitored pages.

---

**👤 You:**
> "Initiate an immediate crawl for site ID 'site_123'."

**🤖 AI Agent:**
> Crawl initiated! I've started an immediate crawl for site ID 'site_123'.


## ❓ FAQ

**Q: How do I get an API Key for Fluxguard?**
You can generate an API key in your Fluxguard dashboard under Organization Settings.

**Q: What types of changes can Fluxguard detect?**
Fluxguard detects text, HTML, and visual changes (CSS/layout) across monitored pages.

**Q: Can I manually trigger a check for a site?**
Yes, you can use the 'initiate_crawl' tool to trigger an immediate crawl for any monitored site.

**Q: Can I acknowledge alerts through the agent?**
Yes, use the 'acknowledge_alert' tool to mark an alert as reviewed, removing it from the active list.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/fluxguard](https://vinkius.com/mcp/fluxguard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Fluxguard** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `fluxguard` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Fluxguard** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "fluxguard": {
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

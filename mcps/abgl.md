# AB.GL MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/abgl)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Shorten URLs, track click performance, and manage branded links with real-time analytics for every campaign.

## Description
Connect your **AB.GL** account to any AI agent and manage your entire link shortening and analytics workflow through natural conversation.

### What you can do

- **Create Short Links** — Shorten any URL with an optional custom alias for branded campaigns
- **Link Management** — List, inspect, update, and delete shortened URLs from your account
- **Click Analytics** — View detailed click statistics including referrers, devices, and geographic data for any link
- **Bio Link Pages** — List and inspect bio link pages with blocks and appearance settings
- **Custom Domains** — View all custom domains configured for your short links
- **Account Monitoring** — Verify API connectivity and account status

### How it works

1. Subscribe to this server
2. Enter your **API Key** from your AB.GL account settings
3. Start managing links from Claude, Cursor, or any MCP client

### Who is this for?

- **Marketing Teams** — create branded short links and track campaign performance in real time
- **Content Creators** — manage bio link pages and monitor audience engagement
- **Growth Engineers** — automate link creation for A/B testing and attribution tracking


## Available Tools (10)
- **check_abgl_status**: Verify API connectivity
- **create_short_link**: gl.

Create a short link
- **delete_link**: Delete a short link
- **get_bio_link**: Get bio page details
- **get_link_stats**: Get link analytics
- **get_link**: Get link details
- **list_bio_links**: List bio pages
- **list_domains**: gl short links.

List custom domains
- **list_links**: gl account with click counts and creation dates.

List all short links
- **update_link**: Update a short link


## 💬 Prompt Examples

Here are some examples of how you can interact with the **AB.GL** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Shorten https://example.com/long-campaign-url with alias 'q4sale'."

**🤖 AI Agent:**
> Done! Your short link is https://ab.gl/q4sale (ID: lnk_4921). It redirects to the campaign URL. Would you like to check its analytics later?

---

**👤 You:**
> "Show me click statistics for link lnk_4921."

**🤖 AI Agent:**
> Link lnk_4921 has 1,247 total clicks. Top referrers: LinkedIn (42%), Twitter (31%), Direct (27%). Devices: Mobile 68%, Desktop 32%. Top country: United States (580 clicks).

---

**👤 You:**
> "List all my bio link pages."

**🤖 AI Agent:**
> You have 3 bio pages: 'Marketing Team' (12 links, 3.4k views), 'Product Launch Q4' (8 links, 1.2k views), and 'Personal Portfolio' (5 links, 890 views). Would you like to inspect any of them?


## ❓ FAQ

**Q: Can my AI create branded short links with custom aliases?**
Yes. Use the `create_short_link` tool with the URL and an optional alias parameter. For example, ask your agent to shorten 'example.com/campaign' with alias 'summer24'.

**Q: How do I view click analytics for a specific link?**
Use the `get_link_stats` tool with the link ID. The agent returns total clicks, referrer sources, device breakdown, and geographic distribution.

**Q: Can I manage and delete links through the AI?**
Yes. The `update_link` tool changes the destination URL of an existing link, and `delete_link` permanently removes it from your account. Both require the link ID.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/abgl](https://vinkius.com/mcp/abgl)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **AB.GL** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `abgl` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **AB.GL** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "abgl": {
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

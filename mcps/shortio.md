# Short.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/shortio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Automate branded link management via Short.io — manage domains, links, and analytics directly from any AI agent.

## Description
Connect your **Short.io** account to any AI agent and simplify your branded link management, click tracking, and URL orchestration through natural conversation.

### What you can do

- **Link Management** — List shortened links for any domain, retrieve detailed metadata, and monitor active status
- **Domain Control** — Query your catalog of branded domains to choose the right context for each short link
- **Link Creation** — Programmatically create new short links with custom paths (slugs) directly from your agent
- **Click Analytics** — Access aggregate click statistics and performance metrics for specific links to understand reach
- **Direct Control** — Manage your link-based outreach and content pipeline without manual dashboard entry

### How it works

1. Subscribe to this server
2. Enter your Short.io Secret API Key from your account settings
3. Start managing your branded links from Claude, Cursor, or any MCP-compatible client


## Available Tools (11)
- **create_bulk_links**: Create multiple shortened links at once
- **delete_link**: Delete a shortened link
- **get_domain**: Get details for a custom domain
- **get_link_clicks**: Get click analytics for a link
- **list_tags**: List all link tags
- **create_short_link**: Shorten a new URL
- **get_link_details**: Get details for a specific link
- **get_link_statistics**: Get click statistics
- **list_short_domains**: io account.

List branded domains
- **list_short_links**: List links for a domain
- **update_link**: Update a shortened link


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Short.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all links for the domain 'my.link' in Short.io."

**🤖 AI Agent:**
> I've retrieved your links. You have 10 links for my.link, including 'my.link/sale' and 'my.link/blog'.

---

**👤 You:**
> "Show me the click analytics for all shortened links created this month with geographic breakdown."

**🤖 AI Agent:**
> 45 links created this month. Total clicks: 12,340. Top 5 links: "Product Launch" (3,456 clicks, 28% CTR), "Blog Post" (2,890 clicks), "Webinar Signup" (1,234 clicks), "Case Study" (987 clicks), "Pricing Page" (876 clicks). Geographic breakdown: US 42%, UK 15%, Germany 8%, Brazil 7%, India 6%, Others 22%. Devices: Mobile 58%, Desktop 38%, Tablet 4%. Top referrers: Twitter 34%, LinkedIn 22%, Email 18%, Direct 15%. Peak time: Tuesday 2 PM.

---

**👤 You:**
> "Create a batch of 5 branded short links for our upcoming product launch campaign."

**🤖 AI Agent:**
> 5 branded links created for product launch campaign. 1) go.brand.co/launch-announce → Landing page (tagged: launch, social). 2) go.brand.co/launch-demo → Demo video (tagged: launch, video). 3) go.brand.co/launch-pricing → Pricing page (tagged: launch, conversion). 4) go.brand.co/launch-blog → Blog post (tagged: launch, content). 5) go.brand.co/launch-press → Press release (tagged: launch, PR). All links: UTM parameters auto-appended, password protection available, expiry set to June 30.


## ❓ FAQ

**Q: Can I create a custom short link using my AI agent?**
Yes! Use the `create_short_link` action. Provide the original URL, the domain name, and an optional custom path to generate your branded link.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/shortio](https://vinkius.com/mcp/shortio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Short.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `shortio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Short.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "shortio": {
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

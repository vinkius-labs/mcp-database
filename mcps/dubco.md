# Dub.co MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/dubco)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Manage your short links via Dub.co — create, track, and analyze your link performance directly from any AI agent.

## Description
Connect your AI agent to **Dub.co** (formerly Dub.sh), the modern link management platform for marketing teams. This integration allows you to generate short links, oversee your workspaces, and retrieve deep performance analytics through natural conversation.

### What you can do

- **Link Creation** — Instantly generate short links for any destination URL with custom slugs and domains
- **Deep Analytics** — Retrieve click data, lead tracking, and geographic breakdowns (countries, cities, devices)
- **Workspace Management** — List and switch between different workspaces and domains associated with your account
- **Organization** — Use tags to categorize your links and filter them efficiently
- **Social Metadata** — Inspect metatags (Open Graph) for any URL before or after link creation

### How it works

1. Subscribe to this server
2. Enter your **Dub.co API Key** (found in your Dub.co account settings)
3. Start managing and analyzing your marketing links via chat

### Who is this for?

- **Marketing Teams** — quickly generate campaign links and check performance without leaving the chat
- **Content Creators** — track audience engagement across different platforms using short links
- **Product Managers** — audit link routing and analyze user flow via geographic data


## Available Tools
- **create_short_link**: Create a new short link
- **delete_short_link**: Permanently delete a short link
- **get_workspace_analytics**: Retrieve aggregate analytics for the authenticated workspace
- **get_link_details**: Retrieve detailed information for a specific short link
- **get_url_metatags**: Retrieve Open Graph metatags for a specific URL
- **list_domains**: Retrieve a list of all domains in the current workspace
- **list_links**: Retrieve a list of short links for the authenticated workspace
- **list_tags**: Retrieve a list of all tags in the current workspace
- **list_workspaces**: Retrieve a list of all workspaces the user has access to
- **update_short_link**: Update an existing short link


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dub.co** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a short link for 'https://vinkius.com' using the slug 'vinkius-home'."

**🤖 AI Agent:**
> Link created! Your short URL is `dub.sh/vinkius-home`. It points to `https://vinkius.com`.

---

**👤 You:**
> "Show me the click analytics for my workspace."

**🤖 AI Agent:**
> Retrieving analytics... Total clicks in the last period: 1,240. Most traffic is coming from the United States (45%) and Brazil (20%).


## ❓ FAQ

**Q: Where do I find my Dub.co API Key?**
Log in to your [**Dub.co Dashboard**](https://app.dub.co/), navigate to your account settings, and you will find the API section where you can create and copy your access token.

**Q: Do I need a Pro plan for analytics?**
While basic link creation works on free tiers, some advanced aggregate analytics and geographic filtering may require a Dub.co Pro plan or higher as per their API policy.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dubco](https://vinkius.com/mcp/dubco)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dub.co** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `dubco` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dub.co** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dubco": {
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

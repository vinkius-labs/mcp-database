# ChangeDetection.io MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/changedetectionio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-management](../categories/data-management.md)

Monitor website changes automatically — track visual or text updates, manage watches, and receive alerts via any AI agent.

## Description
Connect your **ChangeDetection.io** instance to any AI agent to automate web monitoring and data extraction through natural conversation.

### What you can do

- **Watch Management** — Create, update, and delete monitors for any URL to track content changes
- **Snapshot Analysis** — Retrieve historical snapshots and compare differences (diffs) to see exactly what changed
- **Tagging & Organization** — Categorize your watches with tags to manage large-scale monitoring projects
- **Instant Rechecks** — Trigger immediate checks for specific watches to get the most up-to-date information
- **History Tracking** — Access the full history of a watch to analyze trends and previous versions of a page

### How it works

1. Subscribe to this server
2. Enter your ChangeDetection.io Instance URL and API Key
3. Start monitoring the web from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — track price changes, availability, or content updates across multiple competitors automatically
- **Developers** — monitor API documentation or website changes to stay ahead of breaking updates
- **SEO Specialists** — keep an eye on SERP changes or competitor landing page modifications


## Available Tools (14)
- **create_tag**: Create a new tag
- **create_watch**: Create a new watch
- **delete_watch**: Delete a watch
- **get_snapshot_diff**: Use "previous" and "latest" as keywords.

Get snapshot difference (diff)
- **get_snapshot**: Use "latest" for the most recent check.

Get single snapshot
- **get_tag**: Get single tag
- **get_watch_favicon**: Get watch favicon
- **get_watch_history**: Get watch history
- **get_watch**: Get single watch
- **import_urls**: io.

Import API
- **list_tags**: List all tags
- **list_watches**: List all watches
- **search_watches**: Search API
- **update_watch**: Update an existing watch


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ChangeDetection.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all my active web watches."

**🤖 AI Agent:**
> I've retrieved your watches. You have 3 active monitors: 'Competitor Pricing' (UUID: 550e8400), 'API Docs' (UUID: 123e4567), and 'Stock Alert' (UUID: 890b1234).

---

**👤 You:**
> "Create a new watch for https://example.com with the title 'Example Monitor'."

**🤖 AI Agent:**
> Successfully created the watch for https://example.com. It has been assigned UUID: 771f9211. I will start tracking changes for you now.

---

**👤 You:**
> "Show me the difference between the last snapshots for watch 550e8400."

**🤖 AI Agent:**
> Comparing snapshots for 'Competitor Pricing'... I found that the price text changed from '$49.99' to '$39.99' and a new 'On Sale' badge was added to the header.


## ❓ FAQ

**Q: Can I see exactly what text changed on a page between the last two checks?**
Yes! Use the `get_snapshot_diff` tool with the watch UUID. It will return the specific differences between the current state and the previous snapshot.

**Q: How do I trigger an immediate recheck of a specific website?**
You can use the `get_watch` tool and set the `recheck` parameter to '1'. This forces the server to fetch the latest version of the page immediately.

**Q: Can I filter my monitors by tags using the AI?**
Absolutely. When using `list_watches`, you can provide a `tag` name to filter the results and only see monitors associated with that specific category.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/changedetectionio](https://vinkius.com/mcp/changedetectionio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **ChangeDetection.io** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `changedetectionio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **ChangeDetection.io** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "changedetectionio": {
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

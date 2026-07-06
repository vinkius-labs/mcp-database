# Meltwater MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/meltwater)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Media intelligence and social monitoring via Meltwater — track news, mentions, and analytics.

## Description
Connect your **Meltwater** account to any AI agent and take full control of your media intelligence and social monitoring through natural conversation.

### What you can do

- **Content Search** — Perform keyword searches across news and social media streams in real-time
- **Social Monitoring** — Retrieve detailed metadata, sentiment, and reach for specific mentions
- **Analytics & Reporting** — Access aggregated performance metrics and AI-driven insights for your searches
- **Organization** — Manage tags, folders, and saved searches to streamline your monitoring workflow
- **Data Connectivity** — List media sources and available content exports directly from your agent

### How it works

1. Subscribe to this server
2. Enter your Meltwater API Key, Client ID, and Client Secret
3. Start monitoring your brand from Claude, Cursor, or any MCP-compatible client


## Available Tools (10)
- **get_search_details**: Get details for a saved search
- **list_content_exports**: List available content exports
- **list_folders**: List all account folders
- **list_saved_searches**: List all saved searches
- **list_media_sources**: List tracked media sources
- **list_tags**: List all organizational tags
- **search_content**: Search news and social media content
- **get_search_analytics**: Get analytics for a search
- **get_media_insights**: Get high-level media insights
- **get_mention_details**: Get details for a specific mention


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meltwater** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for recent news about 'Artificial Intelligence'."

**🤖 AI Agent:**
> Retrieving news... I found 10 recent articles covering AI breakthroughs and policy changes.

---

**👤 You:**
> "What is the sentiment for my brand search ID 123?"

**🤖 AI Agent:**
> Analyzing sentiment... Your brand sentiment for search 123 is currently 75% positive, with a notable increase in neutral mentions.

---

**👤 You:**
> "List all saved searches in my Meltwater account."

**🤖 AI Agent:**
> Querying searches... You have 5 saved searches including 'Competitor Tracking' and 'Local News Monitor'.


## ❓ FAQ

**Q: How do I get Meltwater API credentials?**
You need to log in to the Meltwater Developer Portal to generate your API Key and create an application to receive your OAuth 2.0 Client ID and Secret.

**Q: What content can I search?**
Meltwater allows you to search across millions of global news sources and various social media platforms like Twitter, Instagram, and Facebook.

**Q: Is my media data secure?**
Absolutely. Your credentials are encrypted at rest and injected securely at runtime.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meltwater](https://vinkius.com/mcp/meltwater)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Meltwater** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `meltwater` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Meltwater** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meltwater": {
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

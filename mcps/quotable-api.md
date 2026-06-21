# Quotable API MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/quotable-api)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Access thousands of quotes — audit authors and tags via AI.

## Description
Empower your AI agent to orchestrate your entire literary research and quote auditing workflow with the **Quotable API**, the comprehensive source for inspirational and famous quotes. By connecting Quotable to your agent, you transform complex keyword searches into a natural conversation. Your agent can instantly retrieve random quotes, audit author biographies, and query specific tags without you ever touching a quote portal. Whether you are building social media content or conducting thematic research, your agent acts as a real-time literary consultant, ensuring your data is always verified and precise.

### What you can do

- **Quote Auditing** — Retrieve random or specific quotes by keyword and maintain a clear view of content, author, and tag distribution.
- **Author Oversight** — Audit comprehensive author profiles, including biographies and descriptions, to understand the source of literary data.
- **Tag Discovery** — Browse available quote tags to identify relevant themes such as 'technology', 'wisdom', or 'famous-quotes' instantly.
- **Metadata Intelligence** — Retrieve unique author slugs and quote identifiers to assist in deep-dive archival classification.
- **Literary Monitoring** — Check API status to ensure your quote research workflow is always operational.

### How it works

1. Subscribe to this server
2. No API Key required (Quotable is a free and open service)
3. Start managing your literary intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — monitor quote trends and retrieve inspirational metadata straight from your workflow.
- **Writers & Researchers** — verify author details and audit thematic patterns without manual searching.
- **Social Media Managers** — perform rapid audits of quote tags and identify relevant content markers through natural language.
- **Operations Leads** — automate literary data querying to orchestrate cross-functional creative teams smoothly.


## Available Tools
- **check_api_status**: Check if the Quotable API service is operational
- **get_author_details**: Get full details and biography for a specific author by slug
- **get_random_quote**: Get a random quote with optional tag or author filters
- **list_quote_authors**: List all authors in the database with their descriptions
- **list_quote_tags**: List all available quote tags and their quote counts
- **search_quotes**: Search for quotes by keyword or phrase


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Quotable API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get a random quote about 'wisdom' using Quotable."

**🤖 AI Agent:**
> I've retrieved a random quote about wisdom! It's by [Author]: "[Quote content]". Would you like the author's biography or other quotes with this tag?

---

**👤 You:**
> "Search for quotes by 'Albert Einstein'."

**🤖 AI Agent:**
> I've identified 10 quotes by Albert Einstein. Notable entries include his thoughts on imagination and logic. I can provide the full details and tags for each of these quotes if you'd like.

---

**👤 You:**
> "List all available quote tags."

**🤖 AI Agent:**
> I've scanned the tag catalog. There are over 50 tags available, including 'technology', 'success', 'love', and 'life'. I can help you retrieve a random quote for any of these specific themes.


## ❓ FAQ

**Q: Is an API Key required for Quotable API?**
No. Quotable.io is a free and open service. This server works out of the box without any static credentials required.

**Q: Can I filter quotes by author?**
Yes. Use the `get_random_quote` tool and provide the `author` parameter (name or slug). Your agent will return matching quotes instantly.

**Q: What biographical data is provided for authors?**
The `get_author_details` tool provides the author's full name, a brief description, and a complete biography from the database.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/quotable-api](https://vinkius.com/mcp/quotable-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Quotable API** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `quotable-api` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Quotable API** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "quotable-api": {
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

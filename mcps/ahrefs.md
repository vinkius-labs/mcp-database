# Ahrefs MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ahrefs)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [growth-engine](../categories/growth-engine.md)

Professional SEO intelligence — audit backlinks, keywords, and domain health via AI.

## Description
Connect your **Ahrefs** account to your AI agent to unlock the world's most powerful SEO data platform. From auditing domain ratings and backlink profiles to researching keyword difficulty and monitoring SERP rankings, your agent handles your organic growth strategy through natural conversation.

### What you can do

- **Site Explorer** — List and audit backlinks, broken links, and referring domains for any website
- **Keyword Research** — Retrieve keyword metrics (volume, difficulty, CPC) and generate related keyword ideas
- **Organic Traffic Auditing** — List top-performing pages and the organic keywords a domain ranks for
- **SERP Analysis** — Retrieve real-time search results for any keyword across different countries
- **SEO Health Monitoring** — Quickly retrieve Domain Rating (DR) and Ahrefs Rank to monitor authority trends

### How it works

1. Subscribe to this server
2. Enter your Ahrefs API v3 Token
3. Start optimizing your SEO and researching competitors through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **SEO Specialists** — automate backlink audits and keyword research workflows effortlessly
- **Content Marketers** — identify top-performing content and relevant topics for your niche
- **Digital Strategists** — monitor competitor authority and organic traffic trends via chat
- **Marketing Agencies** — retrieve granular SEO data for client reports and performance tracking


## Available Tools (10)
- **get_domain_overview**: Get domain SEO metrics
- **list_backlinks**: List website backlinks
- **list_organic_keywords**: List ranking keywords
- **get_backlinks_stats**: Get backlink summary
- **list_broken_backlinks**: Identify 404 broken links
- **list_top_pages**: List top performing pages
- **get_keyword_overview**: Get keyword metrics
- **list_keyword_ideas**: Generate keyword ideas
- **get_keyword_volume_history**: Get historical search volume
- **get_serp_overview**: Analyze search results


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Ahrefs** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the domain overview for 'ahrefs.com'."

**🤖 AI Agent:**
> I've retrieved the domain overview for ahrefs.com. The Domain Rating (DR) is 90, and it currently ranks for over 1.5 million organic keywords. Total backlinks are approximately 25 million.

---

**👤 You:**
> "List 10 backlinks for 'example.com' with the highest Domain Rating."

**🤖 AI Agent:**
> I've retrieved the top 10 backlinks for example.com. The strongest links come from high-authority domains like wikipedia.org (DR 91) and nytimes.com (DR 94). Would you like to see the anchor texts for these links?

---

**👤 You:**
> "Check keyword metrics for 'best SEO tools' in the US."

**🤖 AI Agent:**
> I've analyzed 'best SEO tools' for the US market. The monthly search volume is 12,000, with a difficulty score of 65 (Hard). The estimated CPC is $5.50. Would you like some related keyword ideas?


## ❓ FAQ

**Q: How do I find my Ahrefs API v3 Token?**
Log in to Ahrefs as a workspace owner or admin, navigate to **Account settings** > **API keys**, and create a new key. Note that API v3 is the current standard; v2 is deprecated.

**Q: Does this integration consume Ahrefs API units?**
Yes! Ahrefs uses a unit-based system. Every request costs at least 50 units, and the total cost depends on the number of rows and fields retrieved.

**Q: Can I analyze competitor domains?**
Absolutely. You can provide any domain or URL to the Site Explorer tools to retrieve their backlink profiles, Domain Rating, and organic traffic data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ahrefs](https://vinkius.com/mcp/ahrefs)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Ahrefs** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ahrefs` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Ahrefs** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ahrefs": {
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

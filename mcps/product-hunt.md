# Product Hunt MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/product-hunt)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [social-network](../categories/social-network.md)

Discover the best new products in tech daily — check the leaderboard, search for specific tools, and get detailed product insights via your AI agent.

## Description
Connect your **Product Hunt** account to any AI agent and track the latest startups, tools, and tech trends without leaving your workspace.

### What you can do

- **Daily Leaderboard** — Fetch the top upvoted products trending right now, complete with their taglines and URLs
- **Search Products** — Search the Product Hunt database for specific tools or explore categories (e.g., "AI", "developer tools", "newsletters")
- **Product Deep Dives** — Retrieve detailed information on any product including full descriptions, upvote counts, review scores, maker profiles, and direct website links

### How it works

1. Subscribe to this server
2. Enter your Product Hunt Developer Token
3. Start discovering the newest startups directly from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Founders & Indie Hackers** — monitor the competition and track daily launches in your specific niche
- **Venture Capitalists** — discover trending startups and get instant briefs on products gaining traction
- **Developers & Designers** — discover new tools, open-source projects, and design inspiration while you code


## Available Tools (3)
- **product_details**: You can get the product ID from the leaderboard or search results.

Retrieves detailed information about a specific product by its ID
- **daily_leaderboard**: It returns a list of products with their taglines, vote counts, and URLs.

Fetches the current daily leaderboard of products from Product Hunt
- **search_products**: g., "AI", "productivity", "marketing").

Searches for products on Product Hunt by keyword or name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Product Hunt** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me the top 5 products currently leading the Product Hunt daily leaderboard."

**🤖 AI Agent:**
> Here are the top 5 trending products for today:
1. ACME AI — The ultimate AI agent builder (1.2k upvotes)
2. WidgetX — Create widgets seamlessly (950 upvotes)
3. SuperMail — Re-imagining your inbox (720 upvotes)
Would you like me to fetch a deep dive description on any of these?

---

**👤 You:**
> "Search Product Hunt for new coding tools."

**🤖 AI Agent:**
> I searched for 'coding tools' and found 10 highly upvoted tools. Top results include CodeBolt (coding assistant) with 1200 upvotes, and TermX (cloud terminal) with 850 upvotes. Shall I detail their features?

---

**👤 You:**
> "Pull the detailed info and maker list for the second product on the leaderboard."

**🤖 AI Agent:**
> I've fetched the details for WidgetX: It's an open-source cross-platform UI builder. It has an average review of 4.9, 950 upvotes, and its direct URL is `widgetx.io`. The listed makers are John Doe and Sarah Lee.


## ❓ FAQ

**Q: How do I get started?**
Subscribe, enter your API credentials (your Developer Token from the **Product Hunt API Dashboard**), and you're ready. No code, no setup, no webhooks — just connect and start exploring daily startup launches through your AI agent.

**Q: Can my AI agent create a summary brief of the top 3 startups launched today?**
Yes. Ask your agent to fetch the daily leaderboard and pull the details of the top 3 items. It will return the product names, descriptions, upvote counts, maker names, and direct URLs — generating a complete morning brief on the tech ecosystem without opening a single browser tab.

**Q: What happens when I need to find the best AI tools launched recently?**
Just tell your AI agent. It uses the search tool to query "AI" directly against the Product Hunt database, surfacing highly-rated matches with their taglines and upvotes instantly. You skip the doom-scrolling and go straight to evaluating the exact tools you are looking for.

**Q: Is this suitable for VC scouting workflows and competitive analysis?**
Absolutely. Because your agent can pull deeply nested product details (including maker names, review scores, and direct website links) for any product ID, you get a comprehensive pulse on fresh competitors or investment opportunities immediately. Perfect for scouting teams building automated deal-flow monitors.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/product-hunt](https://vinkius.com/mcp/product-hunt)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Product Hunt** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `product-hunt` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Product Hunt** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "product-hunt": {
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

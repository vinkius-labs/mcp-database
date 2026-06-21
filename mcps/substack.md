# Substack MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/substack)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent with direct access to Substack — manage publications, draft posts, and track subscriber data without opening the Substack editor.

## Description
Connect **Substack** to your AI agent and manage your newsletter publication conversationally.

### What you can do

- **Post Management** — List, create, and manage newsletter posts including drafts, published, and scheduled content.
- **Subscriber Insights** — Query subscriber counts, growth trends, and audience demographics.
- **Publication Settings** — Access and modify publication metadata, categories, and custom domains.
- **Content Analytics** — Track open rates, click rates, and engagement metrics per post.

### How it works

1. Subscribe to the Substack integration on the marketplace.
2. Get your API token from your Substack publication settings (Settings → Publication API).
3. Ask your AI agent to draft posts, check analytics, or manage subscribers.

### Who is this for?

- **Newsletter Creators** — Draft and schedule posts without switching context to the Substack editor.
- **Content Marketers** — Track newsletter performance and audience growth from a conversational interface.
- **Thought Leaders** — Manage multiple Substack publications efficiently from your AI workflow.


## Available Tools
- **list_posts**: List recent posts
- **get_post**: Get post
- **get_post_stats**: Get post stats
- **list_subscribers**: List subscribers
- **get_publication_info**: Get publication info
- **get_leaderboard**: Get leaderboard


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Substack** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How many subscribers does my Substack have?"

**🤖 AI Agent:**
> Your publication has 4,250 total subscribers. Breakdown: 3,890 free (91.5%) and 360 paid (8.5%). Growth this month: +185 new subscribers (4.5% growth rate). Churn: 12 unsubscribes.

---

**👤 You:**
> "Draft a new newsletter post titled 'The Future of AI in Sales'."

**🤖 AI Agent:**
> Draft created: 'The Future of AI in Sales'. Status: Draft (unpublished). You can ask me to add body content, set a subtitle, or schedule it for publication.

---

**👤 You:**
> "What was the open rate on my last newsletter?"

**🤖 AI Agent:**
> Your last newsletter 'Q1 Market Insights' had a 52% open rate (2,210 opens out of 4,250 sent), 8% click rate on embedded links, and generated 23 new subscribers from shares.


## ❓ FAQ

**Q: How do I get my Substack API token?**
Log in to your Substack publication at **yourdomain.substack.com**. Navigate to **Settings** from the left sidebar. Look for the **Publication API** or **Developer** section. Generate an API token and copy it. Paste it into the configuration field below. Note: Substack's API is currently in limited availability — check Substack's developer page for the latest access information.

**Q: Can I draft and schedule newsletter posts?**
Yes. Your AI agent can create draft posts with title, body content, subtitle, and metadata. You can then schedule them for a specific date and time — managing your entire editorial calendar conversationally.

**Q: Can I track how many subscribers I gained this month?**
Yes. Ask your AI agent for subscriber growth metrics and get total subscribers, new subscribers this month, churn rate, and free vs. paid subscriber breakdown.

**Q: Does this work with paid Substack publications?**
Yes. The integration supports both free and paid publications. You can manage paywalled content, check paid subscriber counts, and analyze revenue metrics through your AI agent.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/substack](https://vinkius.com/mcp/substack)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Substack** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `substack` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Substack** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "substack": {
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

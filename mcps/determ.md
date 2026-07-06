# Determ MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/determ)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [marketing-automation](../categories/marketing-automation.md)

Equip your AI agent to monitor media mentions, track keywords, and analyze sentiment via the Determ (formerly Mediatoolkit) API.

## Description
Integrate **Determ** (formerly **Mediatoolkit**), the powerful media monitoring and social listening platform, directly into your AI workflow. Track brand mentions across the web and social media, analyze sentiment trends, and monitor your competitive landscape using natural language.

### What you can do

- **Mention Monitoring** — List and retrieve real-time media mentions for your keywords and topics from over 100 million sources.
- **Sentiment Intelligence** — Retrieve a breakdown of sentiment (positive, neutral, negative) for any of your monitoring queries.
- **Query Management** — List and review your configured monitoring queries and their specific settings.
- **Analytics Reporting** — Access metadata for your media monitoring and analytics reports directly via chat.

### How it works

1. Connect the Determ integration to your AI assistant.
2. Authorize using your Determ API Key (found in your settings).
3. Orchestrate your brand monitoring and reputation management through intuitive conversation.

### Who is this for?

- **PR & Communications Managers** — Quickly check recent mentions and brand sentiment on the go.
- **Marketing Teams** — Monitor campaign reach and identify top media sources via chat.
- **Social Media Specialists** — Track social listening queries and mention details during planning sessions.


## Available Tools (10)
- **get_account_metadata**: Retrieve settings and limits for your Determ account
- **get_mention_details**: Get full content and technical metadata for a specific media mention
- **get_monitoring_query_details**: Get detailed settings and status for a specific monitoring query
- **get_query_sentiment_summary**: Retrieve a breakdown of sentiment (positive, neutral, negative) for a specific query
- **list_media_mentions**: List recent media mentions for a specific monitoring query
- **list_monitoring_queries**: List all media monitoring queries (keywords/topics) in your Determ account
- **list_recent_high_reach_mentions**: List only the mentions with the highest estimated reach
- **list_analytics_reports**: List all available analytics and media monitoring reports
- **list_top_media_sources**: Identify the media sources with the highest volume of mentions (mock logic)
- **search_mentions_by_keyword**: Search for specific keywords within the mentions of a monitoring query


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Determ** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List my active monitoring queries."

**🤖 AI Agent:**
> I've found 4 active queries in your account: 'My Brand', 'Main Competitor', 'Industry Trends', and 'Product Feedback'. Would you like to see the latest mentions for 'My Brand'?

---

**👤 You:**
> "Show me the sentiment breakdown for the 'Main Competitor' query."

**🤖 AI Agent:**
> The sentiment for 'Main Competitor' over the last 7 days is 15% Positive, 55% Neutral, and 30% Negative. Negative sentiment has increased by 5% compared to last week. Should I list the negative mentions?

---

**👤 You:**
> "What are the top media sources for 'Industry Trends'?"

**🤖 AI Agent:**
> The top 3 media sources for 'Industry Trends' are 'TechCrunch' (12 mentions), 'The Verge' (8 mentions), and 'Twitter' (45 posts). Would you like to see the most recent article from 'TechCrunch'?


## ❓ FAQ

**Q: How do I get a Determ API Key?**
Log in to your Determ account, navigate to **Settings > API**, and you can retrieve your unique API Key from that section.

**Q: Can the agent show the full text of an article?**
Yes, you can use the get_mention_details tool to retrieve the full content and metadata for a specific mention found by Determ.

**Q: Is real-time monitoring supported?**
Yes, the list_media_mentions tool retrieves the most recent mentions based on your query settings, providing real-time data from the Determ platform.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/determ](https://vinkius.com/mcp/determ)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Determ** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `determ` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Determ** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "determ": {
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

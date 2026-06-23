# New York Times MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/new-york-times)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access top stories, article search, best-seller lists, and movie reviews via the NYTimes API.

## Description
Connect the **New York Times** API to any AI agent and unlock access to over 170 years of journalism — including breaking news, historical archives, best-seller lists, and cultural reviews.

### What you can do
- **Top Stories** — Get the latest top stories for any section (World, Politics, Tech, Sports, etc.)
- **Article Search** — Search the complete archive from 1851 to the present day with keywords and date filters
- **Most Popular** — See what readers are emailing, sharing, and viewing the most
- **Best-Seller Lists** — Retrieve current and historical book best-seller lists
- **Movie Reviews** — Access thousands of movie reviews and critic summaries
- **Section Discovery** — List all available sections and topics covered by the NYTimes

### How it works
1. Subscribe to this server
2. Enter your NYTimes Developer API Key
3. Start exploring world-class journalism from Claude, Cursor, or any MCP-compatible client

The NYTimes API is free for development use, providing a generous limit of requests per day.

### Who is this for?
- **Researchers & Historians** — Track how events were reported over decades using the extensive archive
- **Journalists & Writers** — Find background context and related coverage for current events
- **Book Lovers** — Check weekly best-seller lists and discover trending authors
- **Cinephiles** — Explore the Paper of Record's vast collection of film criticism


## Available Tools (9)
- **get_archive**: Get all articles for a specific month
- **get_book_lists**: "list_name_encoded" is the list slug (e.g., "hardcover-fiction"). Optional date is YYYY-MM-DD.

Get current or historical best-seller lists
- **get_most_emailed**: Period can be 1, 7, or 30 days.

Get the most emailed articles for a specific period
- **get_most_shared**: Period can be 1, 7, or 30 days.

Get the most shared articles on social media
- **get_most_viewed**: Get the most viewed articles
- **get_movie_reviews**: Optional "query" filters by movie title.

Search for movie reviews in the NYTimes archive
- **search_articles**: Use "q" for keywords, "begin_date" and "end_date" for date ranges (YYYYMMDD), and "sort" for "newest", "oldest", or "relevance".

Search for articles using keywords, date ranges, and sorting
- **get_sections**: List all available news sections
- **get_top_stories**: g., home, world, politics, technology, sports). Use get_sections to see available options.

Get top stories for a specific section


## 💬 Prompt Examples

Here are some examples of how you can interact with the **New York Times** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me today's top world news."

**🤖 AI Agent:**
> Top World Headlines: 1. Global Summit Reaches Climate Deal. 2. Elections in Europe Shift Political Landscape. 3. Tech Giants Face New Regulations in Asia.

---

**👤 You:**
> "What is the #1 Hardcover Fiction book this week?"

**🤖 AI Agent:**
> This Week's #1 Hardcover Fiction: 'The Midnight Library' by Matt Haig. It has been on the list for 12 weeks.

---

**👤 You:**
> "Find movie reviews for 'The Godfather'."

**🤖 AI Agent:**
> Found classic NYTimes reviews: 1. Original 1972 Review by Vincent Canby — 'A magnificent film'. 2. Retrospective reviews from later decades.


## ❓ FAQ

**Q: How far back does the NYTimes archive go?**
The article search API provides access to articles dating back to 1851. It is one of the most comprehensive historical newspaper archives available.

**Q: Can I get the actual text of the articles?**
The API provides the headline, abstract (summary), snippet, and URL to the full article on NYTimes.com. Full text is not included in the API response but can be accessed via the provided link.

**Q: What sections are available for Top Stories?**
You can access almost any section of the NYTimes, including home, world, politics, business, technology, sports, arts, health, and science. Use the get_sections tool to see the full list.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/new-york-times](https://vinkius.com/mcp/new-york-times)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **New York Times** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `new-york-times` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **New York Times** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "new-york-times": {
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

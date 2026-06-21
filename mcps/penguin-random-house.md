# Penguin Random House MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/penguin-random-house)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Access the global Penguin Random House catalog—search for authors, titles, works, and literary categories directly from your AI agent.

## Description
Connect the **Penguin Random House** Open Service to your AI agent to explore one of the world's largest trade book catalogs. Retrieve detailed metadata for millions of titles, authors, and literary events through natural conversation.

### What you can do

- **Author Discovery** — List authors, illustrators, and narrators. Filter by tour status or last initial to find specific contributors.
- **Title & ISBN Lookup** — Fetch complete metadata for specific book editions using ISBNs, including format details, sale dates, and award status.
- **Work Grouping** — Access 'Works' which group different formats (hardcover, ebook, audio) of the same book under a single identifier for better organization.
- **Category Hierarchy** — Explore the complex tree of book categories and genres to discover new content or classify existing lists.
- **Event Tracking** — List upcoming author events and tours to stay updated on the literary world.

### How it works

1. Subscribe to this server
2. Enter your Penguin Random House API Key
3. Start querying the catalog from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators & Researchers** — quickly verify book details, author bios, and publication dates without manual web searches.
- **Developers & Librarians** — integrate professional-grade book metadata into workflows or personal databases.
- **Book Enthusiasts** — find upcoming releases, award-winning titles, and author tour dates through simple chat.


## Available Tools
- **get_author**: Get details for a specific author
- **get_category_hierarchy**: Get category hierarchy view
- **get_series**: Get details for a specific series
- **get_title**: Get details for a specific title by ISBN
- **get_work**: Get details for a specific work
- **list_authors**: Can be scoped to a domain and filtered by tour status or last initial.

List authors, illustrators, narrators, and contributors
- **list_categories**: List book categories
- **list_events**: List author events (signings, talks)
- **list_series**: List book series
- **list_titles**: Can be scoped to a domain and filtered by format, sale dates, etc.

List book editions identified by ISBN
- **list_works**: A work groups different formats (hardcover, ebook, etc.) under a single ID.

List works (groups of different formats of the same book)
- **predictive_search**: Predictive search for autocomplete
- **search**: Responses include a facets array for filtering results.

Full-text search powered by Apache Solr


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Penguin Random House** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all authors whose last names start with 'S' and show if they are on tour."

**🤖 AI Agent:**
> I've found several authors. For example, George Saunders (ID: 27103) is currently listed. Would you like to see his full bio or check his upcoming events?

---

**👤 You:**
> "Get the full details for the book with ISBN 9780525559474."

**🤖 AI Agent:**
> That ISBN corresponds to 'The Midnight Library' by Matt Haig. It's a Hardcover edition published under the Viking imprint. It has won several awards and has a high print score. Would you like the work summary?

---

**👤 You:**
> "Search for upcoming author events in the PRH.US domain."

**🤖 AI Agent:**
> I've retrieved the latest events for the US domain. There are tours scheduled for several bestselling authors this month. Should I list the specific dates and locations for a particular author?


## ❓ FAQ

**Q: What is the difference between a 'Title' and a 'Work' in this server?**
A 'Title' refers to a specific edition (identified by ISBN), while a 'Work' (using `get_work`) groups all formats of that book—like hardcover, paperback, and ebook—under a single record.

**Q: Can I retrieve an author's biography along with their details?**
Yes! When using the `get_author` tool, set the `showBio` parameter to true to include the full author biography in the response.

**Q: How can I find books that are currently on sale or coming soon?**
Use the `list_titles` tool with filters like `showComingSoon` or date ranges `onSaleFrom` and `onSaleTo` to find specific release windows.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/penguin-random-house](https://vinkius.com/mcp/penguin-random-house)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Penguin Random House** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `penguin-random-house` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Penguin Random House** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "penguin-random-house": {
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

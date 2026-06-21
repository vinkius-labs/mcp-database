# Goodreads MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/goodreads)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

The world's largest site for readers and book recommendations — search books and audit reviews via AI.

## Description
Empower your AI agent to orchestrate your reading life and book research with **Goodreads**, the world's premier platform for readers and bibliophiles. By connecting Goodreads to your agent, you transform complex book searching, author research, and community review auditing into a natural conversation. Your agent can instantly retrieve detailed book metadata including titles and descriptions, access comprehensive author bibliographies, and audit user reviews and ratings without you ever needing to navigate the legacy Goodreads interface. Whether you are conducting literary research or coordinating your next personal read, your agent acts as a real-time librarian, providing accurate results from a single, authorized source.

### What you can do

- **Book Orchestration** — Search the massive Goodreads library and retrieve detailed metadata for any title.
- **Author Research** — Access full biographies and comprehensive bibliographies for millions of authors.
- **Review Auditing** — Retrieve and audit user reviews and community ratings to gauge book sentiment.
- **Series Discovery** — Explore book series and their members to maintain chronological reading order.
- **User Insights** — Access public user profiles and bookshelves to discover reading trends and collections.

### How it works

1. Subscribe to this server
2. Enter your legacy Goodreads API Key (and Secret if available)
3. Start managing your literary data through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Students** — automate the gathering of book metadata and author info through natural language.
- **Content Creators** — audit book reviews and community ratings to identify trending topics and sentiment.
- **Developers** — integrate professional-grade literary data into your AI-driven daily routines.
- **Goodreads Legacy Users** — continue leveraging your existing API access within your AI-driven workspace.


## Available Tools
- **get_author_profile**: Get author details
- **get_book_info**: Get book metadata
- **get_series_metadata**: Get book series info
- **get_user_public_profile**: Get user profile data
- **get_user_reviews**: Get reviews for user
- **get_user_shelves_list**: List user book shelves
- **list_author_books**: List books by author
- **search_books**: Search for books


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Goodreads** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for books by author 'Stephen King' and show me the list."

**🤖 AI Agent:**
> I've retrieved the book list for Stephen King from Goodreads. I found over 500 titles, including classics like 'The Shining', 'It', and 'Misery'. Would you like me to get the detailed metadata for a specific one?

---

**👤 You:**
> "Get the metadata and reviews summary for the book with ID '136251'."

**🤖 AI Agent:**
> I've retrieved the details for book ID `136251` ('Harry Potter and the Deathly Hallows'). It has an average rating of 4.62 from over 3 million users. Should I show you the most recent reviews for this title?

---

**👤 You:**
> "List all books in the 'Mistborn' series."

**🤖 AI Agent:**
> I've explored the 'Mistborn' series (ID: `40910`). The series contains the original trilogy plus subsequent entries like 'The Alloy of Law'. Would you like me to list them in their recommended reading order?


## ❓ FAQ

**Q: Can I still get a new Goodreads API Key?**
No. Goodreads stopped issuing new developer keys in December 2020. This server is designed for users who already possess a legacy key or for developers maintaining existing integrations.

**Q: What data format does this server return?**
The Goodreads API natively returns XML. This server retrieves the raw XML data and provides it to your agent, which can then parse and reason over the structure using natural language.

**Q: Are there limits to review access?**
Yes. Due to privacy policies, the Goodreads API typically provides snippets or widgets for reviews rather than full-text access for all users. The tools here will retrieve all information permitted by your specific API key.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/goodreads](https://vinkius.com/mcp/goodreads)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Goodreads** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `goodreads` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Goodreads** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "goodreads": {
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

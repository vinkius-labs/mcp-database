# Internet Archive Search MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/internet-archive-search)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Search 40M+ books, videos, audio, software across the Internet Archive.

## Description
Connect **Internet Archive Search** to any AI agent and perform advanced searches across the world's largest digital library — 40M+ items including books, films, music, software, and images.

### What you can do
- **Universal Search** — Complex queries with AND, OR, NOT, wildcards, field-specific searches
- **Collection Browsing** — Explore curated collections (Prelinger, Gutenberg, NASA, TV News)
- **Media Type Filtering** — Search by format: texts, movies, audio, software, images
- **Creator/Author Search** — Find all works by a specific person or organization
- **Date Range Search** — Discover content from specific decades or year ranges
- **Subject Search** — Find items by curated topic keywords
- **Top Downloads** — See what's most popular across the archive
- **Language Search** — Find content in specific languages
- **Publisher Search** — Find all content from specific publishers
- **Recent Items** — Discover newly uploaded content
- **Faceted Search** — Analyze search results by category distributions


## Available Tools
- **faceted_search**: The facets parameter uses JSON faceting syntax (e.g., "mediatype:{type:terms,field:mediatype}"). Use this to understand the composition of search results by categories like media type, collection, or creator.

Search with faceted results for category analysis
- **search_by_collection**: Use this to explore themed collections.

Search items within a specific Internet Archive collection
- **search_by_creator**: Creator names should match item metadata. Examples: "George Orwell", "NASA", "Charlie Chaplin", "Project Gutenberg". Use this to find the complete works of an author or content from an organization.

Search for all items by a specific creator or author
- **search_by_date_range**: Combines a text query with year filtering. Example: query="science fiction", startYear="1950", endYear="1959" finds 1950s sci-fi. Use this for historical content discovery.

Search for items within a specific year range
- **search_fulltext**: Returns identifier, title, and description. Use this when you need to find items containing specific terms in their descriptions. Limited to 25 results by default.

Full-text search across item descriptions and metadata
- **search_by_language**: Examples: "English", "French", "Spanish", "Portuguese", "German". Use this to find content in a specific language.

Search for items in a specific language
- **search_by_mediatype**: Use this to filter by format type.

Search for items of a specific media type
- **search_by_publisher**: Examples: "Penguin Books", "Marvel Comics", "National Geographic". Use this to find all content from a specific publisher.

Search for items by publisher name
- **search_recent**: Use this to discover new content added to the archive. Useful for staying current with new additions.

Get the most recently uploaded items to the Internet Archive
- **search_by_subject**: Subjects are curated topics assigned to items. Examples: "world war 2", "science fiction", "civil rights", "jazz music". Use this to find content about specific topics across all collections.

Search for items by subject or topic
- **search**: Supports AND, OR, NOT, wildcards (*), and field searches. Use this for broad discovery. Optional: fields (e.g., "identifier,title,mediatype"), rows (1-100), page for pagination, and sort (e.g., "date desc").

Universal search across 40M+ items in the Internet Archive
- **search_top_downloads**: Optional mediatype filter narrows to a specific format (texts, movies, audio, software). Use this to find popular content.

Get the most downloaded items from the Internet Archive


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Internet Archive Search** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for public domain films from the 1940s."

**🤖 AI Agent:**
> Found 12,847 films from the 1940s in Prelinger Archives and community collections, including WWII propaganda, educational shorts, and home movies.

---

**👤 You:**
> "Show me the most downloaded items."

**🤖 AI Agent:**
> Top downloads include: Big Buck Bunny (movie), various Project Gutenberg ebooks, NASA Apollo mission photos, and classic software from the softwarelibrary collection.

---

**👤 You:**
> "Search for NASA images."

**🤖 AI Agent:**
> Found 185,000+ NASA items including Apollo mission photographs, Hubble Space Telescope images, satellite imagery, and Space Shuttle documentation.


## ❓ FAQ

**Q: What search syntax does the Internet Archive support?**
The IA search uses Solr-like syntax: AND, OR, NOT for boolean logic, wildcards (*), phrase matching ("..."), and field-specific searches like creator:"Name", subject:"Topic", collection:"name". Combine multiple criteria for precise results.

**Q: What collections are available?**
Major collections include: prelinger (ephemeral films), gutenberg (free ebooks), nasa (space images/videos), tv (TV news archive), fedflix (government films), netlabels (independent music), softwarelibrary (classic games/apps), and thousands more community collections.

**Q: Can I search by date range?**
Yes! Use search_by_date_range with a query, start_year, and end_year. Example: query="science fiction", start_year="1950", end_year="1959" finds all sci-fi from the 1950s.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/internet-archive-search](https://vinkius.com/mcp/internet-archive-search)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Internet Archive Search** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `internet-archive-search` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Internet Archive Search** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "internet-archive-search": {
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

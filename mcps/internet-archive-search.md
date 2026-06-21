# Internet Archive Search MCP Server

Search 40M+ books, videos, audio, software across the Internet Archive.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/internet-archive-search)

## Overview
**Category:** knowledge-management
**Tools Count:** 12

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


## Installation & Usage

To install and use the **Internet Archive Search** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/internet-archive-search](https://vinkius.com/mcp/internet-archive-search)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

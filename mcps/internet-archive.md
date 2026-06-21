# Internet Archive MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/internet-archive)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/internet-archive-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/internet-archive-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [brain-trust](../categories/brain-trust.md)

Search 40M+ books, videos, audio, software. Access Wayback Machine and item metadata.

## Description
Connect the **Internet Archive** to any AI agent and access the world's largest digital library — 40M+ books, videos, audio recordings, software, images, and archived web pages — plus the Wayback Machine for historical website snapshots, all through natural conversation.

### What you can do

- **Universal Search** — Search across the entire Internet Archive collection for books, films, music, software, images, and web pages with complex query syntax
- **Collection Browsing** — Explore curated collections like Prelinger Archives, Project Gutenberg, NASA images, TV news, and more
- **Media Type Filtering** — Search specifically for texts, movies, audio, software, images, or datasets
- **Creator Search** — Find all works by a specific author, director, musician, or organization
- **Historical Date Range** — Discover content from specific decades or year ranges
- **Item Metadata** — Get complete details for any item including description, subjects, collections, file formats, and download links
- **File Listings** — See all downloadable files for an item with formats (PDF, EPUB, MP4, MP3) and sizes
- **User Reviews** — Read community reviews and ratings for archived items
- **Wayback Machine** — Check if any URL has been archived and find the closest snapshot date
- **View Statistics** — Track popularity and access counts for archived items

### How it works

1. Subscribe to this server
2. No API key needed — completely free and public
3. Start searching the world's digital library from Claude, Cursor, or any MCP-compatible client

The Internet Archive is a non-profit library providing universal access to all knowledge — no authentication or registration required for searching and viewing.

### Who is this for?

- **Researchers & Students** — find historical documents, academic papers, rare books, and primary sources from any era
- **Journalists** — use the Wayback Machine to find archived versions of websites, verify claims, and track content changes over time
- **Content Creators** — discover public domain films, music, and images for creative projects and video essays
- **Historians** — explore Prelinger Archives, government films, TV news coverage, and cultural artifacts from any decade
- **Software Developers** — access classic software, abandonware, and historical computing materials


## Available Tools
- **search_by_collection**: Common collections: "prelinger" (Prelinger Archives), "fedflix" (Federal government films), "gutenberg" (Project Gutenberg ebooks), "opensource_movies" (community films), "netlabels" (netlabel music), "softwarelibrary" (classic software), "tv" (TV news archive), "pubmed" (medical journal articles), "nasa" (NASA images and videos), "americanlibraries" (library collections). Returns items within that collection with their identifiers, titles, and metadata. Use this to browse or search within curated collections.

Search for items in a specific Internet Archive collection
- **search_by_creator**: The creator name should match how it appears in the item metadata (may be full name or organization name). Use this to find the complete works of an author, all films by a director, or all content from an organization. Example creators: "George Orwell", "Charlie Chaplin", "NASA", "Project Gutenberg".

Search for items created by a specific person or organization
- **search_by_date_range**: Combines a search query with year filtering to find historical content from a specific era. Use this to find content from specific decades or periods. Example: query="science fiction", startYear="1950", endYear="1959" finds 1950s sci-fi. The query parameter can be any valid search term. Years should be 4-digit format.

Search for items within a specific year range
- **search_by_mediatype**: Media types include: "texts" (books, articles, documents), "movies" (films, videos, TV clips), "audio" (music, podcasts, radio, audiobooks), "software" (classic PC games, applications), "image" (photos, artwork, maps), "dataset" (data files), "web" (web pages). Use this when you want to find only items of a specific format. Example: mediatype="movies" returns only video content.

Search for items of a specific media type in the Internet Archive
- **get_item_files**: Items may contain multiple files in various formats (PDF, EPUB, MP4, MP3, JPEG, etc.). The identifier is the unique item ID from search results or the item URL. Use this to see what formats are available for download. Files can be downloaded from: https://archive.org/download/{identifier}/{filename}

Get the file listing for a specific Internet Archive item
- **get_item_metadata**: Returns: title, creator, date, description, subjects, collection(s), publisher, language, license, download stats, reviews, and complete file listing with formats and sizes. The identifier is obtained from search results or can be found in the item URL (e.g., from https://archive.org/details/big_buck_bunny, the identifier is "big_buck_bunny"). Use this to get comprehensive information about a specific item before downloading or citing it.

Get complete metadata and details for a specific Internet Archive item
- **get_item_reviews**: Each review includes reviewer name, star rating, review text, and submission date. Use this to understand community reception and quality assessment of items. Not all items have reviews — community items tend to have more user feedback.

Get user reviews for a specific Internet Archive item
- **get_views_stats**: Returns total views and, when available, daily view counts and geographic breakdown. Use this to measure the popularity and reach of archived content. The identifier is the unique item ID from search results or the item URL.

Get view count statistics for an Internet Archive item
- **search**: The query parameter supports complex search syntax: AND, OR, NOT, wildcards (*), phrase matching ("..."), and field-specific searches (title:"X", subject:"Y"). Returns item identifiers, titles, media types, creators, dates, and collection info. Use this for broad searches across all media types. Optional fields parameter specifies which fields to return (comma-separated: "identifier,title,mediatype,creator,date,collection"). Default returns 25 rows; use rows to get up to 100 per page. Use page for pagination. Sort options: "date desc", "date asc", "title asc", "title desc", "creator asc", "downloads desc". Example queries: "moon landing", "subject:world war 2", "collection:prelinger".

Search the Internet Archive for books, videos, audio, software, images, and more
- **wayback_availability**: Returns the closest (most recent) archived snapshot with its timestamp and availability status. Use this to find archived versions of websites, verify if a page is preserved, or get the date of the most recent snapshot. The archived URL can be accessed at: https://web.archive.org/web/{timestamp}/{original_url}. Example: For https://example.com, returns the closest archived snapshot date and URL.

Check if a URL has been archived by the Wayback Machine and find available snapshots


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Internet Archive** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for public domain films from the 1940s."

**🤖 AI Agent:**
> Found 12,847 films from the 1940s in the Prelinger Archives and community collections. Notable items: "It's a Wonderful Life" (1946), "The Scarlet Letter" (1934), various WWII propaganda and newsreel films, educational shorts, and home movies. Most are available for free download in MP4 and OGV formats. Would you like details on any specific title?

---

**👤 You:**
> "Check if https://example.com has been archived."

**🤖 AI Agent:**
> ✅ URL is archived! Closest snapshot: 20240101120000 (January 1, 2024). View the archived page at: https://web.archive.org/web/20240101120000/https://example.com. The Wayback Machine has captured this page multiple times over the years.

---

**👤 You:**
> "Show me all NASA images available."

**🤖 AI Agent:**
> Found 185,000+ NASA items in the Internet Archive. The NASA collection includes: Apollo mission photographs, Hubble Space Telescope images, satellite imagery, astronaut training footage, Space Shuttle launches, ISS documentation, and planetary exploration photos. Items span from the 1960s to present day. Would you like to narrow by specific mission, decade, or image type?


## Installation & Usage

To install and use the **Internet Archive** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/internet-archive](https://vinkius.com/mcp/internet-archive)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

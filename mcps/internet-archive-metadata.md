# Internet Archive Metadata MCP Server

Get detailed metadata, files, reviews, and stats for any Internet Archive item.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/internet-archive-metadata)

## Overview
**Category:** knowledge-management
**Tools Count:** 10

## Description
Connect **Internet Archive Metadata** to any AI agent and retrieve comprehensive details about any archived item — including file listings, user reviews, collection memberships, access statistics, and modification history.

### What you can do
- **Complete Metadata** — Title, creator, date, description, subjects, license, language
- **File Listings** — All downloadable files with formats (PDF, EPUB, MP4, MP3) and sizes
- **User Reviews** — Community ratings and review text
- **Collection Info** — Which collections the item belongs to
- **View Statistics** — Download and view counts
- **Modification History** — Track changes made to items over time
- **Parent Collections** — Hierarchical categorization structure
- **Derivative Files** — Auto-generated thumbnails, streaming files, OCR text
- **Lightweight Lookup** — Metadata-only mode for fast queries
- **Server Info** — Storage location and hosting details


## Available Tools
- **get_collections**: Items can belong to multiple collections (e.g., "prelinger", "opensource_movies"). Use this to understand the categorization of an item.

Get collections an item belongs to
- **get_derivatives**: ). These are derived from the original uploads. Use this to see what processed formats are available.

Get auto-generated derivative files for an item
- **get_files**: Files can be downloaded from: https://archive.org/download/{identifier}/{filename}. Use this to see what formats are available.

Get all downloadable files for an Internet Archive item
- **get_metadata**: Returns title, creator, date, description, subjects, collection, files, reviews, and stats. The identifier is found in item URLs (e.g., from archive.org/details/big_buck_bunny, identifier is "big_buck_bunny"). Use this for comprehensive item information.

Get complete metadata for an Internet Archive item
- **get_history**: Use this to track changes to an item over time.

Get modification history of an Internet Archive item
- **get_metadata_only**: Lighter response for quick lookups. Use this when you only need basic item information.

Get only the metadata fields without files or reviews
- **get_parents**: Use this to understand the broader categorization structure.

Get parent collections of an Internet Archive item
- **get_reviews**: Returns reviewer names, star ratings, and review text. Not all items have reviews. Use this to see community feedback.

Get user reviews for an Internet Archive item
- **get_server_info**: Useful for understanding where files are hosted. Use this for technical diagnostics.

Get server and storage information for an item
- **get_stats**: Shows how popular the item is. Use this to measure item popularity.

Get access statistics for an Internet Archive item


## Installation & Usage

To install and use the **Internet Archive Metadata** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/internet-archive-metadata](https://vinkius.com/mcp/internet-archive-metadata)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

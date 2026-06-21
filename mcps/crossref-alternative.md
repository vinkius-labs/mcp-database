# CrossRef MCP Server

Search 150M+ academic works — find journal articles, books, DOIs, citations and scholarly metadata.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/crossref-alternative)

## Overview
**Category:** the-unthinkable
**Tools Count:** 13

## Description
Connect to **CrossRef** and explore the world's largest scholarly metadata database through natural conversation — no API key needed.

### What you can do

- **Work Search** — Search 150M+ academic works by title, author, DOI, keywords or abstract
- **DOI Lookup** — Get complete metadata for any academic work by its DOI
- **Journal Search** — Browse academic journals by name with ISSNs and work counts
- **Publisher Search** — Find academic publishers with their work counts and journal lists
- **Funder Search** — Discover research funding organizations and their funded works
- **Member Search** — Browse CrossRef member organizations that register DOIs
- **Work Types** — Explore publication types (journal-article, book-chapter, proceedings, dataset)
- **Licenses** — View academic licenses used in scholarly works

### How it works

1. Subscribe to this server
2. No API key needed — start searching immediately
3. Explore academic metadata from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers** — find relevant papers, check citation counts and discover related works
- **Students** — search for papers by topic, find journals and explore academic literature
- **Librarians** — look up DOIs, verify citations and discover journal metadata


## Available Tools
- **get_funder**: Returns funder name, country, URI, work count and location info.

Get details for a specific research funder
- **get_journal**: Returns journal title, ISSNs, publisher, work count and URL.

Get details for a specific journal by ISSN
- **get_licenses**: Returns license IDs, URLs and names.

Get list of known licenses used in academic works
- **get_member**: Returns member name, prefixes, work counts and location info.

Get details for a specific CrossRef member
- **get_publisher**: Returns publisher name, work count, journal count and location info.

Get details for a specific publisher
- **get_types**: ). Useful for filtering searches by publication type.

Get list of academic work types
- **get_work**: Returns title, authors, abstract, publication date, journal, publisher, license, references, citation count and full citation info.

Get metadata for a specific academic work by DOI
- **get_works_by_doi_list**: Provide a comma-separated list of DOIs. Returns metadata for each work including title, authors, publication date and journal.

Get metadata for multiple works by their DOIs
- **search_funders**: Returns funder names, IDs, country codes, URIs and work counts.

Search research funders by name
- **search_journals**: Returns journal titles, ISSNs, publisher names and work counts.

Search academic journals by name
- **search_members**: Returns member names, IDs, prefixes and work counts.

Search CrossRef member organizations
- **search_publishers**: Returns publisher names, work counts, journal counts and organization names.

Search academic publishers by name
- **search_works**: Supports free-text query and advanced filtering by type, publication date, author, journal, publisher, funder, license and more. Returns titles, authors, publication dates, DOIs, citation counts and abstracts.

Search academic works by title, author, DOI or keywords


## Installation & Usage

To install and use the **CrossRef** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crossref-alternative](https://vinkius.com/mcp/crossref-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

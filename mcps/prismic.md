# Prismic MCP Server

Query and manage your Prismic headless CMS content — search documents, list custom types, and retrieve specific content directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/prismic)

## Overview
**Category:** loved-by-devs
**Tools Count:** 10

## Description
Connect your **Prismic** headless CMS to any AI agent and integrate content querying directly into your conversation workflow.

### What you can do

- **Search Documents** — Perform advanced searches using Prismic predicates, filter by tags, locales, and custom types
- **Retrieve Content** — Fetch full document data by their unique IDs to immediately get component architecture and copy
- **Explore Schema** — List all available custom types, tags, and languages defined in your repository
- **Analyze Structure** — Retrieve repository metadata including master refs and view specific query form schemas

### How it works

1. Subscribe to this server
2. Enter your Prismic Repository Name and optional Access Token
3. Start fetching and analyzing your CMS content from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Frontend Developers** — query documents and components exactly as they return from the API directly inside your IDE without context switching
- **Content Managers** — quickly audit tags, find specific document IDs, and verify translations without opening the Prismic dashboard
- **SEO Specialists** — inspect live structured data, slugs, and copy for specific pages in seconds


## Available Tools
- **search_filtered_locale**: g., "en-us" or "fr-fr").

Performs a filtered search for documents within a specific locale
- **get_repo_metadata**: Retrieves metadata about the Prismic repository, including master refs, types, and languages
- **get_document_by_id**: g., from a search result or relationship field) and need to retrieve its full content.

Fetches a specific Prismic document by its unique ID
- **get_query_form_schema**: Retrieves the schema for a specific query form (e.g., "everything")
- **list_i18n_languages**: Lists the languages (locales) configured in the repository
- **list_global_tags**: Lists all tags used across the Prismic repository
- **list_custom_types**: Lists all Custom Types defined in the Prismic repository
- **list_documents_by_tag**: Lists all Prismic documents that have a specific tag
- **list_documents_by_type**: Lists all Prismic documents of a specific Custom Type
- **query_prismic_documents**: This is the most powerful tool for finding content. It supports pagination and locale filtering internally.

Queries the Prismic API for documents using raw Predicates


## Installation & Usage

To install and use the **Prismic** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/prismic](https://vinkius.com/mcp/prismic)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

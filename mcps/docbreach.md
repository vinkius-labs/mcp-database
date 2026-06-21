# DocBreach MCP Server

Real-time documentation discovery for AI agents. Discover, read, and extract any API documentation without browser rendering or API keys.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/docbreach)

## Overview
**Category:** developer-tools
**Tools Count:** 5

## Description
The web is hostile to AI agents. DocBreach brings a crowbar. Discover, read, and extract any API documentation in real-time — without browser rendering, without API keys, without SaaS dependencies. Supports OpenAPI, Swagger, Postman Collections, llms.txt, and 12+ SPA frameworks.

### What you can do

- **Discover Sources** — Find documentation sources for any service or API using `docs.discover`.
- **Read Documentation** — Read any documentation URL and return clean, LLM-ready Markdown using `docs.read`.
- **Map Structures** — Map the complete documentation structure of any domain via sitemaps using `docs.map`.
- **Search Topics** — Search for specific topics within a documentation site using `docs.search`.
- **Extract Endpoints** — Extract structured endpoint information from OpenAPI specs using `docs.extract`.

### How it works

1. Subscribe to this server
2. No authentication is required
3. Start using the tools to read and extract documentation directly from your AI agent

### Who is this for?

- **Developers** — Find API documentation for code generation and read library documentation during coding sessions.
- **AI Agents** — Extract API endpoints from OpenAPI specifications and map entire documentation sites for comprehensive context.


## Available Tools
- **docs_search**: Always provide the "site" parameter when searching within a known domain. Example: docs.search({ query: "authentication headers", site: "docs.stripe.com" })

Search for specific topics within a documentation site
- **docs_discover**: Use specific, descriptive queries. Example: "stripe API webhooks" instead of just "stripe". Combine your search intents into a single query. Do NOT call this tool in rapid loops — refine your query instead.

Find documentation sources for any service, library, or API
- **docs_map**: Provide a domain (e.g., "stripe.com") and receive a complete table of contents with every documentation page organized by section. Then use docs.read on specific pages from the map.

Map the complete documentation structure of any domain
- **docs_read**: Handles HTML, JSON, YAML, OpenAPI specs, Postman Collections, PDFs (<5MB), and llms.txt. The response includes a "Related Documentation Links" section extracted from page navigation. ALWAYS check these links for authentication and getting-started pages before generating code.

Read any documentation URL and return clean, LLM-ready Markdown
- **docs_extract**: read has identified an OpenAPI/Swagger spec URL or Postman Collection. Provide a tag to filter endpoints by API group. If no tag is provided, returns a summary of all tags with endpoint counts.

Extract structured endpoint information from an OpenAPI, Swagger, or Postman spec


## Installation & Usage

To install and use the **DocBreach** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/docbreach](https://vinkius.com/mcp/docbreach)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

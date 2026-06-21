# NPM Registry MCP Server

Search and inspect the NPM registry — query package metadata, check versions, and explore the JavaScript ecosystem directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/npm-registry)

## Overview
**Category:** developer-tools
**Tools Count:** 4

## Description
Connect to the **NPM Registry** to explore the world's largest software registry. This MCP server allows your AI agent to query package information, search for libraries, and retrieve specific version details without leaving your chat or IDE.

### What you can do

- **Package Metadata** — Fetch full or abbreviated metadata for any NPM package using its name.
- **Version Tracking** — Get specific details for any version or the 'latest' release of a package.
- **Advanced Search** — Find packages using full-text search with qualifiers for authors, keywords, and quality metrics.
- **Registry Health** — Monitor the registry instance status, document count, and database sizes.

### How it works

1. Subscribe to this server
2. Enter your NPM Read-Only Token (optional for public queries, recommended for rate limits)
3. Start searching and inspecting packages from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Software Engineers** — quickly check package dependencies, versions, and metadata without switching to a browser.
- **DevOps & CI/CD Teams** — verify package availability and version history during pipeline debugging.
- **Security Researchers** — inspect package metadata and maintenance scores to evaluate library health.


## Available Tools
- **get_registry_meta**: Get information about the NPM registry instance
- **get_package**: Get metadata for an NPM package
- **get_package_version**: Get metadata for a specific version of an NPM package
- **search_packages**: Supports qualifiers like author:name, maintainer:name, keywords:word, is:unstable, not:insecure.

Search for packages in the NPM registry


## Installation & Usage

To install and use the **NPM Registry** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/npm-registry](https://vinkius.com/mcp/npm-registry)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

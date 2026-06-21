# NPM Registry MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/npm-registry)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/npm-registry-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/npm-registry-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [developer-tools](../categories/developer-tools.md)

Search and inspect the NPM registry — query package metadata, check versions, and explore the JavaScript ecosystem directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NPM Registry** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for packages related to 'react' with high popularity."

**🤖 AI Agent:**
> I've searched the registry for 'react' with a focus on popularity. Top results include 'react' (the core library), 'react-dom', and 'react-router'. Would you like to see the specific metadata for any of these?

---

**👤 You:**
> "Get the metadata for the latest version of the 'lodash' package."

**🤖 AI Agent:**
> Fetching the latest version of 'lodash'... The current version is 4.17.21. It has 0 dependencies and is widely used for JavaScript utility functions. I can provide the full list of exported methods if needed.

---

**👤 You:**
> "What is the current document count in the NPM registry?"

**🤖 AI Agent:**
> Checking registry metadata... The NPM registry currently contains over 3.5 million documents with a total database size of approximately 2.4TB. The instance name is 'registry'.


## Installation & Usage

To install and use the **NPM Registry** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/npm-registry](https://vinkius.com/mcp/npm-registry)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

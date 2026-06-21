# DBpedia MCP Server

Access the world's largest open knowledge graph — execute SPARQL queries, lookup entities, and monitor Wikipedia updates in real-time.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/dbpedia)

## Overview
**Category:** databases
**Tools Count:** 8

## Description
Connect your AI agent to **DBpedia**, the structured heart of Wikipedia. This server allows you to perform complex semantic queries, resolve entities, and access real-time data updates from the global knowledge graph.

### What you can do

- **SPARQL Queries** — Execute powerful queries against the main DBpedia and DBpedia Live endpoints using `query_sparql` and `query_live_sparql` to extract structured data.
- **Entity Lookup** — Search for resources using keywords or autocomplete prefixes with `lookup_search` and `lookup_prefix` to find specific Wikipedia entities.
- **Resource Inspection** — Fetch full linked data (RDF, JSON-LD) for any DBpedia resource like cities, people, or events using `get_resource`.
- **Real-time Updates** — Monitor recent Wikipedia changes with `get_live_changes` and retrieve the latest article data through `get_live_resource`.
- **Bulk Retrieval** — Use `retrieve_live_articles` to extract data for multiple resources simultaneously.

### How it works

1. Subscribe to this server
2. DBpedia is a public service; simply confirm your connection to the public endpoint
3. Start querying the world's knowledge from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Researchers & Data Scientists** — extract structured datasets from Wikipedia without manual scraping
- **Developers** — enrich applications with global entity data and semantic relationships
- **AI Engineers** — provide agents with a factual grounding source for general knowledge and real-time events


## Available Tools
- **retrieve_live_articles**: Extract recent data for a list of resource names
- **get_live_changes**: List change events from the DBpedia Live Sync API
- **get_live_resource**: Retrieve the most recent data for a specific Wikipedia page
- **query_live_sparql**: dbpedia.org/sparql for real-time Wikipedia updates.

Execute a SPARQL query against the DBpedia Live endpoint
- **lookup_prefix**: Autocomplete search for DBpedia resources
- **lookup_search**: Search for DBpedia resources using keywords
- **get_resource**: g., "Berlin") using content negotiation.

Retrieve linked data for a specific DBpedia resource
- **query_sparql**: org/sparql. Max 10,000 rows.

Execute a SPARQL query against the public DBpedia endpoint


## Installation & Usage

To install and use the **DBpedia** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/dbpedia](https://vinkius.com/mcp/dbpedia)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

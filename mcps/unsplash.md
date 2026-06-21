# Unsplash MCP Server

Automate high-resolution photo searches via Unsplash — find images, browse collections, retrieve user portfolios, and get random inspiration directly from your AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/unsplash)

## Overview
**Category:** design-creative
**Tools Count:** 10

## Description
Connect the **Unsplash** photography ecosystem to any AI agent and take full autonomous control over discovering, indexing, and retrieving high-resolution imagery and curated collections native to your chat interface.

### What you can do

- **Intelligent Image Search** — Query the global massive library using natural language to extract direct photo IDs, resolution properties, and immediate HD links
- **Curated Collection Auditing** — Dive into thematic human-curated folders grabbing entire bundles of contextual visuals natively via API `search_collections`
- **Random Inspiration Hooks** — Prompt the LLM to pluck out absolutely random high-res visuals based on subtle conceptual inputs finding the elusive perfect placeholder
- **Photographer Telemetry** — Isolate public artists retrieving entire portfolios tracking the `search_users` capabilities inherently within your workspace

### How it works

1. Subscribe manually to this connected MCP instance
2. Introduce your Personal Unsplash Developer App Access Key 
3. Start mapping live creative inquiries inside Claude or Cursor without navigating web libraries manually

Drop visually browsing the Unsplash homepage for 30 minutes. Provide specific semantic constraints to your AI agent and receive the exact raw asset links instantly.

### Who is this for?

- **Content Editors & Bloggers** — automatically request the AI to find 3 "minimalist coffee shop" images returning direct hotlinks bypassing manual downloads
- **Frontend Architects** — rapidly ingest realistic placeholder imagery natively when scaffolding React projects instructing Cursor to pull random visuals
- **Design Agencies** — fetch thematic collections querying specialized curations finding a consistent look & feel without switching contexts


## Available Tools
- **list_collection_photos**: Requires a collection ID.

Lists all photos contained within a specific collection
- **get_collection_details**: Retrieves details for a specific photo collection
- **get_photo_details**: Retrieves details for a specific Unsplash photo
- **get_photographer_photos**: Lists photos uploaded by a specific Unsplash user
- **list_latest_photos**: Lists the most recently uploaded photos on Unsplash
- **list_editorial_topics**: Lists curated editorial topics (Nature, Architecture, etc.)
- **get_random_photo**: Optionally provide a query to narrow the random selection.

Retrieves a random high-resolution photo
- **search_collections**: g. "Nature", "Industrial").

Search for curated photo collections by keyword
- **search_photos**: Returns photo IDs, URLs, and photographer information. Note: Proper attribution is required.

Search Unsplash for free high-resolution photos
- **search_photographers**: Search for Unsplash photographers by name or username


## Installation & Usage

To install and use the **Unsplash** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unsplash](https://vinkius.com/mcp/unsplash)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

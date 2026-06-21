# Unsplash MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/unsplash)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/unsplash-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/unsplash-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Automate high-resolution photo searches via Unsplash — find images, browse collections, retrieve user portfolios, and get random inspiration directly from your AI agent.

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


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Unsplash** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for 3 high resolution images containing 'cyberpunk city' aesthetics and provide their URLs natively in your response."

**🤖 AI Agent:**
> I've tapped the search engine: I found three gorgeous neon-lit cyberpunk style captures. [Image 1: Tokyo Nights API URL], [Image 2: Neon Reflection API URL], [Image 3: Rainy Alley API URL]. Photographers are mentioned below for proper attribution.

---

**👤 You:**
> "Grab a random photo matching 'coffee desk concept' to help me prototype a blog layout."

**🤖 AI Agent:**
> Random request executed. I returned Photo ID yX45p, showcasing a minimalist white desk with an espresso shot, shot natively by James L. [Here is the Raw Image URL] to plug into your `src` tag.

---

**👤 You:**
> "I need to see what's trending. Quickly gather the 10 most recently published latest photos off the main feed."

**🤖 AI Agent:**
> I've hit the latest unformatted feed natively. The top fresh photos display a significant trend in abstract landscapes and minimalist tech setups from users across Europe. Returning a list of their IDs alongside URLs right now.


## Installation & Usage

To install and use the **Unsplash** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/unsplash](https://vinkius.com/mcp/unsplash)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

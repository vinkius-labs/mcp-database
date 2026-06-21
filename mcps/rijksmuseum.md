# Rijksmuseum MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rijksmuseum)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/rijksmuseum-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/rijksmuseum-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [knowledge-management](../categories/knowledge-management.md)

Explore the Rijksmuseum's world-class art collection and research library. Search for masterpieces, access high-resolution image metadata via IIIF, and query linked open data.

## Description
Connect your AI agent to the **Rijksmuseum Data API** to explore centuries of Dutch art and history. This server provides comprehensive access to the museum's digital collection, research library, and high-resolution image services.

### What you can do

- **Collection Search** — Query the museum's vast holdings by creator (e.g., Rembrandt), title, material, technique, or specific time periods.
- **Research Library** — Access bibliographic records from the Rijksmuseum Research Library using the SRU protocol for deep academic research.
- **IIIF Integration** — Retrieve standardized IIIF manifests and image metadata to inspect high-resolution digital assets and object structures.
- **Linked Open Data** — Harvest metadata via OAI-PMH or explore immutable object streams through Linked Data Event Streams (LDES).
- **Persistent Identifiers** — Resolve PIDs to ensure you are always looking at the most accurate and up-to-date metadata for any given object.

### How it works

1. Subscribe to this server
2. Enter your Rijksmuseum API Key
3. Start exploring art history directly from your AI assistant

### Who is this for?

- **Art Historians & Researchers** — Quickly find specific works, bibliographic references, and detailed provenance data.
- **Educators & Students** — Explore the collection for educational materials and high-quality imagery.
- **Developers & Data Scientists** — Integrate cultural heritage data into applications or perform large-scale metadata analysis.


## Available Tools
- **get_iiif_image_info**: Get IIIF image metadata
- **get_iiif_manifest**: Get IIIF presentation manifest
- **get_ldes_collection**: Get the Linked Data Event Streams (LDES) collection
- **get_ldes_dataset**: Get a specific LDES dataset
- **oai_pmh_request**: Harvest metadata using the OAI-PMH API
- **resolve_pid**: Supports content negotiation.

Dereference a Persistent Identifier (PID)
- **search_collection**: Returns Linked Open Data identifiers based on various filters.

Search for characteristics of objects in the Rijksmuseum collection
- **search_library**: Supports Contextual Query Language (CQL).

Search bibliographic records from the Rijksmuseum Research Library


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Rijksmuseum** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search the Rijksmuseum collection for paintings by Johannes Vermeer."

**🤖 AI Agent:**
> I've found several works by Johannes Vermeer, including 'The Milkmaid' (SK-A-2344) and 'The Love Letter' (SK-A-1595). Would you like to see the detailed description or IIIF manifest for any of these?

---

**👤 You:**
> "Find books about the restoration of 'The Night Watch' in the research library."

**🤖 AI Agent:**
> Searching the library records... I found several bibliographic entries related to the restoration of Rembrandt's 'Night Watch', including technical reports and exhibition catalogs. Here are the top results...

---

**👤 You:**
> "Get the IIIF image info for the identifier 'SK-C-5'."

**🤖 AI Agent:**
> Retrieving IIIF metadata for 'The Night Watch' (SK-C-5)... The image is available at a maximum resolution of 12000x10000 pixels with support for multiple zoom levels and formats. You can access the tiles via the following base URL...


## Installation & Usage

To install and use the **Rijksmuseum** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rijksmuseum](https://vinkius.com/mcp/rijksmuseum)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

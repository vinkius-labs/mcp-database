# Xeno-canto MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/xeno-canto)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/xeno-canto-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/xeno-canto-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [audio-music](../categories/audio-music.md)

Search and explore the world's largest collection of bird sound recordings directly from your AI agent.

## Description
Connect to the **Xeno-canto** database to access over 800,000 recordings of bird sounds from across the globe. This MCP server allows your AI agent to query the massive open-access collection of wildlife sounds for research, identification, or education.

### What you can do

- **Advanced Search** — Query recordings using specific filters like genus, species, country, or quality grade using the `search_recordings` tool.
- **Scientific Data** — Retrieve metadata including location, recordist, date, and sound type (song, call, etc.) for every recording found.
- **Global Coverage** — Access recordings from every continent, covering thousands of species and subspecies.
- **Pagination Support** — Navigate through large result sets with built-in page management for comprehensive data analysis.

### How it works

1. Subscribe to this server
2. No API key is required for public access to the Xeno-canto database
3. Start searching for bird sounds using natural language or Xeno-canto's advanced query syntax

### Who is this for?

- **Ornithologists & Researchers** — quickly gather audio data and metadata for specific species across different geographic regions.
- **Nature Enthusiasts** — identify bird calls and explore the vocalizations of birds from around the world.
- **Data Scientists** — collect bioacoustic datasets for machine learning and environmental analysis.


## Available Tools
- **search_recordings**: g., gen:Turdus cnt:france q:A).

Search for bird sound recordings on Xeno-canto


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Xeno-canto** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for recordings of the Common Blackbird in the Netherlands."

**🤖 AI Agent:**
> I've found several recordings for the Common Blackbird (Turdus merula) in the Netherlands. The top results include high-quality songs recorded in Gelderland and Utrecht. Would you like to see the details for a specific recording?

---

**👤 You:**
> "Find high-quality recordings of the genus Turdus in France using quality grade A."

**🤖 AI Agent:**
> Searching for high-quality (grade A) recordings of Turdus in France... I've retrieved 15 recordings, including Turdus philomelos and Turdus merula. All these recordings are rated 'A' for excellent sound clarity.

---

**👤 You:**
> "Get the second page of results for 'owl' recordings."

**🤖 AI Agent:**
> Fetching page 2 of the search results for 'owl'... I have loaded the next set of recordings, featuring various species like the Barn Owl and Tawny Owl from different global locations.


## Installation & Usage

To install and use the **Xeno-canto** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/xeno-canto](https://vinkius.com/mcp/xeno-canto)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

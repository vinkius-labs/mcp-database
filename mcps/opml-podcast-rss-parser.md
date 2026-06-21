# OPML Podcast & RSS Parser MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/opml-podcast-rss-parser)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/opml-podcast-rss-parser-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/opml-podcast-rss-parser-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Turn standard OPML export files from your podcast app or RSS reader into clean JSON data. Let your AI analyze your subscriptions and become your personal content curator.

## Description
When you want Claude to recommend new podcasts or blogs based on what you already consume, you export an `.opml` file from Apple Podcasts, Pocket Casts, or Feedly. But XML outlines are noisy, recursive, and confusing for LLMs to read efficiently.

This MCP uses a fast, deterministic XML parser to flatten the OPML hierarchy into a simple, structured list of your subscriptions, dropping all the unnecessary XML tags and attributes.

### The Superpowers

- **Universal Support:** Parses OPML files from any standard podcast player or RSS reader.
- **Zero Token Waste:** Converts heavy XML markup into a clean, flat JSON array.
- **Local Privacy:** Your subscription habits are parsed locally, ensuring they aren't uploaded to a public server.
- **Assistant Ready:** Turn Claude into your personal entertainment and news curator.


## Available Tools
- **parse_opml_feeds**: Provide the absolute file path.

Parse an OPML file (Podcast or RSS feed export) into a clean JSON list of subscriptions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **OPML Podcast & RSS Parser** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Read my podcasts.opml file and recommend 3 new tech podcasts I might like."

**🤖 AI Agent:**
> Based on your 15 current tech subscriptions (like Lex Fridman), I highly recommend: 1. Hard Fork, 2. Syntax, 3. The Vergecast.

---

**👤 You:**
> "Extract all the RSS URLs from my Feedly export and format them as a Markdown table."

**🤖 AI Agent:**
> | Title | RSS Feed URL |
|-------|-------------|
| Wired | wired.com/feed |
| TechRadar | techradar.com/rss |

---

**👤 You:**
> "Analyze my OPML file and tell me what my primary interests are."

**🤖 AI Agent:**
> Looking at your 45 subscriptions, your primary interests are: 1. Artificial Intelligence (12 feeds), 2. Economics (8 feeds), 3. Design (5 feeds).


## Installation & Usage

To install and use the **OPML Podcast & RSS Parser** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/opml-podcast-rss-parser](https://vinkius.com/mcp/opml-podcast-rss-parser)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

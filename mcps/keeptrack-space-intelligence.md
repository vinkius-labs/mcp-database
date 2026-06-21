# KeepTrack Space Intelligence MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/keeptrack-space-intelligence)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/keeptrack-space-intelligence-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/keeptrack-space-intelligence-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Universal space intelligence — search satellites, orbital debris, and launches via AI.

## Description
Equip your AI agent with real-time orbital intelligence through the **KeepTrack** MCP server. This integration provides instant access to a massive database of satellites, space debris, and other objects orbiting the Earth. Your agent can search for satellites by name, retrieve detailed metadata (including NORAD IDs, country of origin, and launch dates), and monitor the most recent objects launched into space. Whether you are conducting aerospace research, tracking telecommunications assets, or exploring orbital mechanics, your agent acts as a dedicated space operations analyst through natural conversation.

### What you can do

- **Satellite Search** — Find satellites and orbital objects by name or keyword.
- **Metadata Retrieval** — Access exhaustive info including NORAD IDs, orbit types, and country data.
- **Launch Monitoring** — Retrieve a list of the most recent objects deployed into orbit.
- **Orbital Auditing** — Track specific satellite constellations like Starlink or GPS.

### How it works

1. Subscribe to this server
2. No API Key required (Public Access)
3. Start querying orbital data from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Aerospace Engineers & Researchers** — quickly verify satellite records and orbital status.
- **Astronomy Enthusiasts** — identify objects passing overhead and research space history.
- **Telecommunications Analysts** — track commercial and government satellite assets.
- **Data Scientists** — access a reliable source of structured orbital metadata.


## Available Tools
- **get_recent_space_launches**: Get most recent space launches
- **get_satellite_details**: Get details for a specific satellite
- **search_satellites**: Search for satellites by name


## 💬 Prompt Examples

Here are some examples of how you can interact with the **KeepTrack Space Intelligence** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for satellites named 'Starlink'."

**🤖 AI Agent:**
> Searching the KeepTrack database... I've found a large list of Starlink satellites. Would you like to see the NORAD IDs for the most recent ones or specific orbital data for one of them?


## Installation & Usage

To install and use the **KeepTrack Space Intelligence** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/keeptrack-space-intelligence](https://vinkius.com/mcp/keeptrack-space-intelligence)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

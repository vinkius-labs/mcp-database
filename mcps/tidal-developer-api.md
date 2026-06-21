# TIDAL Developer API MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/tidal-developer-api)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/tidal-developer-api-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/tidal-developer-api-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Access music data — audit albums, artists, and tracks via AI.

## Description
Empower your AI agent to orchestrate your entire music research and discography auditing workflow with the **TIDAL Developer API**, the comprehensive source for high-fidelity audio metadata. By connecting TIDAL to your agent, you transform complex music searches into a natural conversation. Your agent can instantly search for albums, audit artist catalogs, and retrieve track lists without you ever touching a music app. Whether you are conducting industry research or managing local playlist constraints, your agent acts as a real-time musical consultant, ensuring your data is always comprehensive and up-to-the-minute.

### What you can do

- **Album Auditing** — Search for thousands of albums by title or artist and retrieve detailed metadata, including track counts and durations.
- **Artist Oversight** — Audit comprehensive artist profiles and discographies to maintain a clear view of musical distribution and scale.
- **Track Discovery** — Query all tracks belonging to specific albums to understand the thematic distribution of music instantly.
- **Metadata Intelligence** — Retrieve high-resolution identifiers and duration markers for any musical record to assist in deep-dive classification.
- **Operational Monitoring** — Check API status to ensure your music research workflow is always operational.

### How it works

1. Subscribe to this server
2. Enter your TIDAL Developer API Key
3. Start managing your musical intelligence through Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Music Analysts & Journalists** — monitor artist catalogs and retrieve official metadata straight from your workflow.
- **Curators & DJ's** — verify track durations and audit album availability without manual searching.
- **App Developers** — perform rapid audits of music data and identify relevant stylistic markers through natural language.
- **Operations Leads** — automate musical data querying to orchestrate cross-functional creative teams smoothly.


## Available Tools
- **check_api_status**: Check if the TIDAL Developer service is operational
- **get_artist_albums**: Get all albums for a specific artist by ID
- **get_album_tracks**: Get all tracks belonging to a specific album by ID
- **search_tidal_albums**: Search for albums on TIDAL by name or artist
- **search_tidal_artists**: Search for artists on TIDAL


## 💬 Prompt Examples

Here are some examples of how you can interact with the **TIDAL Developer API** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for album 'Lemonade' by Beyoncé using TIDAL."

**🤖 AI Agent:**
> I've retrieved the details for Lemonade! It was released in 2016 and features 12 tracks. Would you like the full tracklist or the artist's full discography metadata?

---

**👤 You:**
> "What are the tracks in the album with ID '12345'?"

**🤖 AI Agent:**
> I've identified the tracks for that album! It includes 10 entries with their respective durations and unique identifiers. I can provide the direct links to each track if you'd like.

---

**👤 You:**
> "Search for artist 'Daft Punk' on TIDAL."

**🤖 AI Agent:**
> I've identified the artist Daft Punk! They are currently identified as an active entity in the TIDAL catalog. I can retrieve their full list of albums and top tracks to help you audit their discography.


## Installation & Usage

To install and use the **TIDAL Developer API** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/tidal-developer-api](https://vinkius.com/mcp/tidal-developer-api)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

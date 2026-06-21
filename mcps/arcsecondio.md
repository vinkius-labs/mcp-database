# Arcsecond.io MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/arcsecondio)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/arcsecondio-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/arcsecondio-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Access astronomical data and manage observatories with Arcsecond.io — search objects and track night logs via AI.

## Description
The **Arcsecond.io MCP Server** provides a unified natural language interface to the world's astronomical data. Connect your Arcsecond account to your AI agent to search for celestial objects, manage observatory data, and track observation night logs seamlessly.

### Key Features

- **Celestial Object Search** — Search for stars, galaxies, planets, and more to retrieve official names, types, and precise coordinates (RA/Dec).
- **Object Metadata** — Access detailed astrophysical data, including visual magnitude and classifications for millions of objects.
- **Observatory Management** — List observing sites, telescopes, and instruments associated with your observatory subdomain.
- **Data Tracking** — Access datasets and night logs to monitor ongoing observations and historical data collections.
- **Night Log Oversight** — Retrieve detailed logs of observations and calibrations organized by local noon-to-noon cycles.
- **Global Data Access** — Interface with a vast network of astronomical databases through a single, consistent API.

### Who is this for?

- **Professional Astronomers** — Quickly retrieve object coordinates and check observatory status without manual database queries.
- **Amateur Stargazers** — Search for interesting celestial targets and get detailed metadata for planning observation sessions.
- **Data Scientists** — Integrate astronomical data retrieval into automated research and analysis workflows.


## Available Tools
- **get_account_check**: Verify Arcsecond account connection
- **get_object**: Get details for a specific astronomical object
- **list_datasets**: List datasets available for an observatory
- **list_night_logs**: List observation night logs for an observatory
- **list_observing_sites**: List observing sites for an observatory
- **list_telescopes**: List telescopes for an observatory
- **search_objects**: Search for astronomical objects (stars, galaxies, planets)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Arcsecond.io** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for the 'Andromeda Galaxy' and get its coordinates."

**🤖 AI Agent:**
> I've found the Andromeda Galaxy (M31). Its coordinates are RA: 00h 42m 44s, Dec: +41° 16′ 09″.

---

**👤 You:**
> "List all observing sites for the 'lco' observatory."

**🤖 AI Agent:**
> The LCO observatory has several sites, including McDonald Observatory (Texas), Cerro Tololo (Chile), and Siding Spring (Australia).

---

**👤 You:**
> "Show me recent night logs for subdomain 'my-observatory'."

**🤖 AI Agent:**
> I've retrieved the latest 5 night logs for 'my-observatory'. The most recent log from last night contains 15 successful observations and 3 calibration frames.


## Installation & Usage

To install and use the **Arcsecond.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/arcsecondio](https://vinkius.com/mcp/arcsecondio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

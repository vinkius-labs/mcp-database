# CityBikes (Bike Sharing) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/citybikes-bike-sharing)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/citybikes-bike-sharing-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/citybikes-bike-sharing-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [travel-hospitality](../categories/travel-hospitality.md)

Access real-time bike-sharing data from over 400 cities worldwide — list networks and check station availability instantly.

## Description
Connect to the **CityBikes** API through your AI agent to retrieve live micromobility data from hundreds of global networks. Whether you are building travel tools or checking your local commute, get precise data on bike availability and station locations.

### What you can do

- **Global Network Discovery** — List all supported bike-sharing networks across the globe, including their location and unique identifiers.
- **Real-time Availability** — Fetch live data for specific networks to see exactly how many bikes and empty docks are available at every station.
- **Station Metadata** — Access precise coordinates and station names to map out bike-sharing infrastructure in any supported city.
- **Filtered Queries** — Use specific fields to optimize data retrieval and focus only on the information you need.

### How it works

1. Subscribe to this server
2. No complex API keys are required for public access
3. Start querying bike networks from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Commuters & Travelers** — quickly find the nearest bike or empty dock in a new city without downloading multiple apps.
- **Data Analysts** — gather real-time urban mobility data for research or visualization projects.
- **Developers** — integrate live transport data into custom dashboards or travel assistants.


## Available Tools
- **get_network**: Get detailed information about a specific bike-sharing network
- **list_networks**: List all bike-sharing networks


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CityBikes (Bike Sharing)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "List all bike-sharing networks available in Italy."

**🤖 AI Agent:**
> I've found several networks in Italy. Some major ones include 'Bicincittà' in various cities, 'ToBike' in Turin (ID: tobike), and 'BikeMi' in Milan (ID: bikemi). Which city are you interested in?

---

**👤 You:**
> "Check the current bike availability for the 'velib' network in Paris."

**🤖 AI Agent:**
> Fetching live data for Vélib' Métropole... I see 1,400+ stations. For example, the station at 'Mairie du 14ème' currently has 12 mechanical bikes and 5 electric bikes available. Do you want to check a specific area?

---

**👤 You:**
> "Get detailed information for the bike network with ID 'citibike-nyc'."

**🤖 AI Agent:**
> Accessing Citi Bike NYC data... This network operates in New York, NY. I have access to real-time status for all stations, including location coordinates and current bike/dock counts. Would you like a summary of the nearest stations?


## Installation & Usage

To install and use the **CityBikes (Bike Sharing)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/citybikes-bike-sharing](https://vinkius.com/mcp/citybikes-bike-sharing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

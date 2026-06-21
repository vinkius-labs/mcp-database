# NASA Open Data MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nasa-open-data)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nasa-open-data-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nasa-open-data-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Universal space intelligence — access NASA APOD, Mars photos, and NEO feed via AI.

## Description
Equip your AI agent with the wonders of the universe through the **NASA Open Data** MCP server. This integration provides real-time access to official NASA databases, including the Astronomy Picture of the Day (APOD), high-resolution imagery from Mars Rovers (Curiosity, Opportunity, Spirit), and the Near Earth Object (NEO) feed for tracking asteroids. Whether you are an astronomy enthusiast, a space researcher, or an educator, your agent acts as a dedicated space science mission specialist through natural conversation.

### What you can do

- **Astronomy Discovery** — Retrieve the daily astronomy picture and its detailed scientific explanation.
- **Planetary Imaging** — Access real-time photos from Mars and monitor Earth via the DSCOVR EPIC instrument.
- **Solar Weather Intelligence** — Track Coronal Mass Ejections (CME) and Solar Flares from the Space Weather Database.
- **Asteroid Tracking** — Monitor Near Earth Objects, track specific asteroids by ID, and review potential Earth impact risks.
- **Space Auditing** — Summarize complex astronomical findings and historical space mission data.

### How it works

1. Subscribe to this server
2. Enter your NASA API Key (get it at api.nasa.gov)
3. Start exploring the cosmos from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Astronomy Enthusiasts** — track daily cosmic events, solar flares, and Martian exploration.
- **Educators & Students** — access reliable high-quality space data for learning and assignments.
- **Science Researchers** — pull structured metadata for asteroids and planetary science.
- **Content Creators** — source stunning official NASA imagery for various digital media.


## Available Tools
- **get_astronomy_picture**: Get the NASA Astronomy Picture of the Day (APOD)
- **get_coronal_mass_ejections**: Get records of Coronal Mass Ejections (CME) from the Space Weather Database
- **get_solar_flares**: Get records of Solar Flares from the Space Weather Database
- **get_earth_polychromatic_images**: Get Earth Polychromatic Imaging Camera (EPIC) images
- **get_mars_rover_manifest**: Get the mission manifest and photo details for a Mars Rover
- **get_mars_rover_photos**: Get photos from Mars rovers (Curiosity, Opportunity, Spirit)
- **get_near_earth_objects_feed**: Get a list of Near Earth Objects (asteroids) for a specific date range
- **lookup_asteroid**: Lookup details for a specific Near Earth Object (Asteroid)


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NASA Open Data** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me today's NASA Astronomy Picture of the Day."

**🤖 AI Agent:**
> Retrieving today's APOD... I found a stunning image of the 'Pillars of Creation'. It captures a vast region of interstellar gas and dust in the Eagle Nebula. Would you like to read the full scientific explanation?

---

**👤 You:**
> "Get photos from the Curiosity rover on Earth date 2023-05-15."

**🤖 AI Agent:**
> Checking Curiosity's records for May 15, 2023... I've retrieved several images from its Mastcam and Navigation cameras showing the rocky terrain of the Gale Crater. I can provide the links to the full-resolution photos.

---

**👤 You:**
> "Are there any potentially hazardous asteroids approaching Earth this week?"

**🤖 AI Agent:**
> Analyzing the NASA NEO feed for this week... I've identified 12 near earth objects. Two of them, designated as '2024 AB' and '2024 CD', are classified as potentially hazardous but will pass at a safe distance. Would you like to see their specific sizes and speeds?


## Installation & Usage

To install and use the **NASA Open Data** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nasa-open-data](https://vinkius.com/mcp/nasa-open-data)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

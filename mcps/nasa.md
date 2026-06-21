# NASA MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nasa)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nasa-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nasa-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Explore space and science via NASA APIs — browse APOD, Mars rover photos, Earth imagery, NEO data and patents from any AI agent.

## Description
Connect to **NASA**'s open APIs through any AI agent and explore space science through natural conversation.

### What you can do

- **Astronomy Picture of the Day** — Fetch today's APOD or any historical image with title, explanation and media URL
- **Mars Rover Photos** — Browse photos from Curiosity, Perseverance, Opportunity and Spirit rovers by date and camera
- **Earth Satellite Imagery** — View Landsat 8 satellite imagery for any coordinate on Earth with date filtering
- **EPIC Earth Images** — See full-disk Earth images from the DSCOVR satellite's Deep Space Camera
- **Near-Earth Objects** — Track asteroids and their size, velocity and hazard rating over a date range
- **NASA Library Search** — Search NASA's extensive image and video library with free-text queries
- **Patent & Technology Transfer** — Search NASA patents and discover technologies available for licensing

### How it works

1. Subscribe to this server
2. Enter your NASA API Key (free at api.nasa.gov)
3. Start exploring space from Claude, Cursor, or any MCP-compatible client

No more navigating multiple NASA websites to find Mars photos or check asteroid data. Your AI acts as a dedicated space science assistant.

### Who is this for?

- **Educators** — quickly find APOD images, Mars photos and space data for lessons and presentations
- **Developers** — discover NASA datasets, search the media library and explore technology transfer opportunities
- **Space Enthusiasts** — track near-Earth objects, browse rover photos and view satellite imagery of any location


## Available Tools
- **get_apod**: If no date is specified, returns today's APOD. Optionally specify a single date, a date range (start_date and end_date), or a count of random APODs. Returns the image/video URL, title, explanation, copyright and date. This is one of NASA's most popular APIs.

Get NASA Astronomy Picture of the Day (APOD)
- **get_epic_images**: Optionally specify a date (YYYY-MM-DD) and whether to use enhanced-color images (true) or natural-color (false, default). Returns image URLs, coordinates and acquisition time.

Get Earth Polychromatic Imaging Camera (EPIC) images from NASA
- **get_earth_imagery**: Requires longitude and latitude coordinates. Optionally specify a date (YYYY-MM-DD) to get imagery from a specific time. Returns the image URL and metadata. Useful for viewing geographic changes over time.

Get satellite imagery of Earth from NASA
- **get_mars_photos**: Optionally filter by Earth date (YYYY-MM-DD), camera type (FHAZ, RHAZ, MAST, CHEMCAM, MAHLI, MARDI, NAVCAM, PANCAM, MINITES), and page number. Each photo includes the image URL, rover name, camera, Earth date and Mars sol date.

Get Mars Rover photos from NASA
- **get_mars_rovers**: Useful for discovering which rovers are active and when they last took photos.

Get information about NASA Mars rovers
- **get_neo_feed**: Optionally specify a start and end date (YYYY-MM-DD, max 7 days range). Returns asteroid count per day, estimated diameters, velocity, and whether they are potentially hazardous. Great for space awareness and planetary defense tracking.

Get Near-Earth Object (NEO) feed from NASA
- **get_tech_transfer**: Optionally filter by category (software, patent). Returns descriptions, contact information and availability status.

Get NASA technology transfer information
- **search_nasa_library**: Accepts a free-text query and returns matching media with titles, descriptions, NASA center information and media type (image, video, audio). Optionally set page number for pagination. This is the primary search endpoint for NASA media assets.

Search the NASA Image and Video Library
- **search_patents**: Requires a search query. Returns patent titles, numbers, abstracts and licensing availability. Useful for technology transfer and commercialization research.

Search NASA patents


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NASA** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Show me today's Astronomy Picture of the Day."

**🤖 AI Agent:**
> Today's APOD is 'Pillars of Creation Revisited' — a stunning new infrared image of the Eagle Nebula's iconic star-forming columns captured by the James Webb Space Telescope. The image reveals previously hidden protostars and dust structures.

---

**👤 You:**
> "Show me photos taken by the Perseverance rover on Mars."

**🤖 AI Agent:**
> I found 25 photos from Perseverance taken on 2024-01-15. Images include views of Jezero Crater using the NAVCAM, close-up rock analysis with MAHLI, and terrain mapping with RHAZ. Each photo includes the Sol number and Earth date.

---

**👤 You:**
> "Are there any potentially hazardous asteroids approaching Earth this week?"

**🤖 AI Agent:**
> Over the next 7 days, NASA is tracking 18 near-Earth objects. 2 are classified as 'potentially hazardous'. The largest is approximately 340 meters in diameter (2024 AB1), passing at a safe distance of 4.2 lunar distances on Wednesday. No impact threats are known.


## Installation & Usage

To install and use the **NASA** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nasa](https://vinkius.com/mcp/nasa)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

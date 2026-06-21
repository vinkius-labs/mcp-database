# NASA MCP Server

Explore space and science via NASA APIs — browse APOD, Mars rover photos, Earth imagery, NEO data and patents from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/nasa)

## Overview
**Category:** the-unthinkable
**Tools Count:** 9

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


## Installation & Usage

To install and use the **NASA** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nasa](https://vinkius.com/mcp/nasa)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

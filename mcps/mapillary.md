# Mapillary MCP Server

Access street-level imagery — search images, sequences, traffic signs and map features worldwide.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/mapillary)

## Overview
**Category:** image-video
**Tools Count:** 7

## Description
Connect to **Mapillary** and access the world's largest street-level imagery platform through natural conversation.

### What you can do

- **Image Search** — Search street-level images by geographic bounding box
- **Image Details** — Get image metadata including GPS coordinates, capture date, compass angle and sequence
- **Sequence Search** — Find image sequences (connected images along routes) by area
- **Map Features** — Search detected traffic signs, objects and road markings by area
- **Object Detections** — Get all detected objects in a specific image

### How it works

1. Subscribe to this server
2. Enter your Mapillary access token
3. Start exploring street-level imagery from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Urban Planners** — analyze street-level imagery for infrastructure and traffic sign inventory
- **Researchers** — access geotagged imagery and map features for GIS and environmental studies
- **Developers** — integrate street-level imagery into mapping and navigation applications


## Available Tools
- **get_detection_value**: Returns the detected value, type, GPS coordinates and image association.

Get details for a specific object detection
- **get_image**: Returns image ID, capture date/time, GPS coordinates, compass angle, sequence ID, organization and thumbnail URL. Use fields parameter to request additional data like "geometry,compass_angle,captured_at,sequence,thumb_256_url,thumb_1024_url,altitude".

Get details for a specific Mapillary image
- **get_image_detections**: Returns detection values, types, geometry and confidence scores.

Get object detections for a specific image
- **get_map_features**: Returns feature type, value, GPS coordinates and detection confidence. Useful for traffic sign inventory and road infrastructure analysis.

Search map features (traffic signs, objects) by area
- **get_sequence**: Returns sequence ID, creation date and related images.

Get details for a specific image sequence
- **search_images**: Returns image IDs, coordinates, capture dates, compass angles and sequence IDs. Bbox format: min_lon,min_lat,max_lon,max_lat (e.g. "-0.15,51.50,-0.10,51.52" for central London).

Search street-level images by geographic area
- **search_sequences**: Returns sequence IDs and metadata for all sequences that pass through the area.

Search image sequences by geographic area


## Installation & Usage

To install and use the **Mapillary** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/mapillary](https://vinkius.com/mcp/mapillary)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

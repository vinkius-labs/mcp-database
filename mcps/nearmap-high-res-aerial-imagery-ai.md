# Nearmap (High-Res Aerial Imagery & AI) MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nearmap-high-res-aerial-imagery-ai)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/nearmap-high-res-aerial-imagery-ai-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/nearmap-high-res-aerial-imagery-ai-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [the-unthinkable](../categories/the-unthinkable.md)

Manage geospatial data via Nearmap — retrieve high-res aerial imagery, extract AI features, and audit survey coverage.

## Description
Connect your **Nearmap** account to any AI agent and take full control of world-class high-resolution aerial imagery, geospatial AI insights, and topographic surface models through natural conversation.

### What you can do

- **Aerial Orchestration** — Retrieve sub-15cm resolution vertical (nadir) imagery tiles using Web Mercator coordinates to verify site conditions directly from your agent
- **AI Feature Extraction** — Automatically detect and extract vector geometries for buildings, swimming pools, solar panels, and vegetation within specific geographic radii
- **Perspective Oblique Imagery** — Access 3D-angled imagery from North, South, East, and West viewpoints to audit structural facades and building heights securely
- **Coverage & Survey Audit** — Verify imagery availability across specific points or complex polygons and retrieve chronological survey dates to track site changes over time
- **Topographic Modeling** — Extract Digital Surface Model (DSM) elevation tiles to analyze terrain peaks, building heights, and surface volumes natively within your workspace
- **True Ortho Visualization** — Retrieve geometric lean-corrected top-down layers providing zero parallax alignments for perfect geospatial mapping and precision measurement
- **Survey Metadata** — Query explicit flight parameters including Ground Sample Distance (GSD) and optical capture details for any specific aerial flyover

### How it works

1. Subscribe to this server
2. Enter your Nearmap API Key
3. Start exploring location intelligence from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Insurance Adjusters** — audit property conditions and detect roof features through natural conversation without manual site visits
- **Urban Planners & Architects** — verify site dimensions and topographic elevations directly from your workspace using high-res imagery
- **Solar Installers** — identify existing solar arrays and extract roof geometries to optimize installation planning and resource allocation efficiently


## Available Tools
- **list_ai_feature_classes**: Lookup all internal AI category taxonomies evaluating computer vision mappings detecting roof arrays
- **get_ai_detected_features**: Extract vector geometry parsing buildings, pools, vegetation, solar panels via automated CV features bounds
- **check_coverage_point**: Verify Nearmap capture boundaries matching geospatial point resolving temporal history arrays
- **check_coverage_polygon**: Verify internal aerial survey boundary masks checking imagery intersections across mapped polygons
- **get_dsm_elevation_tile**: Extract pixelated Digital Surface Model mapping topographic terrain and building peak heights
- **get_oblique_tile**: Retrieve oblique perspective 3D-angled imagery tiles pointing North, South, East, West locating structural targets
- **list_survey_dates**: Iterate chronological availability boundaries mapping all temporal captures crossing target nodes
- **get_survey_metadata**: Query explicitly bounded survey parameters finding GSD resolutions finding optical flight details
- **get_true_ortho_tile**: Retrieve lean-corrected true geometric top-down bounding layers capturing zero parallax alignments
- **get_vertical_tile**: Retrieve high-resolution vertical static nadir aerial imagery tiles tracking captured boundaries


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Nearmap (High-Res Aerial Imagery & AI)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get the latest high-res vertical imagery for coordinates '34.0522,-118.2437'"

**🤖 AI Agent:**
> Retrieving imagery… I've identified the tile coordinates for downtown Los Angeles at zoom level 20. The most recent survey was captured on Feb 12, 2026. Here is the vertical imagery URL for your inspection. Would you like me to check for AI-detected features at this location?

---

**👤 You:**
> "Detect all solar panels within a 100m radius of this point: [lat,lon]"

**🤖 AI Agent:**
> Running AI feature extraction… I've identified 3 solar arrays within the specified radius. The detected features include high-confidence vector geometries. Array 1 covers approximately 45 sq meters. I can provide the full GeoJSON for these detections if you'd like.

---

**👤 You:**
> "Show me the oblique view from the North for this building coordinate"

**🤖 AI Agent:**
> Retrieving oblique perspective… I've fetched the perspective tile looking North for your target. This view clearly shows the structural facade and roof orientation. Would you like me to retrieve the South or East perspectives for a complete comparison?


## Installation & Usage

To install and use the **Nearmap (High-Res Aerial Imagery & AI)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nearmap-high-res-aerial-imagery-ai](https://vinkius.com/mcp/nearmap-high-res-aerial-imagery-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

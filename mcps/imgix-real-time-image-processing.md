# imgix (Real-time Image Processing) MCP Server

Optimize and transform images via imgix — manage CDN sources, purge assets, and monitor origin connections.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/imgix-real-time-image-processing)

## Overview
**Category:** developer-tools
**Tools Count:** 10

## Description
Connect your **imgix** account to any AI agent and take full control of your real-time image processing and CDN infrastructure through natural conversation.

### What you can do

- **Source Orchestration** — List, create, and configure imgix sources to connect your origin storage (S3, GCS, Web Folder) to the CDN directly from your agent
- **Cache Management** — Purge specific assets from the imgix Edge network to force a re-fetch of original files and invalidate all processed derivatives instantly
- **Asset Monitoring** — Enumerate files in your origin sources and retrieve metadata including file paths, sizes, and content types
- **Operational Control** — Enable or disable specific sources to manage traffic flow and deployment windows for your visual media
- **Source Audit** — Retrieve detailed configuration for existing sources, including deployment types, custom domains, and origin status
- **Infrastructure Management** — Permanently remove unused sources or update caching attributes to optimize your image delivery pipeline

### How it works

1. Subscribe to this server
2. Enter your imgix API Key
3. Start managing your image CDN from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Frontend Developers** — verify origin connections and purge processed image derivatives after asset updates without leaving your IDE
- **SREs & DevOps** — monitor source availability and manage CDN deployment states through natural conversation
- **Digital Asset Managers** — audit asset libraries and organize origin storage connections across multiple imgix projects


## Available Tools
- **list_sources**: List all Imgix sources. Imgix is an image CDN that optimizes, resizes, and transforms images in real-time via URL parameters
- **get_source**: Get details of an Imgix source. Returns name, domain, deployment type, and status
- **create_source**: Create a new Imgix source. Connects your origin (S3, GCS, web folder) to Imgix CDN
- **update_source**: Update an Imgix source configuration. Modify name, caching, or deployment settings
- **enable_source**: Deploy/enable an Imgix source. Makes it live and serving images
- **disable_source**: Undeploy/disable an Imgix source. Stops serving images
- **purge**: Purge an asset from Imgix CDN cache. Removes original and all derivatives, forcing re-fetch
- **list_assets**: List assets in an Imgix source. Returns file paths, sizes, and content types
- **get_asset**: Get metadata of a specific asset in Imgix. Returns path, size, content type
- **delete_source**: Delete an Imgix source permanently


## Installation & Usage

To install and use the **imgix (Real-time Image Processing)** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/imgix-real-time-image-processing](https://vinkius.com/mcp/imgix-real-time-image-processing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

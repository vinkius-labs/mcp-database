# Kraken.io MCP Server

Optimize, compress, and resize images via URL or direct upload using the Kraken.io API.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/krakenio)

## Overview
**Category:** productivity
**Tools Count:** 3

## Description
Connect **Kraken.io** to your AI agent to automate image processing. Reduce page load times and save storage space by compressing images with industry-leading algorithms.

### What you can do

- **URL Optimization** — Provide a link to any image and get an optimized version back instantly via the `optimize_url` tool
- **Direct Uploads** — Process base64 encoded images directly from your workflow using `upload_image` 
- **Smart Resizing** — Resize images to specific dimensions using various strategies (exact, portrait, landscape, etc.) during optimization
- **Quota Management** — Monitor your plan usage, total quota, and remaining balance with `get_user_status` 
- **Sandbox Testing** — Use the 'dev' mode to test your integration without consuming your paid quota

### How it works

1. Subscribe to this server
2. Enter your Kraken.io API Key and API Secret
3. Start optimizing images from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Web Developers** — automate image optimization in content workflows to improve Core Web Vitals
- **Content Managers** — ensure all uploaded assets are compressed and resized correctly without manual tools
- **Designers** — quickly generate web-ready versions of high-resolution assets through natural conversation


## Available Tools
- **get_user_status**: io account.

Get Kraken.io user status and quota
- **optimize_url**: io. Supports lossy/lossless compression, resizing, and format conversion.

Optimize an image from a URL
- **upload_image**: io.

Upload and optimize a base64 encoded image


## Installation & Usage

To install and use the **Kraken.io** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/krakenio](https://vinkius.com/mcp/krakenio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

# QuickChart MCP Server

Automate data visualization via QuickChart — generate charts, QR codes, barcodes, and word clouds directly from any AI agent.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/quickchart)

## Overview
**Category:** design-creative
**Tools Count:** 9

## Description
Connect **QuickChart** to your AI agent to transform raw data into professional visuals instantly. This server provides a comprehensive suite of tools for generating static images of charts, codes, and text visualizations.

### What you can do

- **Chart.js Rendering** — Generate high-quality Chart.js images (v2, v3, or v4) from JSON configurations using `get_chart_url` or `render_chart_post`.
- **QR Codes & Barcodes** — Create customized QR codes with logos and various barcode formats (UPC, EAN, Code128) using `get_qr_url` and `get_barcode_url`.
- **Word Clouds** — Transform text blocks into beautiful word cloud images with custom fonts and colors via `get_wordcloud_url`.
- **Short URLs** — Generate permanent, shareable links for your visualizations with `create_chart_short_url`.
- **Complex Rendering** — Handle large datasets and complex configurations using POST requests to avoid URL length limits.

### How it works

1. Subscribe to this server
2. (Optional) Enter your QuickChart API Key for higher rate limits
3. Start generating visuals from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — quickly visualize trends and distributions without leaving the chat interface
- **Developers** — generate barcodes or QR codes for documentation or testing on the fly
- **Marketers** — create word clouds from customer feedback or social media text for reports


## Available Tools
- **create_chart_short_url**: js configuration.

Generate a permanent short URL for a chart
- **get_barcode_url**: Construct a GET URL for a barcode image
- **get_chart_url**: Best for simple charts.

Construct a GET URL for a chart image
- **get_graphviz_url**: Construct a GET URL for a GraphViz diagram
- **get_qr_url**: Construct a GET URL for a QR code image
- **get_wordcloud_url**: Construct a GET URL for a word cloud image
- **render_apex_chart**: Render an Apex Chart and return as base64 data URI
- **render_chart_post**: js configurations that exceed URL length limits.

Render a complex chart and return as base64 data URI
- **render_google_chart**: Render a Google Chart and return as base64 data URI


## Installation & Usage

To install and use the **QuickChart** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/quickchart](https://vinkius.com/mcp/quickchart)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

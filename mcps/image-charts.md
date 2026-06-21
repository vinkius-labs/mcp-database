# Image-Charts MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/image-charts)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/image-charts-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/image-charts-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Generate professional charts, graphs, and QR codes instantly — transform raw data into high-quality images directly within your AI conversations.

## Description
Connect **Image-Charts** to your AI agent to visualize data on the fly. Whether you need a quick bar chart for a report or a complex radar chart for performance analysis, this server provides the tools to render data into beautiful, embeddable images.

### What you can do

- **Instant Visualization** — Generate GET URLs for quick charts like pie, bar, line, and scatter plots using standard parameters.
- **Handle Large Datasets** — Use POST requests to render charts when your data exceeds the 2KB URL limit, receiving a Base64 image response.
- **QR Code Generation** — Create high-quality QR codes for URLs, text, or contact information instantly.
- **Deep Customization** — Control every aspect of your charts, including colors, labels, legends, axis styles, and even animations (GIF).
- **Retina & Vector Support** — Output in PNG, SVG, or GIF formats with optional high-resolution Retina support for crisp displays.

### How it works

1. Subscribe to this server
2. Enter your Image-Charts Account ID and Secret Key
3. Ask your AI to visualize any dataset or generate a QR code

No more manual exporting of data to spreadsheet tools just to see a trend. Your AI now has a built-in graphics department.

### Who is this for?

- **Data Analysts** — quickly visualize query results without leaving the chat interface
- **Marketing Teams** — generate QR codes and campaign performance charts for instant review
- **Developers** — test chart configurations and styles during the prototyping phase


## Available Tools
- **generate_chart_url**: Best for standard charts with data under 2KB.

Generate a GET URL for an Image-Charts chart
- **render_chart_post**: Required for datasets exceeding the 2KB URL limit. Returns the image as a Base64 Data URI.

Render a chart via POST request and return Base64 image


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Image-Charts** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a pie chart showing sales: 40% North, 30% South, 20% East, 10% West."

**🤖 AI Agent:**
> I've generated the pie chart for you using `generate_chart_url`. You can view the sales distribution here: [Chart URL]

---

**👤 You:**
> "Create a QR code for the URL 'https://vurb.com' with size 200x200."

**🤖 AI Agent:**
> I've created the QR code for Vurb. Here is the link to the image: [QR Code URL]

---

**👤 You:**
> "Render a bar chart via POST for this dataset of 100 monthly values: [data...]"

**🤖 AI Agent:**
> Since the dataset is large, I've used `render_chart_post` to generate the image. Here is the visualization of your monthly data.


## Installation & Usage

To install and use the **Image-Charts** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/image-charts](https://vinkius.com/mcp/image-charts)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

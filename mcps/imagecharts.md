# ImageCharts MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/imagecharts)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/imagecharts-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/imagecharts-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [data-analytics](../categories/data-analytics.md)

Generate charts and graphs as images from URL parameters with a simple API that creates data visualizations on the fly.

## Description
Connect **ImageCharts** to any AI agent and generate data visualizations through natural conversation.

### What you can do

- **Bar Charts** — Generate vertical/horizontal bar charts with custom colors, labels, and data series
- **Pie Charts** — Create pie and doughnut charts with percentage labels
- **Line Charts** — Build trend charts with multiple data series and markers
- **Radar Charts** — Generate radar/spider charts for multi-dimensional comparisons
- **Bubble Charts** — Create scatter/bubble visualizations with size encoding
- **QR Codes** — Generate scannable QR codes from any text or URL

### How it works

1. Subscribe to this server
2. Optionally enter your ImageCharts API Key for watermark-free output
3. Start generating charts from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Data Analysts** — generate quick visualizations for reports and presentations
- **Developers** — embed chart images in applications, emails, or dashboards
- **Marketing** — create data-driven visuals for campaigns and social media


## Available Tools
- **generate_bar_chart**: Generate a bar chart image
- **generate_bubble_chart**: Generate a bubble chart image
- **generate_doughnut_chart**: Generate a doughnut chart image
- **generate_line_chart**: Generate a line chart image
- **generate_pie_chart**: Generate a pie chart image
- **generate_polar_area_chart**: Generate a polar area chart image
- **generate_qr_code**: Generate a QR code image
- **generate_radar_chart**: Generate a radar chart image
- **generate_scatter_plot**: Generate a scatter plot image
- **generate_venn_diagram**: Generate a Venn diagram image


## 💬 Prompt Examples

Here are some examples of how you can interact with the **ImageCharts** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a bar chart showing Q1-Q4 revenue and a pie chart of market share."

**🤖 AI Agent:**
> Bar chart generated! Revenue Q1-Q4: Q1 ($120K), Q2 ($145K), Q3 ($190K), Q4 ($210K). Colors: blue gradient. Size: 600x400px. Image URL ready for embedding. Pie chart generated! Market share: Product A (42%, blue), Product B (28%, green), Product C (18%, orange), Others (12%, gray). Size: 500x500px. Both charts ready for download or embedding.

---

**👤 You:**
> "Generate a QR code for our website and a line chart of monthly user growth."

**🤖 AI Agent:**
> QR code generated! Content: https://company.com. Size: 300x300px. Error correction: Medium. Scannable and ready for print. Line chart generated! Monthly users (Jan-Jun): Jan (1.2K), Feb (1.5K), Mar (2.1K), Apr (2.8K), May (3.4K), Jun (4.1K). Growth trend: +242% over 6 months. Colors: teal with markers.

---

**👤 You:**
> "Create a radar chart comparing 5 team skills and a bubble chart of project priorities."

**🤖 AI Agent:**
> Radar chart generated! Team skills: Frontend (85%), Backend (92%), DevOps (70%), Design (65%), Testing (78%). Shape shows strong backend with design as growth area. Bubble chart generated! Projects: 'Alpha' (high impact, low effort, large team), 'Beta' (medium impact, high effort, small team), 'Gamma' (low impact, low effort, medium team). Bubble size = team size. Both charts ready.


## Installation & Usage

To install and use the **ImageCharts** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/imagecharts](https://vinkius.com/mcp/imagecharts)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

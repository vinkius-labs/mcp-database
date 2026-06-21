# Pixabay MCP Server

Search and retrieve royalty-free stock images, vectors, illustrations, and videos via AI directly from Pixabay.

[![View on Vinkius](https://img.shields.io/badge/View_on-Vinkius-blue?style=for-the-badge)](https://vinkius.com/mcp/pixabay)

## Overview
**Category:** design-creative
**Tools Count:** 10

## Description
Connect the **Pixabay** massive media library natively to your AI agent. Access over 4.5 million high-quality, royalty-free stock photos, illustrations, vector graphics, and video clips for commercial use without ever opening a browser.

### What you can do

- **Deep Media Search** — Query photos, illustrations, and SVG vectors directly. Instruct the AI to filter strictly by "Editors Choice" or "Safe Search".
- **Video Assets** — Fetch MP4 video clips natively, returning multiple resolutions and exact durations for editing suites.
- **Parametric Lookups** — Find exactly what you need by instructing your agent to filter by orientation (horizontal/vertical), dominant colors, or deep topological categories (backgrounds, architecture, science).
- **Direct Payloads** — Given a media ID, the agent resolves high-resolution CDN download URLs instantly.

### How it works

1. Subscribe to this server
2. Provide your free Pixabay API Key
3. Start fetching media assets natively in Cursor, Claude, or any MCP client

### Who is this for?

- **Content Creators** — retrieve engaging background illustrations or B-roll MP4s instantly for blogs and social networks.
- **Frontend Developers** — mock up entire websites with high-res placeholder imagery filtered seamlessly by dominant hex colors.
- **Designers** — discover curated vector SVGs mapping directly to specific project themes and vertical canvas sizes.


## Available Tools
- **search_images**: Search Pixabay free stock images. Over 4.5M photos, illustrations, vectors. Returns IDs, preview URLs, page URL, tags, dimensions, downloads, and likes. Pixabay license allows free commercial use. Instructions: Pass query, page, per_page (max 200), image_type (all/photo/illustration/vector)
- **search_illustrations**: Search Pixabay illustrations. Drawings, digital art, and clipart
- **search_vectors**: Search Pixabay vector graphics. Scalable SVG art, icons, and infographics
- **search_videos**: Search Pixabay free stock videos. Returns video IDs, sizes, durations, and download URLs at multiple resolutions
- **search_by_category**: Search Pixabay by content category. Categories: backgrounds, fashion, nature, science, education, feelings, health, people, religion, places, animals, industry, computer, food, sports, transportation, travel, buildings, business, music
- **search_by_color**: Search Pixabay by dominant color. Instructions: Pass comma-separated colors (e.g. "red,yellow" or "grayscale,transparent")
- **search_editors_choice**: Search Pixabay editors choice images. Hand-picked premium quality selection
- **search_safe_content**: Search Pixabay with safe search enabled. Filters inappropriate content
- **search_by_orientation**: Search Pixabay by image orientation. Instructions: Pass horizontal, vertical, or all
- **get_image**: Get Pixabay image by ID. Returns full details, tags, and download URLs


## Installation & Usage

To install and use the **Pixabay** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pixabay](https://vinkius.com/mcp/pixabay)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---
*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

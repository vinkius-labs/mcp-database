# Pixabay MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pixabay)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Search and retrieve royalty-free stock images, vectors, illustrations, and videos via AI directly from Pixabay.

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


## Available Tools (10)
- **search_vectors**: Search Pixabay vector graphics. Scalable SVG art, icons, and infographics
- **search_videos**: Search Pixabay free stock videos. Returns video IDs, sizes, durations, and download URLs at multiple resolutions
- **search_by_category**: Search Pixabay by content category. Categories: backgrounds, fashion, nature, science, education, feelings, health, people, religion, places, animals, industry, computer, food, sports, transportation, travel, buildings, business, music
- **search_by_color**: Search Pixabay by dominant color. Instructions: Pass comma-separated colors (e.g. "red,yellow" or "grayscale,transparent")
- **search_editors_choice**: Search Pixabay editors choice images. Hand-picked premium quality selection
- **search_safe_content**: Search Pixabay with safe search enabled. Filters inappropriate content
- **search_by_orientation**: Search Pixabay by image orientation. Instructions: Pass horizontal, vertical, or all
- **get_image**: Get Pixabay image by ID. Returns full details, tags, and download URLs
- **search_images**: Search Pixabay free stock images. Over 4.5M photos, illustrations, vectors. Returns IDs, preview URLs, page URL, tags, dimensions, downloads, and likes. Pixabay license allows free commercial use. Instructions: Pass query, page, per_page (max 200), image_type (all/photo/illustration/vector)
- **search_illustrations**: Search Pixabay illustrations. Drawings, digital art, and clipart


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pixabay** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Find 5 editors choice photos showing coffee."

**🤖 AI Agent:**
> I retrieved 5 premium Editors Choice images for 'coffee'. Result `ID: 153068` features an aerial shot with 2.4k likes matching your description. Would you like the raw CDN string for the high-resolution backdrop (3000x2000)?

---

**👤 You:**
> "Search for transparent SVG vectors of a rocket ship."

**🤖 AI Agent:**
> Searching the vector graphics registry… I found `ID: 1475510` (Space Rocket Vector SVG) matching transparent backgrounds closely. The file is lightweight format (Scaleable Vector). Let me know if you want the exact layout attributes and download link.

---

**👤 You:**
> "Give me a vertical mountain video for an Instagram reel background."

**🤖 AI Agent:**
> Executing video lookup targeted for mobile devices. Found `ID: 329004` (Drone over Alps). It spans exactly 15 seconds, available native dimension mapping 1080x1920 MP4 (`8mb filesize`). Shall I construct a snippet that mounts this locally?


## ❓ FAQ

**Q: Can my AI download and directly embed high-resolution MP4 video URLs into my code?**
Yes. Instruct the agent to run a video search (`search_videos`). The JSON returned points mapping precisely to the highest resolution native CDN endpoints. Your AI agent can ingest these exact `mp4` URI addresses and format them perfectly into `<video>` tags inside your application mockup.

**Q: How can I easily discover only landscape photos related to 'urban night' containing mainly orange?**
The integration exposes distinct analytical endpoints natively. You simply prompt: 'Search Pixabay for urban night landscape containing orange'. The agent internally invokes the pixel-color mapping API (`search_by_color`) bounded by the (`horizontal`) orientation constraint to drastically minimize latency and fetch the literal perfect image.

**Q: Are there licensing restrictions when generating code using these results?**
No. All media assets managed by the Pixabay integration carry the pure royalty-free license. They are completely safe for commercial use, client mockups, and public deployment without explicit attribution, meaning you don't face unexpected DMCA copyright claims when your agent auto-selects dummy data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pixabay](https://vinkius.com/mcp/pixabay)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pixabay** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pixabay` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pixabay** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pixabay": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

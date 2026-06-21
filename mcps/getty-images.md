# Getty Images MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/getty-images)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Manage stock media via Getty Images — search millions of creative and editorial photos, handle video discovery, and download assets directly from any AI agent.

## Description
Connect your **Getty Images** account to any AI agent and take full control of your stock media research and asset procurement through natural conversation.

### What you can do

- **Stock Media Orchestration** — Search over 500M editorial and creative images to retrieve asset IDs, titles, and preview URLs natively within your chat
- **Creative Discovery** — Identify bounded creative images pre-filtered for commercial, advertising, and marketing use flawlessly
- **Editorial Auditing** — Search across news, sports, entertainment, and archival photography to track specific historical events and global trends synchronousy
- **Video Library Management** — Browse stock video libraries and retrieve duration, aspect ratio, and available resolution metadata securely
- **Visual Similarity Search** — Find visually similar assets by providing source IDs to discover related compositions and aesthetic patterns natively
- **Lightbox Collection Oversight** — List and manage your Lightbox collections to organize selected assets across different projects limitlessly
- **Asset Procurement** — Execute direct download mutations to consume corporate quota limits and retrieve high-resolution download URLs securely

### How it works

1. Subscribe to this server
2. Enter your Getty Images API Key (found in the Getty Developer Portal)
3. Start managing your stock media from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators & Editors** — search for high-quality stock photos and videos using natural language without leaving the creative workflow
- **Marketers** — quickly find commercially-safe images for campaigns and manage project lightboxes in real-time
- **Journalists & Researchers** — search editorial and archival photography to verify historical events through natural conversation
- **Designers** — discover visually similar assets and audit video metadata directly from the chat interface


## Available Tools (10)
- **search_images**: Returns asset IDs, titles, captions, preview URLs. Pass phrase and page.

Search Getty Images stock photos
- **search_creative**: Search Getty creative (commercial-use) images only
- **search_editorial**: Not for commercial use.

Search Getty editorial images
- **get_image**: Get full details of a Getty image
- **get_images_batch**: Get details for multiple Getty images at once
- **search_videos**: Search Getty stock videos
- **get_video**: Get full details of a Getty video
- **download_image**: Returns download URL and consumes corporate quota limits. Pass asset ID.

Download a Getty image
- **get_similar**: Find visually similar Getty images
- **list_collections**: List your Getty lightbox collections


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Getty Images** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for creative images of 'modern sustainable architecture'"

**🤖 AI Agent:**
> Searching creative library... I found several high-quality images of sustainable buildings with solar panels and vertical gardens. Would you like to see the preview URLs and asset IDs for these?

---

**👤 You:**
> "Find visually similar images to asset '12345678'"

**🤖 AI Agent:**
> Analyzing visual properties... I found 5 similar assets with matching aesthetic patterns and compositions. I can provide the titles and artist names for these related images.

---

**👤 You:**
> "List my Getty lightboxes"

**🤖 AI Agent:**
> Retrieving collections... You have 3 active lightboxes: 'Q2 Web Campaign', 'Social Media Assets', and 'Inspiration Board'. Which one would you like to explore for selected assets?


## ❓ FAQ

**Q: Can my agent search only for commercially safe images in Getty?**
Yes. Use the 'search_creative' tool. It pre-filters results for commercial, advertising, and marketing use, ensuring the assets you discover are commercially safe natively.

**Q: How do I download an image through the agent?**
Use the 'download_image' tool. Provide the Asset ID. Note that this requires an active subscription and will consume your corporate quota. The agent will return a secure download URL synchronously.

**Q: Can I find images similar to one I already liked through the agent?**
Absolutely. Use the 'get_similar' tool. Provide the ID of your source image, and the agent will analyze its visual properties to find related compositions and aesthetic patterns within Getty's library.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/getty-images](https://vinkius.com/mcp/getty-images)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Getty Images** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `getty-images` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Getty Images** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "getty-images": {
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

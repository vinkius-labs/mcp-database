# Pixabay MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pixabay-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Search and retrieve millions of royalty-free images and videos directly from Pixabay's massive creative library.

## Description
Connect your **Pixabay** account to any AI agent to instantly source high-quality, royalty-free media for your projects through simple natural language commands.

### What you can do

- **Image Discovery** — Search through millions of photos, illustrations, and vector graphics with precise filters for category, color, and orientation.
- **Video Search** — Find professional film clips and animations for your video editing or web projects.
- **Curated Quality** — Use the Editor's Choice filter to retrieve only the highest-rated assets vetted by the Pixabay community.
- **Safe Browsing** — Enable SafeSearch filters to ensure all returned media is appropriate for all audiences.
- **Technical Precision** — Filter results by minimum dimensions, image types, and specific ordering (popular vs. latest).

### How it works

1. Subscribe to this server
2. Enter your Pixabay API Key
3. Start searching for media from Claude, Cursor, or any MCP-compatible client

Stop wasting time manually browsing stock sites. Let your AI find the perfect visual asset while you stay in your creative flow.

### Who is this for?

- **Content Creators & Marketers** — Find the perfect blog header or social media image in seconds.
- **Designers** — Source vectors and illustrations directly within your design environment.
- **Developers** — Quickly populate prototypes and applications with high-quality placeholder or production media.


## Available Tools (2)
- **search_images**: Search for images on Pixabay
- **search_videos**: Search for videos on Pixabay


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pixabay** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Search for high-quality photos of futuristic cities in nature with a horizontal orientation."

**🤖 AI Agent:**
> I've found several stunning horizontal photos of futuristic cities integrated with nature. Here are the top results from Pixabay, including a lush green metropolis and a sustainable urban landscape.

---

**👤 You:**
> "Find vertical vector illustrations of coffee beans for a mobile app design."

**🤖 AI Agent:**
> I've retrieved vertical vector illustrations of coffee beans. These are perfect for mobile layouts and can be scaled without losing quality. Would you like to see the direct download links?

---

**👤 You:**
> "Search for Editor's Choice videos of ocean waves or surfing."

**🤖 AI Agent:**
> I've filtered for the best cinematic clips of ocean waves and surfing awarded with Editor's Choice. I found 3 high-quality films showing slow-motion breaks and professional surfing footage.


## ❓ FAQ

**Q: Can I filter specifically for illustrations or vector graphics instead of photos?**
Yes! When using the `search_images` tool, you can set the `image_type` parameter to 'illustration' or 'vector' to narrow down your results to specific artistic formats.

**Q: How do I ensure I only get the highest quality images recommended by Pixabay?**
You can set the `editors_choice` parameter to `true` in both `search_images` and `search_videos` tools. This filters the results to show only assets that have received the Editor's Choice award.

**Q: Is it possible to search for videos and animations as well?**
Absolutely. Use the `search_videos` tool to find video clips. You can further filter by `video_type` to choose between 'film' (live action) or 'animation'.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pixabay-alternative](https://vinkius.com/mcp/pixabay-alternative)
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
3. Set Type to "SSE" (or "streamable HTTP"), enter `pixabay-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pixabay** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pixabay-alternative": {
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

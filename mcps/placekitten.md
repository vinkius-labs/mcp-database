# PlaceKitten MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/placekitten)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Generate placeholder kitten images of any size for your design mockups and creative projects.

## Description
Connect to **PlaceKitten** to instantly generate adorable placeholder images for your web and design projects. Whether you need specific dimensions for a UI layout or a grayscale image for a minimalist aesthetic, this server provides quick access to high-quality kitten photos.

### What you can do

- **Custom Dimensions** — Request kitten images with precise width and height in pixels using the `get_kitten` tool.
- **Grayscale Effects** — Generate black and white kitten placeholders using `get_grayscale_kitten` to match specific design themes.
- **Design Mockups** — Quickly fill empty image slots in your prototypes without leaving your AI assistant or code editor.

### How it works

1. Subscribe to this server
2. Since PlaceKitten is a public service, no specific API key is required (simply enter 'public' if prompted)
3. Start requesting kitten images directly in your conversation

### Who is this for?

- **Frontend Developers** — test image containers and responsive layouts with real images
- **UI/UX Designers** — create more engaging wireframes and high-fidelity mockups
- **Prototypers** — quickly visualize content flow with varied image sizes


## Available Tools (2)
- **get_grayscale_kitten**: Get a grayscale kitten image
- **get_kitten**: Get a basic kitten image


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PlaceKitten** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get a kitten image 400 pixels wide and 300 pixels high."

**🤖 AI Agent:**
> I've generated a 400x300 kitten image for you: https://placekitten.com/400/300

---

**👤 You:**
> "I need a grayscale kitten placeholder, 500x500 pixels."

**🤖 AI Agent:**
> Here is a 500x500 grayscale kitten image for your project: https://placekitten.com/g/500/500

---

**👤 You:**
> "Show me a kitten image that is 800x200 for a website banner."

**🤖 AI Agent:**
> I've fetched an 800x200 kitten image suitable for a banner: https://placekitten.com/800/200


## ❓ FAQ

**Q: How do I get a kitten image with specific dimensions?**
Use the `get_kitten` tool and provide the desired `width` and `height` in pixels. The agent will return a URL to a kitten image matching those exact dimensions.

**Q: Can I generate black and white kitten images for my design?**
Yes! Use the `get_grayscale_kitten` tool. It works just like the standard tool but applies a grayscale filter to the image, perfect for minimalist or wireframe designs.

**Q: Is an API key required to use PlaceKitten?**
No, PlaceKitten is a free public service. You don't need to create an account or generate a token. Simply connect the server and start using it.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/placekitten](https://vinkius.com/mcp/placekitten)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PlaceKitten** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `placekitten` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PlaceKitten** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "placekitten": {
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

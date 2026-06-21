# PlaceDog MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/placedog)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Generate dog placeholder images with custom dimensions for your design and development projects.

## Description
Connect to **PlaceDog** to instantly generate high-quality dog placeholder images for your mockups, websites, or presentations through natural conversation.

### What you can do

- **Custom Dimensions** — Specify exact width and height in pixels for your placeholder needs
- **Instant URLs** — Get direct JPEG links to cute dog images ready for immediate use in your code or design tools
- **Design Workflow** — Speed up your UI/UX prototyping by fetching assets directly from your AI agent without searching manually

### How it works

1. Subscribe to this server
2. This service is public and does not require a personal API key
3. Start generating dog images by asking for specific dimensions

No more searching through stock photo sites for simple placeholders. Your AI acts as a quick asset generator for your frontend development needs.

### Who is this for?

- **Frontend Developers** — quickly populate image tags with realistic placeholders during component building
- **UI/UX Designers** — generate assets for wireframes and high-fidelity mockups instantly
- **Content Managers** — create visual guides for layout planning using temporary dog images


## Available Tools
- **get_dog_image**: Get a dog placeholder image


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PlaceDog** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a dog image with 400px width and 300px height."

**🤖 AI Agent:**
> I've generated a 400x300 dog placeholder for you. You can view it here: https://place.dog/400/300

---

**👤 You:**
> "I need a square dog placeholder of 500x500 pixels."

**🤖 AI Agent:**
> Here is a 500x500 square dog image for your design: https://place.dog/500/500

---

**👤 You:**
> "Get a dog image for a 800x400 banner."

**🤖 AI Agent:**
> I've fetched a 800x400 dog image for your banner. URL: https://place.dog/800/400


## ❓ FAQ

**Q: Can I specify the exact size of the dog image?**
Yes! Use the `get_dog_image` tool and provide the `width` and `height` in pixels. The agent will return a URL to a JPEG image matching those exact dimensions.

**Q: What kind of images does this server provide?**
It provides high-quality JPEG placeholder images of dogs, perfect for web development, UI design mockups, and layout testing.

**Q: Do I need an account or API key to use PlaceDog?**
No, PlaceDog is a free public service. You can start using the `get_dog_image` tool immediately without any registration or private credentials.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/placedog](https://vinkius.com/mcp/placedog)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PlaceDog** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `placedog` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PlaceDog** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "placedog": {
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

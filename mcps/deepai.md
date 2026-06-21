# DeepAI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/deepai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Generate and edit images using AI — create art from text, remove backgrounds, colorize photos, and upscale images directly from your AI agent.

## Description
Connect **DeepAI** to your AI agent to unlock powerful image generation and manipulation capabilities through natural language.

### What you can do

- **Text-to-Image** — Generate high-quality images from descriptions using various models like HD, Genius, and Super Genius.
- **Background Removal** — Instantly strip backgrounds from any image URL using advanced AI segmentation.
- **Image Editing** — Modify existing images by describing changes in plain text (e.g., 'make the sky red').
- **Colorization** — Bring old black and white photos to life with realistic AI-powered coloring.
- **Super Resolution** — Upscale and sharpen low-resolution images without losing detail or quality.

### How it works

1. Subscribe to this server
2. Enter your DeepAI API Key
3. Start creating and editing visuals from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Content Creators** — Generate unique visuals for blogs and social media without leaving your workflow.
- **Designers** — Quickly iterate on concepts, remove backgrounds, or upscale assets using AI commands.
- **Developers** — Integrate image processing tasks directly into your coding environment or agent-led projects.


## Available Tools
- **colorize_image**: Adds color to black and white or historic images
- **edit_image**: Modifies images based on text prompts
- **remove_background**: Removes the background from an image using AI
- **super_resolution**: Upscales and sharpens images without losing quality
- **generate_image**: Create an image from a text description


## 💬 Prompt Examples

Here are some examples of how you can interact with the **DeepAI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an image of a cyberpunk coffee shop in 4k using the super_genius model."

**🤖 AI Agent:**
> I've generated your cyberpunk coffee shop image using the Super Genius model at 4k resolution. You can view it here: [URL]

---

**👤 You:**
> "Remove the background from this product photo: https://example.com/photo.jpg"

**🤖 AI Agent:**
> Processing background removal... Done! Here is your image with a transparent background: [URL]

---

**👤 You:**
> "Colorize this historic black and white photo: https://example.com/history.jpg"

**🤖 AI Agent:**
> I've applied AI colorization to the photo. The colorized version is available here: [URL]


## ❓ FAQ

**Q: Can I choose different quality levels for image generation?**
Yes! The `generate_image` tool allows you to specify `image_generator_version` such as 'standard', 'hd', 'genius', or 'super_genius' to match your needs.

**Q: How do I improve the quality of a blurry or small image?**
Use the `super_resolution` tool. Just provide the image URL, and the AI will upscale and sharpen it while preserving details.

**Q: Is it possible to edit an image using only text commands?**
Absolutely. With the `edit_image` tool, you provide a base image URL and a text prompt describing the changes you want to see.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/deepai](https://vinkius.com/mcp/deepai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **DeepAI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `deepai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **DeepAI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "deepai": {
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

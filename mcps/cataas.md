# CatAAS MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/cataas)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/cataas-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/cataas-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Access the Cat as a Service (CATAAS) API to fetch random cat images, GIFs, and create custom cat memes with filters and text.

## Description
Bring the joy of cats to your AI interactions with the **CatAAS** MCP server. This integration allows any AI agent to fetch, filter, and customize cat images and GIFs directly from the CATAAS library.

### What you can do

- **Random Cats & GIFs** — Instantly fetch random cat images or animated GIFs to brighten your day or UI.
- **Tag Filtering** — Search for specific types of cats (e.g., 'orange', 'cute', 'sleeping') using the extensive tagging system.
- **Custom Text Overlays** — Create instant memes by overlaying custom text on cat images with adjustable fonts and colors.
- **Visual Filters** — Apply professional filters like blur, mono, or negate, and fine-tune brightness, saturation, and hue.
- **Metadata Exploration** — List all available tags and cat entries to discover the perfect visual for your needs.

### How it works

1. Subscribe to this server
2. Configure your access (no complex setup required)
3. Start requesting cats from Claude, Cursor, or any MCP client

### Who is this for?

- **Developers** — Add fun placeholders or dynamic cat content to applications during development.
- **Content Creators** — Quickly generate cat memes and visual assets using natural language.
- **Teams** — Lighten the mood in collaborative environments with random cat GIFs and images.


## Available Tools
- **get_cat_by_tag**: Get a random cat filtered by tag
- **get_cat_with_tag_and_text**: Get a random cat with a specific tag and custom text
- **get_cat_with_text**: Get a random cat with custom text overlaid
- **get_random_cat**: Get a random cat image metadata
- **get_random_gif_cat**: Get a random animated cat GIF
- **list_cats**: List cats from the database
- **list_tags**: List all available tags


## 💬 Prompt Examples

Here are some examples of how you can interact with the **CatAAS** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Get a random cat image with a 'blur' filter."

**🤖 AI Agent:**
> I've fetched a blurred cat image for you. [Image ID: 596e421d844c04001011cc98]

---

**👤 You:**
> "Show me a cat with the tag 'orange' saying 'I am hungry'."

**🤖 AI Agent:**
> Here is an orange cat with your custom text overlay. [Image ID: 596e421f844c04001011cc9a]

---

**👤 You:**
> "List all available cat tags."

**🤖 AI Agent:**
> I've retrieved the tags. Popular ones include 'cute', 'orange', 'sleeping', 'black', and 'funny'. There are hundreds more available!


## Installation & Usage

To install and use the **CatAAS** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/cataas](https://vinkius.com/mcp/cataas)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

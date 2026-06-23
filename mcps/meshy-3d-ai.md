# Meshy (3D AI) MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/meshy-3d-ai)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Transform text and images into high-quality 3D models using Meshy's generative AI directly from your agent.

## Description
Connect **Meshy** to your AI agent to bridge the gap between 2D concepts and 3D reality. This server allows you to generate, refine, and optimize professional-grade 3D meshes using industry-leading AI models.

### What you can do

- **Text to 3D Generation** — Create 3D previews from simple text prompts and refine them into fully textured models with PBR maps.
- **Image to 3D Conversion** — Turn single or multiple reference images (up to 4 angles) into detailed 3D objects automatically.
- **Advanced Retexturing** — Apply entirely new styles to existing 3D models using text or image guidance while maintaining geometry.
- **Mesh Optimization** — Use the remeshing tools to adjust topology (triangles or quads) and target specific polycounts for games or web apps.
- **Asset Management** — List, retrieve, and manage your generation tasks and 3D assets through a unified interface.

### How it works

1. Subscribe to this server
2. Enter your Meshy API Key
3. Start creating 3D assets in Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Game Developers** — Generate base meshes and textures directly within your development environment to speed up prototyping.
- **3D Artists** — Automate the tedious parts of the workflow like initial block-outs, UV mapping, and base texturing.
- **Creative Agencies** — Rapidly visualize 3D concepts for clients starting from just a text description or a sketch.


## Available Tools (17)
- **create_text_to_image**: Create Text to Image task
- **delete_text_to_3d_task**: Delete a Text to 3D task
- **get_balance**: Get account balance
- **get_text_to_3d_task**: Get a Text to 3D task by ID
- **list_text_to_3d_tasks**: List Text to 3D tasks
- **repair_printability**: Repair 3D Printability
- **analyze_printability**: Analyze 3D Printability
- **create_animation**: Create an Animation task
- **create_image_to_3d**: Create an Image to 3D task
- **create_image_to_image**: Create Image to Image task
- **create_multi_color_print**: Create Multi-Color Print
- **create_multi_image_to_3d**: Create a Multi-Image to 3D task
- **create_remesh**: Create a Remesh task
- **create_retexture**: Create a Retexture task
- **create_rigging**: Create a Rigging task
- **create_text_to_3d_preview**: This is the first step in the Text to 3D workflow.

Create a Text to 3D preview task
- **create_text_to_3d_refine**: This is the second step in the Text to 3D workflow.

Create a Text to 3D refine task


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Meshy (3D AI)** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Create a 3D preview of a futuristic cyberpunk motorcycle."

**🤖 AI Agent:**
> I've initiated the `create_text_to_3d_preview` task for your cyberpunk motorcycle. The task ID is 'msy_abc123'. I'll let you know as soon as the preview mesh is ready.

---

**👤 You:**
> "Generate a 3D model from this image: https://example.com/character.png"

**🤖 AI Agent:**
> Starting the `create_image_to_3d` process. I'm uploading the reference image to Meshy's AI to generate the geometry and textures. This usually takes a few minutes.

---

**👤 You:**
> "List my recent 3D generation tasks."

**🤖 AI Agent:**
> Fetching your history via `list_text_to_3d_tasks`... I found 3 recent models: a 'Sci-fi Crate' (Succeeded), a 'Stone Arch' (Succeeded), and a 'Dragon' (In Progress).


## ❓ FAQ

**Q: How do I add high-quality textures to a 3D model I just generated from text?**
After creating a preview with `create_text_to_3d_preview`, use the `create_text_to_3d_refine` tool with the resulting task ID. You can enable PBR and HD textures to get professional results.

**Q: Can I use multiple photos of an object to create a better 3D model?**
Yes! Use the `create_multi_image_to_3d` tool and provide an array of up to 4 image URLs showing different angles of the object for much higher accuracy.

**Q: Is it possible to reduce the polygon count for game engine optimization?**
Absolutely. Use the `create_remesh` tool on any existing model ID. You can specify the `target_polycount` and choose between `triangle` or `quad` topology.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/meshy-3d-ai](https://vinkius.com/mcp/meshy-3d-ai)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Meshy (3D AI)** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `meshy-3d-ai` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Meshy (3D AI)** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "meshy-3d-ai": {
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

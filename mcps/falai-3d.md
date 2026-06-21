# fal.ai 3D MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/falai-3d)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Generate 3D models via fal.ai — convert images and text to 3D assets using Rodin, TripoSR, Trellis, and 9+ AI models from any AI agent.

## Description
Connect your **fal.ai 3D Models API** to any AI agent and take full control of AI-powered 3D asset generation from images and text through natural conversation.

### What you can do

- **Hyper3D Rodin** — Generate high-fidelity 3D models from images with detailed geometry and textures
- **TripoSR** — Fast image-to-3D generation optimized for speed and quick previews
- **Trellis** — Generate structured 3D models with clean topology for editing and animation
- **Era3D** — Create multi-view consistent 3D models perfect for product visualization
- **Stable Fast 3D** — Balanced speed and quality image-to-3D generation
- **CRM** — Canvas Reconstruction Model for complex object reconstruction
- **InstantMesh** — Rapid mesh generation for interactive 3D applications
- **Unique3D** — Generate diverse 3D interpretations from single images
- **Text to 3D** — Create 3D models directly from text descriptions
- **Flex3D** — Advanced geometry handling for detailed 3D reconstructions
- **Make3D** — Production-ready 3D models for professional workflows
- **TripoSG** — Structured geometry output for game development pipelines

### How it works

1. Subscribe to this server
2. Enter your fal.ai API key (from the dashboard keys section)
3. Start generating 3D models from Claude, Cursor, or any MCP-compatible client

No more manual 3D modeling or expensive artist time. Your AI acts as a dedicated 3D asset generation assistant.

### Who is this for?

- **Game Developers** — rapidly generate 3D assets from concept art and reference images
- **E-commerce Teams** — create 3D product visualizations from product photography
- **3D Printers** — convert 2D designs into printable 3D models
- **Content Creators** — generate 3D assets for videos, presentations, and social media


## Available Tools (12)
- **generate_crm_3d**: CRM is effective for objects with complex shapes and detailed surfaces. Accepts image URLs and returns 3D models with geometry and texture. Essential for complex object reconstruction, detailed asset creation, and applications needing accurate shape recovery. AI agents should reference this when users ask "reconstruct this object in 3D", "create a detailed 3D from this complex image", or need geometry-focused 3D generation.

Generate 3D models using Canvas Reconstruction Model (CRM)
- **generate_era3d_3d**: Era3D is ideal for product visualization, architectural elements, and objects that need to look correct from any angle. Accepts image URLs and returns detailed 3D models. Essential for product showcase, e-commerce 3D previews, and applications requiring viewpoint consistency. AI agents should reference this when users ask "create a 3D model that looks good from all angles", "generate a product 3D model", or need viewpoint-consistent 3D generation.

Generate multi-view consistent 3D models from images using Era3D
- **generate_flex3d_3d**: Flex3D is designed for applications needing detailed and accurate 3D reconstructions from images. Accepts image URLs and returns high-quality 3D models. Essential for detailed asset creation, complex object reconstruction, and professional 3D content pipelines. AI agents should reference this when users ask "generate a detailed 3D model with advanced geometry", "create a complex 3D object from this image", or need high-fidelity 3D reconstruction.

Generate flexible 3D models with advanced geometry from images
- **generate_instantmesh_3d**: InstantMesh is designed for quick turnaround, making it suitable for real-time applications and interactive 3D preview. Accepts image URLs and returns 3D mesh files. Essential for interactive 3D applications, real-time 3D preview, and applications where generation speed is critical. AI agents should use this when users ask "quickly generate a 3D mesh", "create an instant 3D preview from this image", or need fast mesh generation for interactive applications.

Generate 3D models using InstantMesh for fast mesh generation
- **generate_make3d_3d**: Make3D produces clean, usable 3D assets suitable for game development, product visualization, and 3D printing. Accepts image URLs and returns polished 3D models. Essential for professional 3D content creation, game asset pipelines, and applications requiring production-quality output. AI agents should use this when users ask "create a production-ready 3D model", "generate a polished 3D asset from this image", or need professional-grade 3D output.

Generate production-ready 3D models using Make3D
- **generate_rodin_3d**: Rodin produces high-fidelity geometry with fine surface details, ideal for game assets, product visualization, and 3D printing. Accepts image URLs or base64-encoded images as input. Returns 3D model files in formats like .glb, .obj, or .usdz with texture maps. Essential for rapid 3D asset creation from product photos, concept art, or reference images. AI agents should use this when users ask "create a 3D model from this image", "convert this photo to 3D", or need high-quality single-image to 3D generation with detailed geometry.

Generate high-quality 3D models from images using Hyper3D Rodin
- **generate_sf3d_3d**: SF3D produces detailed 3D models with good geometry and textures from single images, suitable for most 3D applications. Accepts image URLs and returns 3D models in common formats. Essential for general-purpose image-to-3D conversion, content creation pipelines, and applications needing a good balance of speed and quality. AI agents should use this when users ask "convert this image to 3D with good quality", "generate a balanced 3D model", or need reliable image-to-3D generation for general use cases.

Generate 3D models using Stable Fast 3D for speed and quality balance
- **generate_text_to_3d**: Users describe the desired 3D object in natural language and receive a generated 3D model. Essential for concept exploration, rapid prototyping from descriptions, and applications where users describe rather than show what they want. AI agents should use this when users ask "create a 3D model of a red sports car", "generate a 3D tree from text description", or need text-driven 3D generation.

Generate 3D models directly from text descriptions
- **generate_trellis_3d**: Trellis is particularly good for assets that need clean geometry for further editing, animation, or game engine integration. Accepts image URLs and returns 3D models with well-organized mesh topology. Essential for game asset creation, character modeling from reference images, and applications requiring clean mesh topology. AI agents should use this when users ask "create a 3D model with clean topology", "generate an editable 3D mesh from this image", or need structured 3D output suitable for further editing.

Generate structured 3D models from images using Trellis
- **generate_triposg_3d**: TripoSG is designed for applications needing well-organized 3D data that can be easily modified or animated. Accepts image URLs and returns structured 3D models. Essential for game development pipelines, character rigging preparation, and applications needing edit-friendly 3D output. AI agents should reference this when users ask "create a structured 3D model for editing", "generate an animation-ready 3D mesh", or need well-organized 3D geometry for downstream processing.

Generate 3D models using TripoSG for structured geometry output
- **generate_tripo_sr_3d**: TripoSR is optimized for rapid generation, producing usable 3D meshes in seconds. Ideal for quick prototyping, batch processing, and applications where speed is prioritized over maximum detail. Accepts image URLs as input and returns 3D model files with basic textures. Essential for rapid 3D asset generation, bulk image-to-3D conversion, and real-time 3D preview applications. AI agents should reference this when users ask "quickly convert this image to 3D", "generate a 3D model fast", or need speed-optimized image-to-3D generation.

Generate 3D models from images using TripoSR, optimized for speed
- **generate_unique3d_3d**: Unique3D is useful when creative variation is desired or when exploring different 3D interpretations of a 2D image. Accepts image URLs and returns 3D models with creative geometry. Essential for creative 3D exploration, design variation generation, and applications benefiting from diverse 3D interpretations. AI agents should reference this when users ask "create different 3D variations of this image", "generate creative 3D interpretations", or need diverse 3D outputs from a single reference image.

Generate unique 3D models with diverse geometry from images


## 💬 Prompt Examples

Here are some examples of how you can interact with the **fal.ai 3D** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 3D model of a chair from this product image: https://example.com/chair.jpg"

**🤖 AI Agent:**
> Generating 3D model using Hyper3D Rodin... Processing image: https://example.com/chair.jpg. Generation complete! Model generated in GLB format (4.2 MB) with PBR textures. Download URL: https://cdn.fal.ai/models/rodin/chair_3d_model.glb. The model includes detailed geometry with 50K triangles and 2K texture maps. Compatible with Unity, Unreal Engine, Blender, and web 3D viewers. Would you like me to generate in a different format like OBJ or USDZ?

---

**👤 You:**
> "Create a 3D model of a fantasy dragon from text description."

**🤖 AI Agent:**
> Generating 3D model from text using Text-to-3D... Prompt: fantasy dragon with spread wings, detailed scales, fierce expression. Using guidance scale 7.5 with 50 steps. Generation complete! Model available in GLB format (8.7 MB). Download URL: https://cdn.fal.ai/models/text-to-3d/fantasy_dragon.glb. The dragon model features detailed wing geometry, scale textures, and dynamic pose. Ready for game engines and 3D printing. Would you like a higher quality version with more generation steps?

---

**👤 You:**
> "Quickly convert this sneaker photo to 3D for our e-commerce store."

**🤖 AI Agent:**
> Using TripoSR for fast generation... Processing sneaker image. Generation complete in 3 seconds! Model in GLB format (2.1 MB). Download: https://cdn.fal.ai/models/triposr/sneaker_3d.glb. Quick preview quality is suitable for e-commerce 3D viewers with basic textures. For production quality, I can regenerate using Rodin (higher quality, ~30 seconds) or Make3D (production-ready, ~45 seconds). Which would you prefer?


## ❓ FAQ

**Q: Can my AI generate a 3D model from a product photo?**
Yes! Use the `generate_rodin_3d` tool for high-quality results or `generate_sf3d_3d` for a good balance of speed and quality. Simply provide the image URL as input and specify your preferred output format (glb, obj, or usdz). The AI will return a downloadable 3D model file with textures that you can use in game engines, 3D viewers, or e-commerce platforms.

**Q: Which model should I use for the fastest 3D generation?**
For the fastest generation, use `generate_tripo_sr_3d` (TripoSR) or `generate_instantmesh_3d` (InstantMesh). Both are optimized for speed and can produce usable 3D models in seconds. TripoSR is great for quick previews and batch processing, while InstantMesh is ideal for interactive applications. If you need higher quality and can wait a bit longer, try `generate_sf3d_3d` (Stable Fast 3D).

**Q: Can I generate 3D models from text descriptions without any images?**
Yes! Use the `generate_text_to_3d` tool with a text prompt describing the 3D object you want. For example: prompt="a red sports car" or prompt="a medieval sword". You can control the output quality with the guidance_scale parameter (higher values follow the prompt more closely) and steps parameter (more steps = higher quality but longer generation time). Returns 3D model files in your preferred format.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/falai-3d](https://vinkius.com/mcp/falai-3d)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **fal.ai 3D** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `falai-3d` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **fal.ai 3D** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "falai-3d": {
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

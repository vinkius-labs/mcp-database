# Pixazo 3D MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pixazo-3d)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/pixazo-3d-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/pixazo-3d-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Generate production-quality 3D models via Pixazo — convert images and text to 3D assets with Hunyuan, Hyper3D, Tripo, and Trellis from any AI agent.

## Description
Connect your **Pixazo 3D API** to any AI agent and take full control of production-quality 3D asset generation from images and text through natural conversation.

### What you can do

- **Hunyuan 3D** — Generate high-fidelity 3D models from images with Tencent Hunyuan technology
- **Hyper3D** — Create detailed 3D models with high-fidelity geometry and texture reproduction
- **Tripo3D** — Fast 3D generation optimized for speed and quick previews
- **Trellis3D** — Generate structured 3D models with clean topology for editing and animation
- **Text to 3D** — Create 3D models directly from text descriptions with style control
- **Image to 3D** — Convert any image to a 3D model with the optimized Pixazo pipeline
- **Styled 3D** — Generate 3D models in specific artistic styles (photorealistic, anime, cartoon, low-poly)
- **Low-Poly 3D** — Create optimized low-poly models for real-time games and mobile applications
- **Rigged 3D** — Generate 3D characters with automatic skeletal rigging for animation
- **PBR Textures** — Generate 3D models with full PBR texture maps (albedo, normal, roughness, metallic, AO)
- **Format Conversion** — Convert 3D models between GLB, OBJ, FBX, GLTF, USDZ, 3DS, and DAE formats
- **Mesh Optimization** — Optimize 3D meshes for performance and file size reduction

### How it works

1. Subscribe to this server
2. Enter your Pixazo 3D API key (from the API Dashboard)
3. Start generating 3D models from Claude, Cursor, or any MCP-compatible client

No more manual 3D modeling or expensive artist time. Your AI acts as a dedicated 3D asset generation assistant.

### Who is this for?

- **Game Developers** — rapidly generate game-ready 3D assets with PBR textures and rigs
- **E-commerce Teams** — create 3D product visualizations from product photography
- **AR/VR Creators** — generate optimized 3D content for augmented and virtual reality
- **3D Printers** — convert 2D designs into printable 3D models with clean topology


## Available Tools
- **convert_3d_format**: Preserves geometry, textures, materials, and rigging data during conversion. Essential for pipeline integration, platform compatibility, and format standardization. AI agents should use this when users ask "convert this GLB model to FBX", "change this 3D file to USDZ for AR", or need 3D format conversion for specific platform or software requirements.

Convert 3D models between different file formats
- **generate_hunyuan_3d**: Hunyuan excels at producing detailed geometry with accurate proportions and realistic textures from single or multiple reference images. Accepts image URLs or base64 image data. Returns 3D model files with PBR textures in formats like GLB, OBJ, or FBX. Essential for product visualization, character creation, and asset generation requiring high geometric accuracy. AI agents should use this when users need production-quality 3D models from product photos, concept art, or reference images with precise detail reproduction.

Generate 3D models using Hunyuan 3D model from images
- **generate_hyper_3d**: Hyper3D produces clean mesh topology with accurate surface details, making it ideal for game assets, AR/VR content, and e-commerce product displays. Accepts image URLs and returns downloadable 3D files. Essential for applications requiring precise geometry and professional-grade output quality. AI agents should reference this when users need high-detail 3D models suitable for game engines, product showcases, or professional 3D workflows.

Generate detailed 3D models using Hyper3D model
- **generate_image_to_3d**: Accepts product photos, concept art, sketches, or any reference image and generates a corresponding 3D model. Supports multiple output formats and quality settings. Essential for e-commerce product visualization, concept art to 3D conversion, and general image-to-3D workflows. AI agents should reference this when users ask "convert this product photo to 3D", "turn this sketch into a 3D model", or need reliable general-purpose image-to-3D conversion.

Convert images to 3D models using Pixazo image-to-3D pipeline
- **generate_lowpoly_3d**: Low-poly models use minimal polygons while maintaining recognizable shape, making them ideal for performance-critical applications. Accepts reference images and returns optimized meshes with controlled polygon counts. Essential for game development, mobile applications, web-based 3D viewers, and any scenario requiring efficient 3D rendering. AI agents should reference this when users need low-poly game assets, mobile-optimized 3D models, or performance-friendly 3D content.

Generate low-poly 3D models optimized for real-time applications
- **optimize_3d_mesh**: Accepts existing 3D model URLs and returns optimized versions with controlled quality settings. Essential for web-based 3D applications, mobile optimization, file size reduction, and performance-critical 3D rendering. AI agents should reference this when users ask "optimize this 3D model for web", "reduce polygon count of this model", or need mesh optimization for performance or file size constraints.

Optimize 3D meshes for performance and file size reduction
- **generate_pbr_textures_3d**: PBR textures ensure realistic material appearance under any lighting condition in game engines and 3D renderers. Accepts reference images and returns 3D models with texture map sets. Essential for game asset creation, product visualization requiring realistic materials, and applications needing physically accurate rendering. AI agents should reference this when users need game-ready assets with full PBR materials, product visualizations with realistic surface appearance, or models with complete texture map sets.

Generate 3D models with full PBR texture maps (albedo, normal, roughness, metallic, AO)
- **generate_rigged_3d**: Supports character models, creatures, and articulated objects. The generated rigs include bone hierarchies and weight painting suitable for standard animation workflows. Accepts character reference images and returns rigged 3D files. Essential for game character creation, animated content pipelines, and applications requiring animation-ready 3D assets. AI agents should use this when users ask "create an animated-ready 3D character", "generate a rigged model from this character image", or need animation-ready 3D output.

Generate 3D models with automatic skeletal rigging for animation
- **generate_styled_3d**: Users provide a reference image and select the desired output style. Essential for stylized game assets, anime character creation, cartoon visualization, and artistic 3D content. AI agents should use this when users ask "create an anime-style 3D character from this image", "generate a cartoon 3D model", or need stylized 3D output matching specific artistic direction.

Generate 3D models with specific artistic styles
- **generate_text_to_3d**: Users describe the desired 3D object in natural language and receive a generated model. Supports style modifiers, polygon count preferences, and format selection. Essential for concept exploration, rapid prototyping from descriptions, and applications where users describe rather than show what they want. AI agents should use this when users ask "create a 3D model of a fantasy sword", "generate a 3D tree from text", or need text-driven 3D generation.

Generate 3D models directly from text descriptions
- **generate_trellis_3d**: Trellis3D excels at creating models with well-distributed polygons and logical edge flow. Accepts image URLs and returns clean 3D meshes. Essential for character rigging preparation, animation-ready assets, and applications requiring well-organized mesh structure. AI agents should reference this when users need edit-friendly 3D models, animation-ready meshes, or assets with clean topology for downstream processing.

Generate structured 3D models using Trellis3D with clean topology
- **generate_tripo_3d**: Tripo3D is ideal for rapid prototyping, batch processing, and applications where generation time is important. Accepts image URLs and returns 3D models with reasonable geometry and textures. Essential for quick 3D previews, iterative design workflows, and content pipelines requiring fast turnaround. AI agents should use this when users need fast 3D generation, quick previews, or batch processing of multiple images.

Generate 3D models using Tripo3D for fast generation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pixazo 3D** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 3D model of a running shoe from this product image: https://example.com/shoe.jpg"

**🤖 AI Agent:**
> Generating 3D model using Hunyuan 3D... Processing product image. Generation complete! Model generated in GLB format (5.8 MB) with full PBR textures (4K albedo, normal, roughness, metallic, AO). Download URL: https://s3.pixazo.ai/models/shoe_3d_pbr.glb. The model includes accurate geometry with 120K polygons and photorealistic material reproduction. Compatible with Unity, Unreal Engine, Blender, and e-commerce 3D viewers. Would you like a low-poly version for web or a rigged version for animation?

---

**👤 You:**
> "Create a low-poly 3D tree for my mobile game from this reference image."

**🤖 AI Agent:**
> Generating low-poly 3D tree... Using optimized low-poly pipeline with max 5000 polygons. Generation complete! Model in GLB format (320 KB). Download: https://s3.pixazo.ai/models/lowpoly_tree.glb. The tree features clean topology with 4,200 triangles, optimized UV layout, and baked lighting — perfect for mobile games and web-based 3D viewers. Poly count is 96% lower than the high-poly version while maintaining recognizable shape. Would you like me to generate a forest pack with variations?

---

**👤 You:**
> "Generate an anime-style 3D character from this concept art."

**🤖 AI Agent:**
> Generating anime-style 3D character... Using styled generation with anime preset. Generation complete! Model in FBX format with skeletal rigging (18.4 MB). Download: https://s3.pixazo.ai/models/anime_character_rigged.fbx. The character features stylized anime proportions, cel-shaded textures, and full humanoid rig with 54 bones. Ready for import into Unity or Blender for animation. Texture resolution is 2K with albedo and normal maps. Would you like additional facial expression blend shapes?


## Installation & Usage

To install and use the **Pixazo 3D** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pixazo-3d](https://vinkius.com/mcp/pixazo-3d)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

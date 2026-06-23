# 3D AI Studio MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/3d-ai-studio)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-creative](../categories/design-creative.md)

Generate and process 3D models via 3D AI Studio — text-to-3D, image-to-3D, AI texturing, remeshing, rendering, and mesh tools from any AI agent.

## Description
Connect your **3D AI Studio API** to any AI agent and take full control of production-quality 3D generation, AI texturing, mesh processing, and rendering through natural conversation.

### What you can do

- **Text to 3D** — Generate 3D models from text prompts using Hunyuan 3D, TRELLIS.2, and Tripo models
- **Image to 3D** — Convert any image to a 3D model with multiple AI model options
- **Multi-View to 3D** — Generate accurate 3D models from multiple reference images
- **AI Texturing** — Apply AI-powered PBR texturing to existing models using text or image prompts
- **Remeshing** — Optimize topology with tri or quad mesh remeshing
- **Mesh Repair** — Fix non-manifold geometry, holes, and inverted normals
- **Format Conversion** — Convert between GLB, OBJ, FBX, STL, PLY, USDZ, and 3MF formats
- **Model Optimization** — Reduce polygon count and compress for web and mobile
- **3D Rendering** — Generate high-quality images and turntable videos up to 4K
- **Mesh Segmentation** — Automatically segment 3D mesh parts by semantic components
- **Texture Baking** — Bake high-poly details onto low-poly game-ready meshes
- **Volume Calculator** — Calculate volume, surface area, and weight estimates for 3D printing

### How it works

1. Subscribe to this server
2. Enter your 3D AI Studio API key (from the platform dashboard)
3. Start generating and processing 3D models from Claude, Cursor, or any MCP-compatible client

No more manual 3D modeling or expensive artist time. Your AI acts as a dedicated 3D generation and processing assistant.

### Who is this for?

- **Game Developers** — generate game-ready assets with AI texturing and optimized meshes
- **E-commerce Teams** — create 3D product visualizations and marketing renders
- **3D Printers** — repair meshes, calculate volumes, and convert to print-ready formats
- **Content Creators** — generate 3D assets and renders for videos and social media


## Available Tools (12)
- **generate_ai_texturing**: Can repaint or restyle existing 3D models with new materials, colors, and surface details. Generates complete PBR texture sets (albedo, normal, metallic, roughness) from descriptions like "rusty metal", "polished wood", or "cartoon stone". Essential for material iteration, style transfers on 3D assets, and adding surface details to generated models. AI agents should reference this when users ask "add rusty metal texture to this model", "restyle this character with cartoon textures", or need AI-powered material generation on existing 3D meshes.

Apply AI-powered PBR texturing to existing 3D models using text or image prompts
- **convert_3d_format**: Preserves geometry, textures, materials, and rigging data during conversion. Essential for pipeline integration, platform compatibility, and format standardization. AI agents should use this when users ask "convert this GLB model to FBX", "change this 3D file to STL for 3D printing", or need 3D format conversion for specific platform or software requirements.

Convert 3D models between different file formats
- **generate_image_to_3d**: 2-4B, and Tripo variants. Accepts product photos, concept art, sketches, or any reference image and generates a corresponding 3D model with PBR textures. Supports style modifiers, face limits, density presets, and orientation control. Returns 3D model files in multiple formats. Essential for e-commerce product visualization, concept art to 3D conversion, and general image-to-3D workflows. AI agents should reference this when users ask "convert this product photo to 3D", "turn this sketch into a 3D model", or need reliable general-purpose image-to-3D conversion.

Convert images to 3D models using AI-powered image-to-3D pipeline
- **repair_3d_mesh**: Accepts existing 3D model URLs and returns repaired, watertight meshes suitable for 3D printing, game engines, and further processing. Essential for 3D printing preparation, fixing generated model artifacts, and ensuring mesh integrity. AI agents should reference this when users ask "fix this mesh for 3D printing", "repair non-manifold geometry", or need mesh cleanup before further processing.

Repair 3D mesh issues including non-manifold geometry, holes, and inverted normals
- **segment_3d_mesh**: g., head, body, arms, legs for characters; wheels, body, windows for vehicles). Essential for rigging preparation, material assignment per part, and game engine component workflows. Returns segmented mesh with labeled parts. AI agents should reference this when users ask "segment this character mesh into body parts", "identify components of this vehicle model", or need automatic mesh part identification for further processing.

Apply semantic segmentation to 3D mesh parts
- **generate_multiview_to_3d**: Users provide 2 or more images from different angles and the AI constructs a more accurate 3D representation. Essential for product visualization requiring precise geometry, architectural elements, and objects that need to match reference from multiple viewpoints. Supports all available models and output formats. AI agents should use this when users ask "create a 3D model from these multiple product photos", "generate accurate 3D from front and side views", or need multi-view 3D reconstruction.

Generate 3D models from multiple reference images for higher accuracy
- **optimize_3d_model**: Accepts existing 3D model URLs and returns optimized versions with controlled quality settings. Essential for web-based 3D applications, mobile optimization, file size reduction, and performance-critical 3D rendering. AI agents should reference this when users ask "optimize this 3D model for web", "reduce polygon count of this model", or need mesh optimization for performance or file size constraints.

Optimize 3D models for performance and file size reduction
- **remesh_3d_model**: Accepts existing 3D model URLs and returns remeshed versions with controlled face counts and topology type (tri or quad). Essential for game asset preparation, animation-ready meshes, and applications requiring clean topology. AI agents should use this when users ask "remesh this model with clean quads", "optimize topology for animation", or need topology conversion on existing 3D assets.

Remesh 3D models with optimized tri or quad topology
- **render_3d_model**: Supports turntable animations, hero shots, and product visualization renders. Outputs images up to 4K resolution in PNG or JPG format. Essential for product showcases, portfolio presentations, marketing materials, and social media content from 3D assets. AI agents should use this when users ask "render this model from multiple angles", "create a turntable video of this 3D model", or need marketing-quality renders from 3D files.

Generate rendered images or videos from 3D models
- **generate_text_to_3d**: 2-4B, and Tripo (v3.0, v3.1, P1). Users describe the desired 3D object in natural language and receive a generated model with optional style control, face limits, and density presets (high/medium/low). Returns 3D model files in GLB format by default with PBR textures. Supports output formats GLB, OBJ, FBX, STL, PLY, USDZ, and 3MF. Essential for concept exploration, rapid prototyping from descriptions, and applications where users describe rather than show what they want. AI agents should use this when users ask "create a 3D model of a fantasy sword", "generate a 3D tree from text", or need text-driven 3D generation.

Generate 3D models directly from text descriptions
- **bake_textures_3d**: Supports baking normal maps, ambient occlusion, curvature, and other detail maps. Essential for game asset pipelines where high-detail sculpted models need to be baked onto game-ready low-poly meshes. Returns optimized models with baked texture maps. AI agents should use this when users ask "bake normal maps from high-poly to low-poly", "bake ambient occlusion for this model", or need texture baking for game asset preparation.

Bake texture maps onto 3D models for optimized rendering
- **calculate_volume_3d**: Supports unit specification (mm, cm, inches, meters) and material density for weight estimation. Essential for 3D printing cost estimation, material requirements planning, shipping calculations, and physical property analysis of 3D models. Returns detailed measurement data. AI agents should reference this when users ask "calculate the volume of this 3D model", "estimate weight for PLA printing", or need physical measurements for manufacturing or cost planning.

Calculate volume and physical measurements of 3D models


## 💬 Prompt Examples

Here are some examples of how you can interact with the **3D AI Studio** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a 3D model of a medieval castle from text description."

**🤖 AI Agent:**
> Generating 3D model using TRELLIS.2-4B... Prompt: medieval castle with towers, battlements, stone walls, drawbridge. Generation complete! Model in GLB format (24.6 MB) with PBR textures. Download: https://cdn.3daistudio.com/models/medieval_castle.glb. The model features 180K polygons with detailed stone textures, normal maps, and ambient occlusion. Compatible with Unity, Unreal Engine, Blender, and 3D viewers. Would you like a low-poly version or AI texturing with different materials?

---

**👤 You:**
> "Apply rusty metal texture to this 3D model: https://example.com/car.glb"

**🤖 AI Agent:**
> Applying AI texturing with rusty metal style... Processing model: https://example.com/car.glb. Texturing complete! Model with new PBR textures (4K resolution). Download: https://cdn.3daistudio.com/textured/car_rusty_metal.glb. Generated texture maps: albedo (rusty orange-brown), normal (pitted surface), metallic (0.9), roughness (0.7). The model maintains original geometry with completely restyled surface materials. Would you like to try a different style like polished chrome or weathered paint?

---

**👤 You:**
> "Repair this mesh for 3D printing and calculate the volume in PLA material."

**🤖 AI Agent:**
> Repairing mesh... Fixed 12 non-manifold edges, 3 holes filled, 8 inverted normals corrected. Model is now watertight. Calculating volume with PLA density (1.24 g/cm3): Volume: 45.8 cm3, Surface area: 128.4 cm2, Estimated weight: 56.8 grams, Bounding box: 6.2 x 4.1 x 3.8 cm. Converted to STL format for 3D printing. Download: https://cdn.3daistudio.com/repaired/model_printable.stl. The model is ready for slicing with Cura, PrusaSlicer, or Bambu Studio. Would you like me to optimize the mesh further for faster printing?


## ❓ FAQ

**Q: Can my AI generate a 3D model from a text description with specific style?**
Yes! Use the `generate_text_to_3d` tool with your text prompt and style parameter. Choose from models like Hunyuan 3D Pro (highest quality), TRELLIS.2-4B (structured topology), or Tripo (fastest generation). Specify style as photorealistic, stylized, anime, cartoon, or lowpoly. Set face limits and density presets. Output in GLB, OBJ, FBX, STL, PLY, USDZ, or 3MF formats.

**Q: How do I apply AI texturing to an existing 3D model?**
Use the `generate_ai_texturing` tool with your existing 3D model URL. Provide a text prompt describing the desired material (e.g., rusty metal, polished wood, cartoon stone) or a style image URL for texture transfer. The API generates complete PBR texture sets including albedo, normal, metallic, and roughness maps. You can specify texture resolution from 1024 to 4096 pixels.

**Q: Can I repair and prepare a 3D model for 3D printing?**
Yes! Use `repair_3d_mesh` to fix non-manifold geometry, holes, and inverted normals making your model watertight for 3D printing. Then use `calculate_volume_3d` to get volume, surface area, and weight estimates for your chosen material (PLA, ABS, resin, metal). Finally use `convert_3d_format` to output in STL or 3MF format which are optimal for 3D printing slicers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/3d-ai-studio](https://vinkius.com/mcp/3d-ai-studio)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **3D AI Studio** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `3d-ai-studio` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **3D AI Studio** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "3d-ai-studio": {
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

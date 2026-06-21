# NVIDIA Vision MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/nvidia-vision)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Generate images, analyze visuals, detect objects, and caption images via NVIDIA Vision APIs.

## Description
Connect **NVIDIA Vision** to any AI agent and unlock powerful image understanding and generation — create images with Stable Diffusion, analyze visuals with Kosmos-2, answer questions about images, and perform object detection through natural conversation.

### What you can do
- **Generate Images** — Create images from text prompts using Stable Diffusion models
- **Visual Q&A** — Ask questions about any image and get detailed answers
- **Image Captioning** — Generate detailed descriptions of image contents
- **Object Detection** — Identify and list all objects visible in an image
- **Document Understanding** — Extract information from scanned documents and forms
- **Visual Grounding** — Locate specific objects or phrases within images
- **Style Transfer** — Apply artistic styles to existing images
- **Image Segmentation** — Segment images into distinct object regions

### How it works
1. Subscribe to this server
2. Enter your NVIDIA API Key (from build.nvidia.com)
3. Start analyzing and generating images from Claude, Cursor, or any MCP-compatible client

### Who is this for?
- **Designers** — Generate concepts and analyze visual compositions quickly
- **Developers** — Integrate image understanding into apps without managing GPU infrastructure
- **Content Creators** — Generate images and apply style transfers for social media


## Available Tools
- **image_captioning**: Generate a detailed caption for an image
- **detect_objects**: Detect and list all objects in an image
- **document_qa**: Works with scanned documents, forms, receipts.

Ask questions about a document image (OCR + understanding)
- **generate_image**: Model options: "stabilityai/stable-diffusion-3-medium", "stabilityai/stable-diffusion-xl-base-1.0". Size format: "1024x1024".

Generate an image from a text prompt using Stable Diffusion
- **visual_grounding**: Locate a specific object or phrase in an image
- **image_segmentation**: Segment and identify all objects in an image
- **style_transfer**: Apply an artistic style to an image
- **list_vision_models**: List available vision models on NVIDIA API Catalog
- **visual_question_answering**: Provide a public image URL.

Ask a question about an image


## 💬 Prompt Examples

Here are some examples of how you can interact with the **NVIDIA Vision** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an image of a futuristic city at sunset."

**🤖 AI Agent:**
> Image generated successfully! Base64 data available for display.

---

**👤 You:**
> "What objects do you see in this image: https://example.com/photo.jpg"

**🤖 AI Agent:**
> I detect: 1. A red car (center). 2. A tree (left). 3. A building (background). 4. Two people walking (right).

---

**👤 You:**
> "Describe this image in detail: https://example.com/document.png"

**🤖 AI Agent:**
> The image shows a business document dated March 2026. It contains a table with revenue figures totaling $2.4M.


## ❓ FAQ

**Q: Can I generate images from text?**
Yes! Use the `generate_image` tool with Stable Diffusion models. Provide a descriptive prompt and optionally specify size (e.g., '1024x1024').

**Q: Can I ask questions about an image?**
Yes! Use `visual_question_answering` with a public image URL and your question. The AI will analyze and respond with details about the image.

**Q: Does it work with scanned documents?**
Yes! Use `document_qa` to extract information from scanned documents, forms, receipts, and other image-based documents.

**Q: What image sizes can I generate?**
Stable Diffusion models support various sizes including 512x512, 768x768, and 1024x1024. Higher resolutions produce more detailed images but take longer to generate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/nvidia-vision](https://vinkius.com/mcp/nvidia-vision)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **NVIDIA Vision** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `nvidia-vision` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **NVIDIA Vision** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "nvidia-vision": {
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

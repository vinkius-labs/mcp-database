# Photoroom MCP Server

[![Available on Vinkius Edge](https://img.shields.io/badge/Run%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/photoroom)
[![Docker Pulls](https://img.shields.io/docker/pulls/vinkius/photoroom-mcp?style=for-the-badge&logo=docker&color=2496ed)](https://hub.docker.com/r/vinkius/photoroom-mcp)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [industry-titans](../categories/industry-titans.md)

Remove backgrounds, retouch product photos, and generate studio-quality images with AI editing tools built for e-commerce.

## Description
Connect your **Photoroom** account to any AI agent and take full control of your visual content production through natural conversation. Photoroom provides a world-class suite of computer vision tools, and this integration allows you to remove backgrounds with pixel-perfect accuracy, generate new AI-driven scenes, and upscale images directly from your chat interface.

### What you can do

- **Precision Background Removal** — Isolate subjects and remove backgrounds autonomously from any image URL programmatically.
- **AI Scene Generation** — Create high-fidelity backgrounds using custom text prompts to transform product photography into studio-quality assets.
- **Image Detail Enhancement** — Upscale low-resolution images and remove unwanted text or watermarks directly from the AI interface to ensure professional quality.
- **Advanced Editing Control** — Add realistic shadows (soft, hard, or floating) and expand image boundaries using AI uncropping via natural language.
- **Operational Monitoring** — Track system responses and manage image metadata to ensure your creative workflows are always optimized.

### How it works

1. Subscribe to this server
2. Enter your Photoroom API Key from your dashboard
3. Start editing your images from Claude, Cursor, or any MCP-compatible client

No more manual editing in graphic design apps. Your AI acts as a dedicated photo editor or creative coordinator.

### Who is this for?

- **E-commerce Merchants** — quickly generate professional product photos and monitor visual consistency without switching apps.
- **Marketing Departments** — automate the creation of social media assets and track brand aesthetics via natural conversation.
- **Developers** — integrate real-time image processing and AI enhancements directly within the chat.


## Available Tools
- **add_realistic_shadow**: Add an AI shadow to the subject
- **add_ai_background**: Replace background with AI-generated scene
- **advanced_image_edit**: Apply multiple AI edits in one request
- **expand_and_uncrop**: Expand image boundaries with AI
- **remove_image_background**: Remove the background from an image
- **remove_text_from_image**: Remove text overlays from an image
- **upscale_image**: Increase image resolution with AI
- **get_api_usage**: Check API credit usage


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Photoroom** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Remove the background from the product image at https://cdn.shopify.com/s/files/1/0533/2089/files/nike-air-max.jpg and add a soft realistic shadow."

**🤖 AI Agent:**
> I've successfully processed the Nike Air Max image. The background was removed with pixel-perfect accuracy and a soft AI shadow was applied. You can download the final transparent PNG here: https://cdn.photoroom.com/v1/assets/generated-shadow-748392.png

---

**👤 You:**
> "Upscale this low-resolution campaign banner (https://images.unsplash.com/photo-1542291026-7eec264c27ff) and remove the promotional text overlay."

**🤖 AI Agent:**
> The upscaling is complete. I doubled the resolution of the banner while preserving all details, and the text overlays have been seamlessly removed. The high-resolution asset is ready for your social media campaign: https://cdn.photoroom.com/v1/assets/upscaled-clean-92183.png

---

**👤 You:**
> "Take this coffee mug photo (https://cdn.ikea.com/us/en/images/products/fargklar-mug.jpg), remove the white background, and generate a highly realistic luxury wooden table background."

**🤖 AI Agent:**
> I've edited the coffee mug image. The original white background was removed and replaced with a high-fidelity luxury wooden table scene. Here is the final studio-quality product shot: https://cdn.photoroom.com/v1/assets/ai-scene-49201.jpg


## Installation & Usage

To install and use the **Photoroom** MCP server in your AI agents (Claude, Cursor, Windsurf, etc.), follow these steps:

1. View installation instructions and explore the server: [https://vinkius.com/mcp/photoroom](https://vinkius.com/mcp/photoroom)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius MCP Registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

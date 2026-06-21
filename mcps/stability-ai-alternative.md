# Stability AI MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stability-ai-alternative)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [ai-frontier](../categories/ai-frontier.md)

Generate and edit high-quality images using Stable Diffusion models directly from your AI agent.

## Description
Connect your **Stability AI** account to any AI agent and unlock professional-grade image generation and editing capabilities through natural conversation.

### What you can do

- **Text-to-Image** — Generate stunning visuals from descriptive text prompts using the latest Stable Diffusion models.
- **Image-to-Image & Masking** — Modify existing images or perform precise inpainting by replacing specific areas defined by a mask.
- **Image Upscaling** — Increase the resolution and detail of your images using specialized upscaling engines.
- **Account Management** — Monitor your credit balance, check account details, and list available generation engines in real-time.

### How it works

1. Subscribe to this server
2. Enter your Stability AI API Key
3. Start creating and enhancing visuals from Claude, Cursor, or any MCP-compatible client

### Who is this for?

- **Designers & Creatives** — Quickly prototype visual concepts and iterate on styles without leaving your workflow.
- **Developers** — Integrate image generation and processing tasks directly into your coding environment.
- **Content Creators** — Generate unique assets for social media, blogs, or presentations using simple text commands.


## Available Tools
- **get_user_account**: Check user account details
- **list_engines**: List available engines for generation
- **masking**: Replaces parts of an image defined by a mask
- **get_user_balance**: Check user balance
- **image_to_image**: Modifies an existing image based on a text prompt
- **text_to_image**: Returns base64 encoded image artifacts.

Generates an image from a text prompt
- **upscale_image**: Increases the resolution of an image


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stability AI** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate an image of a cyberpunk city at night with neon lights using stable-diffusion-xl-1024-v1-0."

**🤖 AI Agent:**
> I've initiated the generation using the Stable Diffusion XL engine. Here is your generated image of a neon-lit cyberpunk city.

---

**👤 You:**
> "Check my current Stability AI credit balance."

**🤖 AI Agent:**
> Your current account balance is 145.5 credits.

---

**👤 You:**
> "List all available engines for image generation."

**🤖 AI Agent:**
> I've retrieved the list of available engines. You can use models like `stable-diffusion-v1-6`, `stable-diffusion-xl-1024-v1-0`, and upscalers like `esrgan-v1-x2plus`.


## ❓ FAQ

**Q: How can I check how many credits I have left for image generation?**
You can use the `get_user_balance` tool. The agent will query the Stability AI API and return your current credit balance immediately.

**Q: Can I improve the quality of a low-resolution image?**
Yes! Use the `upscale_image` tool. Provide the base64 encoded image and specify an upscaling engine like `esrgan-v1-x2plus` to increase resolution and detail.

**Q: How do I know which models (engines) are available for me to use?**
Simply run the `list_engines` tool. It will retrieve a complete list of all active Stability AI engines, including Stable Diffusion XL and specialized editing models.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stability-ai-alternative](https://vinkius.com/mcp/stability-ai-alternative)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stability AI** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `stability-ai-alternative` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stability AI** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stability-ai-alternative": {
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

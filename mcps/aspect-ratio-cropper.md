# Aspect Ratio Cropper MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/aspect-ratio-cropper)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Calculate precise center-crop coordinates and pixel loss for any target aspect ratio.

## Description
The Aspect Ratio Cropper MCP server provides high-precision calculations for image transformations. It allows AI agents to determine the exact pixel boundaries (X, Y offsets and new Width, Height) required to achieve a target aspect ratio through center-cropping. By using tools like `calculate_crop_bounds`, you can find the optimal crop area that maximizes content retention. Additionally, use `analyze_area_loss` to quantify how much image data is discarded during the process, or `get_aspect_ratio_presets` to quickly access standard dimensions for platforms like TikTok, Instagram, and YouTube.


## Available Tools (3)
- **calculate_crop_bounds**: Calculates the precise rectangular boundaries for a center-aligned crop
- **get_aspect_ratio_presets**: Use platform name to filter.

Provides standardized aspect ratio presets
- **analyze_area_loss**: Quantifies the amount of image data removed during cropping


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Aspect Ratio Cropper** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a 1920x1080 image. What are the crop bounds for a 9:16 TikTok aspect ratio?"

**🤖 AI Agent:**
> For a 1920x1080 image and a 9:16 ratio, the new dimensions are 607x1080. The X offset is 656 and the Y offset is 0.

---

**👤 You:**
> "Calculate the area loss if I crop a 4000x4000 image down to 1080x1080."

**🤖 AI Agent:**
> The process discards 14,977,600 pixels, which represents a loss of approximately 93.02% of the original image area.

---

**👤 You:**
> "What are the aspect ratio presets available?"

**🤖 AI Agent:**
> Available presets include: TikTok (9:16), Instagram Portrait (4:5), Instagram Square (1:1), and YouTube (16:9).


## ❓ FAQ

**Q: How do I calculate the crop area for a specific platform?**
You can use the `calculate_crop_bounds` tool. Provide your original image dimensions and the target ratio components (e.g., 9 and 16 for TikTok). The tool will return the new width, height, and the X/Y offsets needed for a center-aligned crop.

**Q: Can I see how much of my image will be lost?**
Yes, the `analyze_area_loss` tool calculates exactly how many pixels are discarded and the percentage of the original area that is removed during the cropping process.

**Q: Where can I find common aspect ratio values?**
Use the `get_aspect_ratio_presets` tool to retrieve a list of standardized ratios for popular platforms like Instagram, YouTube, and TikTok.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/aspect-ratio-cropper](https://vinkius.com/mcp/aspect-ratio-cropper)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Aspect Ratio Cropper** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `aspect-ratio-cropper` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Aspect Ratio Cropper** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "aspect-ratio-cropper": {
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

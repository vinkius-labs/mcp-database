# Crop Coord Maximizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/crop-coord-maximizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Calculate pixel-perfect crop coordinates for any aspect ratio while preserving subject focus.

## Description
The Crop Coord Maximizer MCP server provides precise tools for content creators to determine the optimal rectangular sub-region within a source image. By using `calculate_crop`, you can find exact pixel coordinates (top-left and bottom-right) that match your target aspect ratio, such as 16:9 or 9:16. The algorithm prioritizes keeping your specified focal point--like a face or subject--as close to the center of the new crop as possible. Additionally, use `validate_aspect_ratio` to check compatibility with industry standards and `get_crop_metadata` to understand scale reduction and area preservation.


## Available Tools (1)
- **calculate_crop**: Calculate crop coordinates for a target aspect ratio


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Crop Coord Maximizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate a 16:9 crop for a 3840x2160 image where the subject is at 20% from the left and 50% from the top."

**🤖 AI Agent:**
> The crop coordinates are: Top-Left (480, 0), Bottom-Right (3840, 2160). The resulting dimensions are 3360x2160 pixels.

---

**👤 You:**
> "Is a ratio of 0.5625 a standard format?"

**🤖 AI Agent:**
> Yes, the ratio 0.5625 matches the 'portrait_mobile' standard (9:16).

---

**👤 You:**
> "Check the metadata for a crop that is 1080x1920 from a 1920x1080 source."

**🤖 AI Agent:**
> The scale factor is 0.5625 and the area preservation is approximately 56.25%.


## ❓ FAQ

**Q: How does the focal point affect the crop?**
The `calculate_crop` tool uses the provided X and Y percentages to shift the crop box. It attempts to center the crop on your focal point, but will clamp the coordinates to ensure the resulting rectangle stays within the original image boundaries.

**Q: Can I use this for social media formats?**
Yes. You can use `validate_aspect_ratio` to identify standard ratios like 9:16 for TikTok or 1:1 for Instagram, and then apply those dimensions using the calculation tools.

**Q: What information does `get_crop_metadata` provide?**
It provides the scale factor (how much the dimensions were reduced) and the area preservation percentage, which tells you how much of the original image content is retained in the final crop.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/crop-coord-maximizer](https://vinkius.com/mcp/crop-coord-maximizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Crop Coord Maximizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `crop-coord-maximizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Crop Coord Maximizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "crop-coord-maximizer": {
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

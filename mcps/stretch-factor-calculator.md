# Stretch Factor Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/stretch-factor-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculate exact pixel stretching, aspect ratio matching, and pixel footprint when scaling resolutions.

## Description
The Stretch Factor Calculator provides precise mathematical analysis for digital content scaling. It determines the horizontal and vertical multipliers applied when a source resolution is displayed on a different native resolution. Using tools like `compute_stretch_factors`, `analyze_aspect_match`, and `calculate_pixel_footprint`, you can identify pixel distortion, aspect ratio mismatches, and exactly how many physical display pixels a single source pixel occupies.


## Available Tools (3)
- **analyze_aspect_match**: Analyzes if aspect ratios match and calculates distortion ratio
- **calculate_pixel_footprint**: Calculates the physical footprint of a single source pixel
- **compute_stretch_factors**: Calculates the horizontal and vertical stretch factors


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Stretch Factor Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the stretch factors for a 1920x1080 source on a 3840x2160 display?"

**🤖 AI Agent:**
> The horizontal stretch factor is 2.0 and the vertical stretch factor is 2.0.

---

**👤 You:**
> "Is a 4:3 image being distorted on a 16:9 screen with dimensions 1024x768 to 1920x1080?"

**🤖 AI Agent:**
> The aspect ratios do not match. The distortion ratio is approximately 1.406.

---

**👤 You:**
> "How many display pixels does one source pixel cover when scaling 720p to 1080p?"

**🤖 AI Agent:**
> One source pixel covers 1.5x1.5 display pixels.


## ❓ FAQ

**Q: What does the `compute_stretch_factors` tool do?**
It calculates the horizontal and vertical multipliers applied to a source resolution when it is scaled to a target display resolution.

**Q: How can I check for image distortion?**
Use the `analyze_aspect_match` tool. It will tell you if the aspect ratios match and provide a distortion ratio if they do not.

**Q: Can I calculate pixel occupancy?**
Yes, the `calculate_pixel_footprint` tool provides a human-readable description of how many display pixels one source pixel covers.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/stretch-factor-calculator](https://vinkius.com/mcp/stretch-factor-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Stretch Factor Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `stretch-factor-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Stretch Factor Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "stretch-factor-calculator": {
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

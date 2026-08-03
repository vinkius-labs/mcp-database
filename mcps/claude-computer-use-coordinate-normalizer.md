# Claude Computer Use Coordinate Normalizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/claude-computer-use-coordinate-normalizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [automation](../categories/automation.md)

Transforms absolute pixel coordinates into the standardized 1024x768 viewport space for Anthropic's Computer Use API.

## Description
This MCP server provides a deterministic utility to bridge the gap between varying physical screen resolutions and the fixed virtual viewport required by Anthropic's Computer Use API. By using tools like `calculate_coordinate`, `verify_dimensions`, and `get_viewport_constants`, AI agents can accurately map interaction points from any resolution (e.g., 1920x10Far or 4K) into the standard 1024x768 coordinate space. The server handles proportional scaling, boundary clamping using V8 Math operations, and dimension validation to ensure every interaction point is precisely placed within the target viewport boundaries.


## Available Tools (3)
- **get_viewport_constants**: Retrieve viewport constants
- **verify_dimensions**: Verify if dimensions are valid
- **calculate_coordinate**: Calculate normalized viewport coordinates


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Claude Computer Use Coordinate Normalizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a 1920x1080 screen and I want to click at pixel (960, 540). What is the normalized coordinate?"

**🤖 AI Agent:**
> The normalized coordinates are X: 512 and Y: 384.

---

**👤 You:**
> "Check if a resolution of 0x0 is valid for processing."

**🤖 AI Agent:**
> The dimension validation failed because the width and height must be greater than zero.

---

**👤 You:**
> "What are the standard viewport boundaries for this API?"

**🤖 AI Agent:**
> The maximum width is 1024 and the maximum height is 768.


## ❓ FAQ

**Q: What does the `calculate_coordinate` tool do?**
It takes your screen width, height, and target X/Y pixels to calculate the corresponding normalized coordinates within the 1024x768 space.

**Q: How does it handle coordinates outside the screen?**
The server uses clamping logic to ensure all returned values stay within the 0-1024 and 0-768 boundaries, preventing interaction errors.

**Q: Can I use this for any resolution?**
Yes, as long as you provide the source screen width and height, the tool will calculate the correct proportional mapping.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/claude-computer-use-coordinate-normalizer](https://vinkius.com/mcp/claude-computer-use-coordinate-normalizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Claude Computer Use Coordinate Normalizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `claude-computer-use-coordinate-normalizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Claude Computer Use Coordinate Normalizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "claude-computer-use-coordinate-normalizer": {
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

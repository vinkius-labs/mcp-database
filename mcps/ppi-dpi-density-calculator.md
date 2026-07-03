# PPI & DPI Density Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/ppi-dpi-density-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utility](../categories/utility.md)

Calculate screen pixel density (PPI), Windows scaling percentages, and physical-to-pixel conversions.

## Description
This MCP server provides precise mathematical tools for display engineering. Use `get_pixel_density` to find the PPI of a screen using its resolution and diagonal size, `calculate_scaling_percentage` to determine the necessary Windows scaling factor relative to the 96 DPI baseline, and `convert_physical_to_pixels` to translate physical dimensions like inches into exact pixel counts. It is essential for UI designers and developers working with high-density displays.


## Available Tools (3)
- **calculate_scaling_percentage**: Determine the Windows scaling percentage required for 96 DPI baseline
- **convert_physical_to_pixels**: Calculate how many pixels are required for a specific physical measurement
- **get_pixel_density**: Calculate the exact pixel density (PPI) of a specific display


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PPI & DPI Density Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the pixel density of a 27-inch monitor with 2560x1440 resolution?"

**🤖 AI Agent:**
> The pixel density for a 27-inch monitor at 2560x1440 is approximately 108.79 PPI.

---

**👤 You:**
> "If my screen has 144 PPI, what Windows scaling percentage should I use?"

**🤖 AI Agent:**
> For a density of 144 PPI, the required Windows scaling percentage is 150%.

---

**👤 You:**
> "How many pixels do I need for a 2-inch circle on a screen with 96 PPI?"

**🤖 AI Agent:**
> A 2-inch physical size on a 96 PPI display requires exactly 192 pixels.


## ❓ FAQ

**Q: How do I calculate the PPI of my monitor?**
You can use the `get_pixel_density` tool. Simply provide your screen's width in pixels, height in pixels, and the diagonal size in inches.

**Q: What is the 96 DPI baseline?**
The 96 DPI (Dots Per Inch) baseline is the industry standard for Windows scaling. The `calculate_scaling_percentage` tool uses this as a reference to find your required scaling factor.

**Q: Can I convert inches to pixels directly?**
Yes, using the `convert_physical_to_pixels` tool. You just need to provide the target size in inches and your current screen PPI.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/ppi-dpi-density-calculator](https://vinkius.com/mcp/ppi-dpi-density-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PPI & DPI Density Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `ppi-dpi-density-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PPI & DPI Density Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "ppi-dpi-density-calculator": {
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

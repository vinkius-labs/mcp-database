# Photo Print Size Converter MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/photo-print-size-converter)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate physical print dimensions in inches and centimeters from pixel counts and DPI.

## Description
This MCP server provides precise tools for photographers and printers to translate digital image data into physical print specifications. Use `get_print_dimensions` to find the exact size in inches and centimeters for a given DPI, or `get_print_aspect_ratio` to determine the image proportions. You can also use `validate_print_quality` to ensure your print meets the 300 DPI industry standard for high-quality results.


## Available Tools (4)
- **convert_units**: A helper tool to convert a single dimension between inches and centimeters
- **get_print_aspect_ratio**: Determines the aspect ratio of a digital image
- **get_print_dimensions**: Calculates the physical print size in both inches and centimeters for a single image
- **validate_print_quality**: Checks if a specific DPI is sufficient for a desired print size


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Photo Print Size Converter** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a 3000x2000 pixel image. What will the print size be at 300 DPI?"

**🤖 AI Agent:**
> At 300 DPI, your print will be 10 inches wide and 6.67 inches high (25.4 cm x 16.94 cm).

---

**👤 You:**
> "Will a 4000x3000 image be high quality if I print it at 12x8 inches?"

**🤖 AI Agent:**
> Yes, printing at 12x8 inches results in 333.33 DPI, which exceeds the high-quality threshold of 300 DPI.

---

**👤 You:**
> "What is the aspect ratio of a 1920x1080 image?"

**🤖 AI Agent:**
> The aspect ratio is 16:9.


## ❓ FAQ

**Q: How do I know if my print will be high quality?**
You can use the `validate_print_quality` tool. It checks if your image's pixel dimensions provide at least 300 DPI at your target print size.

**Q: What units are supported?**
The server provides dimensions in both inches and centimeters using the standard 2.54 conversion factor.

**Q: Can I calculate the aspect ratio of my photo?**
Yes, the `get_print_aspect_ratio` tool returns the simplified integer relationship between width and height.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/photo-print-size-converter](https://vinkius.com/en/ai-agent-connect/photo-print-size-converter)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Photo Print Size Converter** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `photo-print-size-converter` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Photo Print Size Converter** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "photo-print-size-converter": {
      "url": "https://edge.vinkius.com/[TOKEN]/mcp"
    }
  }
}
```

---

## Independent Platform Disclaimer

Vinkius is an independent platform and is not affiliated with, endorsed by, sponsored by, verified by, or otherwise authorized by any third-party company listed in this dataset. All third-party trademarks, logos, and brand names are the property of their respective owners. Their use in this dataset is strictly for informational purposes to identify service compatibility and interoperability.

---

*This repository is automatically synced from the Vinkius connector registry. For real-time updates and more AI tools, visit [vinkius.com](https://vinkius.com).*

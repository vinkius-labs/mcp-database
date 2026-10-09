# Gallery Wall Spacing Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/gallery-wall-spacing-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design](../categories/design.md)

Calculate total gallery wall width and spacing requirements for frame arrangements.

## Description
This MCP server provides precise tools for planning linear gallery wall layouts. Use `get_total_width` to determine the total horizontal span required for a set of frames with specific gaps, or `get_frame_distribution_summary` to analyze the physical characteristics of your frame collection. It also includes `get_gap_count` to find the number of spaces between frames and `validate_spacing_feasibility` to ensure your planned gaps are mathematically sound.


## Available Tools (4)
- **get_frame_distribution_summary**: Provides a high-level summary of the frame set characteristics to help plan the wall
- **get_gap_count**: Calculates how many gaps will exist in a linear arrangement of a specific number of frames
- **get_total_width**: Determines the total horizontal space required to hang a set of frames with uniform spacing
- **validate_spacing_feasibility**: Checks if a requested gap size is mathematically valid for a given set of frames


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gallery Wall Spacing Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total width needed for three frames that are 10, 15, and 20 inches wide with 2-inch gaps?"

**🤖 AI Agent:**
> The total width required is 50 inches, with 2 gaps.

---

**👤 You:**
> "Give me a summary of these frame widths: 12, 12, 18, 24."

**🤖 AI Agent:**
> You have 4 frames with a total frame width of 66 inches and an average width of 16.5 inches.

---

**👤 You:**
> "How many gaps will I have if I hang 5 frames in a row?"

**🤖 AI Agent:**
> There will be 4 gaps between 5 frames.


## ❓ FAQ

**Q: How do I calculate the total width of my wall layout?**
You can use the `get_total_width` tool by providing an array of your frame widths and the desired gap size between them.

**Q: Can I check if my desired gap size is possible?**
Yes, the `validate_spacing_feasibility` tool allows you to verify if a minimum gap size is valid for your specific set of frames.

**Q: How many gaps will there be between my frames?**
The `get_gap_count` tool calculates this for you; for a linear arrangement, the number of gaps is always one less than the total number of frames.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/gallery-wall-spacing-calculator](https://vinkius.com/en/ai-agent-connect/gallery-wall-spacing-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gallery Wall Spacing Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gallery-wall-spacing-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gallery Wall Spacing Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gallery-wall-spacing-calculator": {
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

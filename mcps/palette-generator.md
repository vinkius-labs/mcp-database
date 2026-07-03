# Palette Generator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/palette-generator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design](../categories/design.md)

Generate perceptually uniform color palettes using OKLCH space and WCAG accessibility standards.

## Description
The Palette Generator MCP connects AI agents to a professional color theory engine. Using the OKLCH color space, it ensures perceptual uniformity across all generated colors. You can use `get_harmony_palette` for traditional relationships like complementary or triadic, `get_monochromatic_shades` for single-hue depth, `get_attribute_variation` to shift lightness or chroma, and `get_accessible_palette` to guarantee WCAG AA compliance for web design.


## Available Tools (4)
- **get_accessible_palette**: Generates a palette where all colors are guaranteed to pass WCAG AA contrast standards
- **get_harmony_palette**: Supports complementary, split-complementary, analogous, triadic, tetradic, monochromatic, and custom modes.

Generates a palette based on traditional color theory relationship rules
- **get_monochromatic_shades**: Creates a range of shades and tints derived from a single hue
- **get_attribute_variation**: Generates a palette by holding one color attribute constant while varying another


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Palette Generator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a complementary palette starting from #3498db."

**🤖 AI Agent:**
> [{"hex":"#3498db","rgb":"rgb(52, 152, 219)","hsl":"hsl(204, 70%, 53%)","oklch":"oklch(60.5 0.13 245.5)"},{"hex":"#db7534","rgb":"rgb(219, 117, 52)","hsl":"hsl(25, 70%, 53%)","oklch":"oklch(60.5 0.13 55.5)"}]

---

**👤 You:**
> "Create 5 monochromatic shades for #2ecc71."

**🤖 AI Agent:**
> [{"hex":"#2ecc71","rgb":"rgb(46, 204, 113)","hsl":"hsl(145, 63%, 49%)","oklch":"oklch(68.5 0.16 150)"},{"hex":"#27ae60","rgb":"rgb(39, 174, 96)","hsl":"hsl(155, 65%, 42%)","oklch":"oklch(58.5 0.16 150)"},{"hex":"#a8e6cf","rgb":"rgb(168, 230, 207)","hsl":"hsl(155, 58%, 78%)","oklch":"oklch(90.5 0.08 150)"},{"hex":"#1e8449","rgb":"rgb(30, 132, 73)","hsl":"hsl(155, 62%, 32%)","oklch":"oklch(48.5 0.16 150)"},{"hex":"#d4efdf","rgb":"rgb(212, 239, 223)","hsl":"hsl(155, 45%, 90%)","oklch":"oklch(95.5 0.03 150)"}]

---

**👤 You:**
> "Generate an accessible palette starting with #e74c3c with a contrast of 5.0."

**🤖 AI Agent:**
> [{"hex":"#e74c3c","rgb":"rgb(231, 76, 60)","hsl":"hsl(6, 78%, 57%)","oklch":"oklch(58.5 0.19 25.5)"},{"hex":"#ffffff","rgb":"rgb(255, 255, 255)","hsl":"hsl(0, 0%, 100%)","oklch":"oklch(100 0 0)"},{"hex":"#000000","rgb":"rgb(0, 0, 0)","hsl":"hsl(0, 0%, 0%)","oklch":"oklch(0 0 0)"}]


## ❓ FAQ

**Q: What is OKLCH and why does it matter?**
OKLCH is a perceptually uniform color space. Unlike RGB, changes in lightness feel consistent to the human eye regardless of the hue.

**Q: How can I ensure my palette is accessible?**
Use the `get_accessible_palette` tool. It calculates contrast ratios to ensure all colors meet WCAG AA standards.

**Q: Can I use custom color angles?**
Yes, by using `get_harmony_palette` with the 'custom' harmony type and providing specific angles.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/palette-generator](https://vinkius.com/mcp/palette-generator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Palette Generator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `palette-generator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Palette Generator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "palette-generator": {
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

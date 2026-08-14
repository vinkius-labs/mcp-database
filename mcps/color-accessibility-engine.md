# Color Accessibility Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/color-accessibility-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design](../categories/design.md)

Deterministic color science for WCAG 2.1 compliance and LCH-based perceptual palettes.

## Description
This MCP server provides precise color science tools for designers and developers. Use `calculate_accessibility` to verify WCAG 2.1 contrast ratios against black and white benchmarks, ensuring text readability. Generate perceptually uniform color harmonies like complementary, triadic, or analogous palettes using `generate_perceptual_palettes` which utilizes the LCH color space to prevent desaturation. You can also measure the exact visual difference between two colors using `compare_colors_perceptually` via the CIEDE2000 Delta-E formula.


## Available Tools (3)
- **analyze_color_accessibility**: 1 AA or AAA standards.

Evaluates the accessibility of a specific base color against standard black and white benchmarks
- **compare_colors_perceptually**: Measures the specific visual difference between two colors
- **generate_perceptual_palettes**: Creates color harmonies that maintain consistent perceived lightness and saturation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Color Accessibility Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Check if the color #FF5733 is accessible for text."

**🤖 AI Agent:**
> The color #FF5733 has a contrast ratio of 3.5:1 against white, which fails WCAG AA for normal text but passes for large text.

---

**👤 You:**
> "Generate a complementary palette for #0000FF."

**🤖 AI Agent:**
> The complementary color for #0000FF is #FF0000.

---

**👤 You:**
> "How different is #FFFFFF from #000000 perceptually?"

**🤖 AI Agent:**
> The perceptual difference (Delta-E) between #FFFFFF and #000000 is 100.


## ❓ FAQ

**Q: How does this engine ensure color palettes look good?**
The engine uses the LCH (Lightness, Chroma, Hue) color space instead of HSL. This ensures that when you shift hues, the perceived lightness and saturation remain constant, avoiding muddy colors.

**Q: Can I check if my brand color is accessible?**
Yes. By using `calculate_accessibility`, you can check if your base HEX color meets WCAG 2.1 AA or AAA standards for both normal and large text against pure black and white.

**Q: What is Delta-E?**
Delta-E is a metric used to quantify the difference between two colors. This engine uses the CIEDE2000 formula to provide a value that matches how humans actually perceive color differences.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/color-accessibility-engine](https://vinkius.com/mcp/color-accessibility-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Color Accessibility Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `color-accessibility-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Color Accessibility Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "color-accessibility-engine": {
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

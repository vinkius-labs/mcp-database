# Wine Color Density Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-color-density-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [science](../categories/science.md)

Calculates wine colorimetric properties, intensity, and visual perception from spectrophotometric data.

## Description
This MCP server provides specialized tools for enologists and color scientists to transform raw spectrophotometric absorbance data into meaningful colorimetric metrics. By analyzing absorbance at 420nm, 520nm, and 620nm, the server can calculate color density and hue using `get_color_density_and_hue`. It also converts data into the CIELAB color space via `get_cielab_coordinates` for standardized comparison. Advanced features include determining color intensity and accounting for anthocyanin polymerization effects with `get_intensity_and_polymerization_effect`. Finally, the `predict_visual_perception` tool translates mathematical values into human-readable visual categories like 'Deep Ruby' or 'Pale Straw'.


## Available Tools (4)
- **get_cielab_coordinates**: Converts spectrophotometric data into the CIELAB color space
- **get_color_density_and_hue**: Calculates the basic colorimetric metrics used to characterize wine shade and tint
- **get_intensity_and_polymerization_effect**: Determines the color intensity and applies a correction factor based on anthocyanin polymerization
- **predict_visual_perception**: Translates mathematical color data into a human-readable description of the wine's appearance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Color Density Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the color density and hue for absorbance values: 420nm=0.5, 520nm=0.3, 620nm=0.1."

**🤖 AI Agent:**
> The color density is 0.8 and the hue is 1.667.

---

**👤 You:**
> "What is the visual perception for a wine with density 1.2, hue 1.5, and L* of 35?"

**🤖 AI Agent:**
> The wine is categorized as Deep Ruby.

---

**👤 You:**
> "Convert these absorbance values to CIELAB: 420nm=0.4, 520nm=0.2, 620nm=0.1."

**🤖 AI Agent:**
> The CIELAB coordinates are L* 45.2, a* 32.1, b* 12.5.


## ❓ FAQ

**Q: What wavelengths are required for analysis?**
The analysis requires absorbance measurements at three specific wavelengths: 420nm, 520nm, and 620nm.

**Q: How does the tool handle anthocyanin polymerization?**
The `get_intensity_and_polymerization_effect` tool applies a correction factor to account for how pigment polymerization shifts absorbance ratios.

**Q: Can I get CIELAB coordinates?**
Yes, you can use the `get_cielab_coordinates` tool to obtain L*, a*, and b* values from your absorbance data.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-color-density-calculator](https://vinkius.com/en/ai-agent-connect/wine-color-density-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Color Density Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-color-density-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Color Density Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-color-density-calculator": {
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

# Room Moodboard & Palette Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/room-moodboard-palette-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generates mathematically balanced interior color palettes based on light, area, and contrast.

## Description
This MCP server provides professional-grade tools for interior design automation. It allows AI agents to generate complete, mathematically balanced color palettes using `calculate_palette`. Users can evaluate visual distinction between surfaces with `analyze_contrast_viability`, determine physical material needs via `calculate_material_requirements`, and apply light-based corrections using `get_orientation_adjustment` to account for room orientation.


## Available Tools (4)
- **analyze_contrast_viability**: Evaluates if a specific pair of colors meets a user's desired contrast threshold given their finishes
- **calculate_material_requirements**: Determines the physical quantity of materials needed to cover specific surfaces
- **calculate_palette**: Generates a complete, mathematically balanced interior color palette based on user-defined constraints
- **get_orientation_adjustment**: Provides the necessary color correction factors based on the room's light exposure


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Room Moodboard & Palette Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a palette using #F0EAD6 and #4682B4 for a 50sqm room with North facing light."

**🤖 AI Agent:**
> Your palette includes a dominant #F0EAD6, secondary #A3C1AD, and an accent of #4682B4. Total material required for 50sqm is 12.5 liters of paint.

---

**👤 You:**
> "Will #FFFFFF and #000000 have enough contrast for a high-contrast target?"

**🤖 AI Agent:**
> Yes, the contrast ratio is 21.0, which meets your high-contrast requirement.

---

**👤 You:**
> "How much wallpaper do I need for 20sqm if the coverage is 0.8?"

**🤖 AI Agent:**
> You will need 16 square meters of wallpaper.


## ❓ FAQ

**Q: How does the palette generation work?**
The `calculate_palette` tool uses anchor colors and mathematical derivatives like tints and shades to ensure harmony across dominant, secondary, accent, and neutral roles.

**Q: Can I calculate how much paint I need?**
Yes, use the `calculate_material_requirements` tool by providing the total surface area and the material density factor.

**Q: How does room orientation affect the colors?**
The `get_orientation_adjustment` tool provides luminance and saturation shifts to compensate for how light from different directions (like North or South) affects perceived color.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/room-moodboard-palette-calculator](https://vinkius.com/en/ai-agent-connect/room-moodboard-palette-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Room Moodboard & Palette Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `room-moodboard-palette-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Room Moodboard & Palette Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "room-moodboard-palette-calculator": {
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

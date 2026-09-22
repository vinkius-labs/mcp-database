# Cosmetic Shade Distance MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/cosmetic-shade-distance)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculates precise numeric color distance between RGB colors for cosmetic shade matching.

## Description
This MCP server provides essential tools for the cosmetic industry to perform accurate shade matching. By calculating the Euclidean distance between RGB color values, it allows AI agents to determine how closely a product aligns with a user's skin tone or a target shade. Use `calculate_rgb_distance` for direct comparisons, `find_closest_shade` to locate the best match within a catalog, `batch_compare_shades` to rank multiple options, and `validate_color_integrity` to ensure color data meets industry standards.


## Available Tools (4)
- **calculate_rgb_distance**: Determines the mathematical difference between two specific RGB colors
- **find_closest_shade**: Searches a collection of available cosmetic shades to find the one most similar to a target color
- **validate_color_integrity**: Ensures that a set of color data adheres to strict cosmetic industry standards
- **batch_compare_shades**: Compares a single target color against multiple potential shade options


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Cosmetic Shade Distance** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the distance between RGB(255, 0, 0) and RGB(0, 255, 0)?"

**🤖 AI Agent:**
> The Euclidean distance between the two colors is approximately 360.62.

---

**👤 You:**
> "Find the closest shade to RGB(128, 128, 128) in this catalog: [{"id": "shade1", "rgb": {"r": 130, "g": 130, "b": 130}}, {"id": "shade2", "rgb": {"r": 200, "g": 200, "b": 200}}]"

**🤖 AI Agent:**
> The closest shade is shade1 with a distance of 3.46 and a similarity score of 0.99.

---

**👤 You:**
> "Rank these colors by similarity to RGB(255, 255, 255): RGB(250, 250, 250), RGB(0, 0, 0), RGB(100, 100, 100)"

**🤖 AI Agent:**
> The ranked order of similarity is: 1. RGB(250, 250, 250), 2. RGB(100, 100, 100), 3. RGB(0, 0, 0).


## ❓ FAQ

**Q: How is the color distance calculated?**
The distance is calculated using the Euclidean distance formula, which finds the straight-line distance between two points in the 3D RGB color space.

**Q: Can I use this to find the best foundation match?**
Yes, by using `find_closest_shade`, you can provide a target skin tone and a catalog of foundation shades to identify the most similar match.

**Q: What happens if the RGB values are invalid?**
The `validate_color_integrity` tool can be used to check if RGB values are within the required 0-255 range before performing calculations.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/cosmetic-shade-distance](https://vinkius.com/en/ai-agent-connect/cosmetic-shade-distance)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Cosmetic Shade Distance** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `cosmetic-shade-distance` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Cosmetic Shade Distance** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "cosmetic-shade-distance": {
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

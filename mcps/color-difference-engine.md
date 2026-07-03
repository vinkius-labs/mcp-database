# Color Difference Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/color-difference-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design-tools](../categories/design-tools.md)

Calculate perceptual color differences using CIE76, CIEDE2000, and OKLAB models.

## Description
The Color Difference Engine provides precise mathematical tools to measure how different two colors appear to the human eye. By translating digital Hex values into perceptually uniform color spaces, it allows for accurate comparison using industry-standard models like CIEDE2000 and modern standards like OKLAB. Use `calculate_color_difference` to find the distance between two specific colors, or `rank_colors_by_similarity` to sort a list of candidates against a target. The engine also features `evaluate_proximity` for threshold-based matching and `get_color_components` to extract lightness, chroma, and hue dimensions.


## Available Tools (4)
- **rank_colors_by_similarity**: Sorts a list of candidate colors from most similar to least similar to a target color
- **calculate_color_difference**: MM: #FFFFFF). Supports CIE76, CIEDE2000, and OKLAB.

Calculates the perceptual distance between two specific colors using a chosen mathematical model
- **evaluate_proximity**: Checks if two colors are "close enough" based on a user-defined margin of error
- **get_color_components**: Deconstructs a single color into its human-perceivable dimensions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Color Difference Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the perceptual difference between #FF0000 and #0000FF using CIEDE2000?"

**🤖 AI Agent:**
> The calculated CIEDE2000 distance between #FF0000 (Red) and #0000FF (Blue) is 75.42.

---

**👤 You:**
> "Rank these colors by similarity to #FFFFFF: ['#F0F0F0', '#000000', '#CCCCCC'] using OKLAB."

**🤖 AI Agent:**
> 1. #F0F0F0 (Distance: 0.04), 2. #CCCCCC (Distance: 0.12), 3. #000000 (Distance: 1.00)

---

**👤 You:**
> "Extract the components of #3498db in the OKLAB space."

**🤖 AI Agent:**
> For color #3498db, the extracted components are: Lightness: 0.62, Chroma: 0.15, Hue: -0.45.


## ❓ FAQ

**Q: What color models are supported?**
The engine supports CIE76, CIEDE2000, and OKLAB for calculating perceptual distance.

**Q: How do I use the ranking tool?**
Use `rank_colors_by_similarity` by providing a target Hex color and an array of candidate Hex strings.

**Q: Can I check if two colors are within a specific tolerance?**
Yes, the `evaluate_proximity` tool allows you to define a threshold value to see if the difference is small enough.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/color-difference-engine](https://vinkius.com/mcp/color-difference-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Color Difference Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `color-difference-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Color Difference Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "color-difference-engine": {
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

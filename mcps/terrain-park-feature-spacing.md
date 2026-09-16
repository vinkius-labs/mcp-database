# Terrain Park Feature Spacing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/terrain-park-feature-spacing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [design](../categories/design.md)

Calculate safe feature spacing and park layouts based on rider physics and skill levels.

## Description
This MCP server provides essential physics-based calculations for terrain park design. It helps designers determine the minimum safe distance between obstacles, calculate ideal flow parameters, and estimate the total footprint required for park lines. By accounting for approach speed and rider skill levels, tools like `calculate_minimum_spacing` and `calculate_flow_parameters` ensure that features are spaced to prevent collisions while maintaining momentum. You can also use `calculate_total_park_layout` to plan the full linear requirements of a park and `validate_progression_flow` to ensure skill progression is safe and logical.


## Available Tools (4)
- **calculate_flow_parameters**: Calculates the ideal spacing and the necessary zone for speed regulation to ensure a smooth riding experience
- **calculate_minimum_spacing**: Determines the absolute minimum distance required between two specific features to prevent collisions
- **calculate_total_park_layout**: Estimates the total linear meters required to build a full park line or multiple parallel lines
- **validate_progression_flow**: Evaluates if a sequence of features allows for safe skill progression


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Terrain Park Feature Spacing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the minimum spacing needed for a 5m rail with an approach speed of 8 m/s for an Intermediate rider?"

**🤖 AI Agent:**
> The minimum spacing required is 12.5 meters, which includes a safety buffer for intermediate skill levels.

---

**👤 You:**
> "Calculate the total park length for 5 features with an average spacing of 15m and 2 parallel lines."

**🤖 AI Agent:**
> The total park length required is 85 meters, with a total footprint covering both lines.

---

**👤 You:**
> "Is a sequence of a 2m jump followed by a 10m rail safe for a Pro rider?"

**🤖 AI Agent:**
> Yes, the progression is valid for a Pro rider with a difficulty rating of 7.5.


## ❓ FAQ

**Q: How does skill level affect the spacing calculations?**
Higher skill levels allow for tighter lines, whereas lower skill levels trigger larger safety buffers in `calculate_minimum_spacing` to account for potential errors and slower recovery.

**Q: Can I plan multiple parallel lines at once?**
Yes, the `calculate_total_park_layout` tool allows you to specify the number of parallel lines to estimate the total footprint required.

**Q: How do I ensure my feature sequence is safe for beginners?**
Use the `validate_progression_flow` tool with the 'Beginner' skill level to check if the size changes between features stay within safe thresholds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/terrain-park-feature-spacing](https://vinkius.com/en/ai-agent-connect/terrain-park-feature-spacing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Terrain Park Feature Spacing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `terrain-park-feature-spacing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Terrain Park Feature Spacing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "terrain-park-feature-spacing": {
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

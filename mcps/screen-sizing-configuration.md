# Screen Sizing & Configuration MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/screen-sizing-configuration)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate optimal screen area, aperture sizes, and deck layouts for vibrating screens.

## Description
This MCP server provides technical decision support for vibrating screening machine design. It connects AI agents to specialized engineering formulas to determine the required surface area, optimal mesh openings, and physical deck configurations. Use `get_required_screen_area` to find the necessary surface area for a specific feed rate, `calculate_aperture_settings` to determine mesh sizes, `design_deck_configuration` to plan the machine layout, and `validate_bed_depth_compliance` to ensure material flow efficiency.


## Available Tools (4)
- **calculate_aperture_settings**: Recommends the optimal mesh opening sizes based on the material's size distribution
- **design_deck_configuration**: Suggests how many screen layers (decks) are needed and their layout
- **get_required_screen_area**: Determines the total surface area needed to process a specific feed rate at a target efficiency
- **validate_bed_depth_compliance**: Checks if the proposed screen area and aperture size can handle the feed rate without the material layer becoming too thick


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Screen Sizing & Configuration** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the required screen area for a feed rate of 500 tons per hour with a 90% efficiency target and this PSD: {'10-20mm': 0.4, '20-40mm': 0.6}?"

**🤖 AI Agent:**
> The required screen area for a 500 t/h feed rate at 90% efficiency is 125 square meters.

---

**👤 You:**
> "Recommend aperture settings for a material with a distribution of {'5mm': 0.5, '10mm': 0.5} targeting a 7mm separation point."

**🤖 AI Agent:**
> The recommended aperture size is 7.5mm, providing an effective open area of 0.65 and an expected passing fraction of 0.52.

---

**👤 You:**
> "Suggest a deck configuration for a total required area of 200 square meters with multi-stage separation."

**🤖 AI Agent:**
> A 3-deck configuration is recommended with a total area of 210 square meters and a total height of 4.5 meters.


## ❓ FAQ

**Q: How do I calculate the required screen area?**
You can use the `get_required_screen_area` tool by providing the feed rate, the particle size distribution, and your target efficiency.

**Q: Can I design multi-deck screen layouts?**
Yes, the `design_deck_configuration` tool allows you to specify if multi-stage separation is required to generate a suitable deck layout.

**Q: How do I ensure the material won't clog the screen?**
Use the `validate_bed_depth_compliance` tool to check if the material layer thickness is compatible with your aperture size and feed rate.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/screen-sizing-configuration](https://vinkius.com/en/ai-agent-connect/screen-sizing-configuration)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Screen Sizing & Configuration** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `screen-sizing-configuration` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Screen Sizing & Configuration** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "screen-sizing-configuration": {
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

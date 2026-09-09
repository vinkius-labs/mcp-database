# Vertical Mill Sizing MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/vertical-mill-sizing)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [engineering](../categories/engineering.md)

Calculate dimensions, power, and media charge for vertical stirred mills.

## Description
This MCP server provides specialized engineering tools for sizing vertical stirred mills like Vertimill or SMD. It allows AI agents to calculate critical parameters including mill diameter and height using `calculate_mill_dimensions`, determine electrical requirements with `calculate_power_requirement`, and optimize grinding media using `optimize_media_charge`. It also includes `evaluate_mill_efficiency` to assess performance against production targets.


## Available Tools (4)
- **calculate_mill_dimensions**: Determine the physical size (diameter and height) of the mill required to process a specific load
- **calculate_power_requirement**: Determine the electrical and mechanical power necessary to drive the mill
- **evaluate_mill_efficiency**: Assess how well a specific mill configuration meets the grinding target
- **optimize_media_charge**: Find the ideal mass and volume of grinding media to maximize grinding efficiency


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Vertical Mill Sizing** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What are the dimensions for a mill processing 50 tph of ore with a work index of 15, target size of 75 microns, and media density of 4500 kg/m3?"

**🤖 AI Agent:**
> The required mill dimensions are a diameter of 2.5 meters and a height of 4.2 meters, with a total volume of 21.1 m3.

---

**👤 You:**
> "How much power is needed for a 3m diameter, 5m high mill grinding ore with a work index of 12 at 15 rpm?"

**🤖 AI Agent:**
> The required power is 450 kW with a motor rating of 500 kW.

---

**👤 You:**
> "Calculate the optimal media charge for a mill with 2.5m diameter and 4m height for an ore with work index 14 and media density 4000 kg/m3."

**🤖 AI Agent:**
> The optimal media mass is 12,500 kg with a media volume of 3.125 m3, resulting in a fill level of 25%.


## ❓ FAQ

**Q: What parameters are needed for mill sizing?**
To use `calculate_mill_dimensions`, you need the ore work index, target product size, required throughput, and media density.

**Q: Can I optimize the media charge?**
Yes, the `optimize_media_charge` tool calculates the ideal mass and volume of grinding media to maximize efficiency.

**Q: How is power requirement calculated?**
The `calculate_power_requirement` tool determines power based on mill dimensions, ore hardness, target size, and agitator speed.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/vertical-mill-sizing](https://vinkius.com/ai-agent-connect/vertical-mill-sizing)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Vertical Mill Sizing** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vertical-mill-sizing` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Vertical Mill Sizing** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vertical-mill-sizing": {
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

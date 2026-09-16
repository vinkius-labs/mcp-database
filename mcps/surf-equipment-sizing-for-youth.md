# Surf Equipment Sizing for Youth MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/surf-equipment-sizing-for-youth)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Calculates surfboard dimensions, volume, and wetsuit sizes for youth surfers based on growth and skill.

## Description
This MCP server provides precise equipment recommendations for young surfers. By analyzing physical metrics like age, height, and weight alongside skill levels, it determines optimal surfboard dimensions and volume. It also identifies appropriate wetsuit sizes and uses pediatric growth models to project future equipment needs. Use `get_board_recommendation` for specific surfboard specs, `get_wetsuit_size` for thermal gear, `get_equipment_growth_trajectory` to plan for growth, and `get_skill_progression_guidance` to transition between skill tiers.


## Available Tools (4)
- **get_wetsuit_size**: Determines the appropriate wetsuit size for thermal protection and mobility
- **get_board_recommendation**: Provides specific surfboard dimensions and volume based on the surfer's physical stats and ability
- **get_equipment_growth_trajectory**: Estimates how much a surfer's equipment needs will change over a specific time horizon
- **get_skill_progression_guidance**: Recommends the next logical equipment step when a surfer is ready to move from one skill level to another


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Surf Equipment Sizing for Youth** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What surfboard should a 10-year-old boy who is 140cm tall and weighs 35kg use if he is a beginner?"

**🤖 AI Agent:**
> For a beginner with those stats, the recommended surfboard is 165cm long, 45cm wide, and 6cm thick, with a volume of 42.5 liters.

---

**👤 You:**
> "What wetsuit size is best for a 12-year-old girl, 150cm tall and 40kg?"

**🤖 AI Agent:**
> The recommended wetsuit size is M with a 3/2mm thickness.

---

**👤 You:**
> "I am an intermediate surfer using a 40L board. What is my next step?"

**🤖 AI Agent:**
> Your next target skill level is advanced, and you should look for a funboard with a volume range between 30L and 35L.


## ❓ FAQ

**Q: How accurate are the surfboard recommendations?**
The recommendations use specific youth-focused sizing formulas that correlate weight and skill level to ensure stability and performance.

**Q: Can I plan for my child's future growth?**
Yes, you can use the growth trajectory tool to estimate how much board volume and size will change over a set number of months.

**Q: Does it account for different skill levels?**
Yes, the tool adjusts volume and dimensions based on whether the surfer is a beginner, intermediate, or advanced user.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/surf-equipment-sizing-for-youth](https://vinkius.com/en/ai-agent-connect/surf-equipment-sizing-for-youth)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Surf Equipment Sizing for Youth** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `surf-equipment-sizing-for-youth` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Surf Equipment Sizing for Youth** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "surf-equipment-sizing-for-youth": {
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

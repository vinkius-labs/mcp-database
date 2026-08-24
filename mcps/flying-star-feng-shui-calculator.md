# Flying Star Feng Shui Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/flying-star-feng-shui-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Generate precise 3x3 Flying Star (Xuan Kong Fei Xing) charts and analyze auspicious sectors.

## Description
This MCP server provides professional-grade Xuan Kong Fei Xing (Flying Star Feng Shui) calculations. It allows AI agents to generate static 3x3 Lo Shu grids based on a building's construction period and sitting mountain. Users can use `calculate_period_chart` to establish the base energy, `analyze_auspicious_sectors` to identify wealth and health zones, and `overlay_annual_stars` to see how yearly energetic shifts impact the space. It bridges complex Feng Shui mathematics with AI reasoning for precise environmental analysis.


## Available Tools (3)
- **calculate_period_chart**: Generates the static 3x3 Flying Star grid for a building based on its construction period and orientation
- **analyze_auspicious_sectors**: Identifies specific areas in the building that are favorable or unfavorable based on the interaction of the stars
- **overlay_annual_stars**: Merges the current year's transient stars with the building's permanent period chart to show yearly shifts


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Flying Star Feng Shui Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Generate a period chart for a building in Period 9 sitting on the Zi mountain."

**🤖 AI Agent:**
> The 3x3 Flying Star grid for Period 9, Zi sitting, has been generated with the specific Mountain, Water, and Base star distributions for each palace.

---

**👤 You:**
> "Which sectors are good for wealth in my Period 8 building?"

**🤖 AI Agent:**
> Based on the Period 8 chart, the South sector is identified as a wealth sector due to the specific Water Star configuration.

---

**👤 You:**
> "How will the annual stars affect my house in 2024?"

**🤖 AI Agent:**
> The 2024 annual overlay shows that the wealth star has shifted to the East palace for this specific building configuration.


## ❓ FAQ

**Q: How do I determine my building's period?**
The period is determined by the year the building was constructed. For example, Period 9 covers the years 2024 to 2043.

**Q: What is the difference between Mountain and Water stars?**
The Mountain Star governs health and relationships, while the Water Star governs wealth and prosperity.

**Q: Can I see how the energy changes every year?**
Yes, you can use the `overlay_annual_stars` tool to see how the transient annual stars interact with your building's permanent period chart.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/flying-star-feng-shui-calculator](https://vinkius.com/ai-agent-connect/flying-star-feng-shui-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Flying Star Feng Shui Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `flying-star-feng-shui-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Flying Star Feng Shui Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "flying-star-feng-shui-calculator": {
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

# VTuber Name Fortune Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/vtuber-name-fortune-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [lifestyle](../categories/lifestyle.md)

Calculate VTuber debut potential using traditional Seimei Handan and modern persona alignment.

## Description
This MCP server connects AI agents to the ancient art of Seimei Handan, a traditional Japanese method of stroke-based fortune telling. By analyzing the stroke counts of a VTuber's stage name, the `calculate_name_fortune` tool calculates five essential luck grids: Heaven, Earth, Person, Outer, and Total. It also evaluates how well a name aligns with modern persona archetypes like 'idol' or 'gamer' through a specialized theme alignment matrix. Use `check_theme_compatibility` to verify if a chosen persona matches the name's energy, or `get_theme_definitions` to see available archetypes.


## Available Tools (3)
- **get_theme_definitions**: Get valid themes
- **calculate_name_fortune**: 
- **check_theme_compatibility**: Check theme compatibility


## 💬 Prompt Examples

Here are some examples of how you can interact with the **VTuber Name Fortune Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the fortune for a VTuber named with stroke counts [10, 5, 12] and an 'idol' theme."

**🤖 AI Agent:**
> { "go_grid_scores": { "heaven": 10, "earth": 15, "person": 27, "outer": 12, "total": 37 }, "theme_alignment_score": 95, "overall_debut_fortune": 80 }

---

**👤 You:**
> "Is a 'dragon' theme compatible with stroke counts [15, 8, 20]?"

**🤖 AI Agent:**
> { "is_compatible": true, "alignment_strength": "Perfect" }

---

**👤 You:**
> "What are the available lore themes?"

**🤖 AI Agent:**
> [ { "theme_name": "idol", "description": "High energy and popularity focused." }, { "theme_name": "dragon", "description": "Powerful and mythical presence." }, { "theme_name": "gamer", "description": "Skill and digital interaction focused." } ]


## ❓ FAQ

**Q: What is Seimei Handan?**
Seimei Handan is a traditional Japanese method of fortune telling that determines luck based on the number of strokes in Kanji characters, organized into five specific relationship grids.

**Q: How do I calculate my VTuber's debut fortune?**
You can use the `calculate_name_fortune` tool by providing the stroke counts of your stage name and your intended lore theme.

**Q: Can I check if my persona theme matches my name?**
Yes, the `check_theme_compatibility` tool is designed specifically to validate if a persona theme is mathematically compatible with your name's stroke structure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/vtuber-name-fortune-calculator](https://vinkius.com/ai-agent-connect/vtuber-name-fortune-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **VTuber Name Fortune Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `vtuber-name-fortune-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **VTuber Name Fortune Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "vtuber-name-fortune-calculator": {
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

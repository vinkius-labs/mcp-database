# Tabletop RPG Mechanics Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/tabletop-rpg-mechanics-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [gaming](../categories/gaming.md)

Deterministic mathematical resolution for TTRPG mechanics like D&D 5e.

## Description
A precise mathematical engine for tabletop roleplaying games. It provides deterministic calculations for ability modifiers using `resolve_ability_check`, simulates d20 outcomes with `simulate_roll_outcome`, calculates damage with `calculate_damage`, and manages resource depletion via `update_spell_slots`. It handles complex rules including resistance, vulnerability, and proficiency scaling.


## Available Tools (4)
- **calculate_damage**: Resolves the final damage value of an attack or spell
- **simulate_roll_outcome**: Determines the outcome of a d20 roll, accounting for advantage or disadvantage
- **update_spell_slots**: Manages the consumption of spell resources
- **resolve_ability_check**: Calculates the total modifier and the resulting proficiency bonus for a specific action


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tabletop RPG Mechanics Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total modifier for an ability score of 16 at level 5 with proficiency."

**🤖 AI Agent:**
> The ability modifier is +3 and the proficiency bonus is +3, resulting in a total modifier of +6.

---

**👤 You:**
> "What is the damage for 2d6+3 against a target with resistance?"

**🤖 AI Agent:**
> The damage range is 5 to 15, with an average of 10. With resistance, the final damage is 2 to 7.

---

**👤 You:**
> "Simulate a d20 roll with advantage."

**🤖 AI Agent:**
> The roll result is 17.


## ❓ FAQ

**Q: How does the engine handle advantage and disadvantage?**
The `simulate_roll_outcome` tool calculates the result by picking the highest value for advantage or the lowest value for disadvantage from two d20 rolls.

**Q: Can I calculate damage with resistances?**
Yes, the `calculate_damage` tool allows you to specify if a target has resistance or vulnerability to adjust the final damage value.

**Q: How are proficiency bonuses determined?**
Proficiency bonuses are determined by character level through the `resolve_ability_check` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/tabletop-rpg-mechanics-engine](https://vinkius.com/ai-agent-connect/tabletop-rpg-mechanics-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tabletop RPG Mechanics Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tabletop-rpg-mechanics-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tabletop RPG Mechanics Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tabletop-rpg-mechanics-engine": {
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

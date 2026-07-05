# RPG Damage Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/rpg-damage-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [gaming](../categories/gaming.md)

Calculate and analyze TTRPG damage distributions, critical hits, and encounter probabilities.

## Description
The RPG Damage Engine is a specialized computational tool for tabletop RPG players and game designers. It allows you to parse complex damage expressions like `2d6+3 fire` and instantly retrieve statistical insights including minimum, maximum, average, and standard deviation. The engine supports advanced combat mechanics such as D&D 5e and PF2e critical hit rules, advantage/disadvantage rolls, and elemental resistances or vulnerabilities. Use the `calculate_encounter_probability` tool to predict your success rate against high-HP enemies by simulating multi-attack distributions.


## Available Tools (4)
- **calculate_encounter_probability**: Predicts the probability of defeating an enemy
- **analyze_damage_expression**: Analyzes the statistical properties of a damage expression
- **evaluate_modified_damage**: Evaluates damage after applying modifiers and critical rules
- **parse_damage_expression**: Parses a damage expression into its components


## 💬 Prompt Examples

Here are some examples of how you can interact with the **RPG Damage Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze the damage for '1d12+5 piercing'."

**🤖 AI Agent:**
> For 1d12+5 piercing: Min: 6, Max: 17, Average: 11.5, Std Dev: 3.45.

---

**👤 You:**
> "What is the damage if I have advantage on '2d6+3 fire' with resistance to fire?"

**🤖 AI Agent:**
> With advantage and fire resistance (0.5 multiplier), the modified average damage is 5.75.

---

**👤 You:**
> "What's my chance of dealing at least 30 damage with 3 attacks of '1d8+4'?"

**🤖 AI Agent:**
> The probability of dealing 30 or more total damage across 3 attacks is approximately 0.24.


## ❓ FAQ

**Q: What damage expressions can I parse?**
You can use standard dice notation such as `1d8+4 slashing` or `2d6+3 fire`. The engine parses the quantity, die type, modifier, and damage type.

**Q: How do critical hits work?**
The engine supports `D&D_5E` (doubling dice) and `PF2E` (doubling the final result) rules. You can specify these using the `critRule` parameter.

**Q: Can I calculate the chance of killing a boss?**
Yes, by using `calculate_encounter_probability`, you can input your attack damage, number of attacks, and the enemy's HP to find your success probability.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/rpg-damage-engine](https://vinkius.com/mcp/rpg-damage-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **RPG Damage Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `rpg-damage-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **RPG Damage Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "rpg-damage-engine": {
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

# Encounter Difficulty Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/encounter-difficulty-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [gaming](../categories/gaming.md)

Calculate D&D 5e/PF2e combat difficulty, lethality risk, and encounter adjustments.

## Description
Determine the intensity of your tabletop RPG encounters using precise XP-based calculations. This tool analyzes monster experience points (XP), party level, and group size to classify combat into Easy, Medium, Hard, or Deadly tiers. By applying encounter multipliers based on the number of creatures present, it provides an accurate 'Adjusted XP' value. Use `analyze_encounter` for a full breakdown including TPK risk estimation and specific recommendations for adjusting monster counts or values to reach your target difficulty.


## Available Tools (3)
- **analyze_encounter**: Performs a complete analysis of a combat encounter
- **get_party_thresholds**: Retrieves the XP budget boundaries for different difficulty tiers
- **lookup_encounter_multiplier**: Retrieves the specific scaling factor used to adjust XP


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Encounter Difficulty Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Analyze an encounter with two CR 3 monsters (450 XP each) and one CR 5 monster (1800 XP) for a party of 4 players at level 5."

**🤖 AI Agent:**
> The encounter difficulty is Medium. The Adjusted XP is 2700, with a Moderate TPK risk. To reach a Hard tier, consider adding more creatures or increasing the monster XP.

---

**👤 You:**
> "What is the multiplier for an encounter with 6 monsters?"

**🤖 AI Agent:**
> The encounter multiplier for 6 creatures is 2.0.

---

**👤 You:**
> "What are the XP thresholds for a party of 5 players at level 10?"

**🤖 AI Agent:**
> For a level 10 party of 5, the thresholds are: Easy up to 1200 XP, Medium up to 2400 XP, Hard up to 3600 XP, and anything above 3600 XP is Deadly.


## ❓ FAQ

**Q: How is the encounter difficulty determined?**
The tool calculates 'Adjusted XP' by summing the base XP of all monsters (multiplied by their count) and then applying an encounter multiplier based on the total number of creatures. This value is compared against thresholds for your specific party level and size.

**Q: What does 'TPK Risk' mean?**
Total Party Kill (TPK) risk is an estimation of the likelihood that all player characters will be defeated. It increases as the encounter's Adjusted XP moves into the 'Deadly' range.

**Q: Can I use this for both D&D 5e and Pathfinder 2e?**
Yes, the calculation engine is designed to work with the XP-based systems used in both D&D 5e and PF2e.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/encounter-difficulty-calculator](https://vinkius.com/mcp/encounter-difficulty-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Encounter Difficulty Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `encounter-difficulty-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Encounter Difficulty Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "encounter-difficulty-calculator": {
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

# BaZi Four Pillars Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/bazi-four-pillars-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Calculate precise Chinese BaZi Four Pillars, Day Master, and elemental balance.

## Description
This MCP server provides deterministic calculations for the Chinese BaZi (Four Pillars of Destiny) system. It allows AI agents to derive the core eight characters from birth data, identify the Day Master, analyze the elemental distribution (Wood, Fire, Earth, Metal, Water), and project 10-year Luck Pillars. Use `calculate_four_pillars` to get the primary pillars, `analyze_elemental_composition` to check for missing elements, and `calculate_luck_pillars` to map life cycles.


## Available Tools (3)
- **analyze_elemental_composition**: Determine the elemental balance and identify missing elements from a set of pillars
- **calculate_four_pillars**: Derive the core eight characters (Four Pillars) from a specific birth moment
- **calculate_luck_pillars**: Project the 10-year cycles of fate following birth


## 💬 Prompt Examples

Here are some examples of how you can interact with the **BaZi Four Pillars Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my BaZi pillars for a male born on July 4, 1990, at 14:30."

**🤖 AI Agent:**
> Your Year Pillar is Metal Horse, Month Pillar is Water Horse, Day Pillar is Wood Dragon, and Hour Pillar is Earth Goat. Your Day Master is Wood.

---

**👤 You:**
> "What is the elemental balance for these pillars: Year: Wood Rat, Month: Fire Ox, Day: Earth Tiger, Hour: Metal Rabbit?"

**🤖 AI Agent:**
> Your elemental distribution is: Wood: 2, Fire: 1, Earth: 2, Metal: 1, Water: 1. You have a balanced elemental profile.

---

**👤 You:**
> "Calculate the luck pillars for a female born with Year Stem: Water, Year Branch: Dragon, and Day Master Element: Fire."

**🤖 AI Agent:**
> Your first Luck Pillar starts in 1995 with the combination of Wood Tiger.


## ❓ FAQ

**Q: What is the Day Master?**
The Day Master is the Heavenly Stem of the Day Pillar, representing your core identity in BaZi.

**Q: How are the Luck Pillars calculated?**
Luck Pillars are 10-year cycles calculated using the Year Pillar, gender, and Day Master element via `calculate_luck_pillars`.

**Q: Can I analyze my elemental balance?**
Yes, use `analyze_elemental_composition` with the output from the pillar calculation to see your elemental counts.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/bazi-four-pillars-calculator](https://vinkius.com/ai-agent-connect/bazi-four-pillars-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **BaZi Four Pillars Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bazi-four-pillars-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **BaZi Four Pillars Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bazi-four-pillars-calculator": {
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

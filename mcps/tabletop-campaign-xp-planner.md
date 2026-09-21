# Tabletop Campaign XP Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tabletop-campaign-xp-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Simulate character progression, track XP, and project leveling timelines for RPG parties.

## Description
This MCP server provides Game Masters with precision tools to manage tabletop role-playing game progression. Use `calculate_party_progress` to get a snapshot of current levels and XP status for all members. Simulate combat or social rewards with `simulate_encounter_reward` to see how difficulty multipliers affect individual gains. Forecast future milestones using `project_leveling_timeline` to estimate how many sessions remain until the next level. Finally, manage narrative achievements with `allocate_milestone_xp` to distribute large rewards using equal or level-weighted rules.


## Available Tools (4)
- **allocate_milestone_xp**: Handles the distribution of large, narrative-driven XP rewards
- **calculate_party_progress**: Provides a comprehensive snapshot of the current XP status for both individuals and the group
- **project_leveling_timeline**: Predicts when the party will reach specific future levels
- **simulate_encounter_reward**: Calculates the XP gained from a specific event and applies it to the party


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tabletop Campaign XP Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the current progress of my party?"

**🤖 AI Agent:**
> The party has a total of 4,500 XP. Character A is level 3 (80% to level 4), Character B is level 2 (45% to level 3), and Character C is level 2 (10% to level 3).

---

**👤 You:**
> "How much XP will the party get from a hard encounter with 1500 base XP for 4 players?"

**🤖 AI Agent:**
> With a hard difficulty multiplier of 2.0, the total XP gained is 3,000. Each of the 4 players will receive 750 XP.

---

**👤 You:**
> "When will the party reach level 5?"

**🤖 AI Agent:**
> Based on your average of 500 XP per session and playing once a week, the party is estimated to reach level 5 in 4 sessions (approximately 4 weeks).


## ❓ FAQ

**Q: How does the XP distribution work?**
You can use `simulate_encounter_reward` for standard encounters or `allocate_milestone_xp` for narrative milestones. The latter allows for equal or level-weighted distribution to ensure fair progression.

**Q: Can I predict when my players will level up?**
Yes, by using `project_leveling_timeline`, you can estimate the number of sessions, weeks, or days required to reach a specific target level based on your average XP per session.

**Q: How do I check the current status of my party?**
The `calculate_party_progress` tool provides a detailed report including current levels, XP needed for the next level, and progress percentages for every character.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tabletop-campaign-xp-planner](https://vinkius.com/en/ai-agent-connect/tabletop-campaign-xp-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tabletop Campaign XP Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tabletop-campaign-xp-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tabletop Campaign XP Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tabletop-campaign-xp-planner": {
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

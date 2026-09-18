# Spice Level Adjuster MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/spice-level-adjuster)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Scale recipe heat and manage spice tolerance using Scoville Heat Units.

## Description
This MCP server provides a specialized calculation engine for adjusting recipe heat profiles. It allows AI agents to precisely scale ingredient quantities to meet specific Scoville Heat Unit (SHU) targets, find equivalent heat substitutes for different ingredients, and generate structured progression plans for building spice tolerance. Use `calculate_adjusted_recipe` to rebalance a recipe, `find_equivalent_heat_substitutes` to swap ingredients without changing heat, or `get_tolerance_progression_plan` to safely increase heat capacity over time.


## Available Tools (4)
- **analyze_heat_distribution**: Breaks down the heat contribution of each ingredient to identify the primary heat drivers in a recipe
- **calculate_adjusted_recipe**: Adjusts the quantities of all spicy ingredients in a recipe to meet a specific target heat level
- **find_equivalent_heat_substitutes**: Finds how much of a new ingredient is needed to replace an existing one while keeping the heat level identical
- **get_tolerance_progression_plan**: Generates a multi-stage plan to gradually increase a user's spice tolerance


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Spice Level Adjuster** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I have a recipe with 2 units of Jalapeño (2500 SHU) and 1 unit of Cayenne (50000 SHU). How much should I use to reach a target of 30000 SHU?"

**🤖 AI Agent:**
> To reach a target of 30,000 SHU, you should use 2 units of Jalapeño and 0.5 units of Cayenne.

---

**👤 You:**
> "I want to replace 3 units of a pepper with 1000 SHU with a pepper that has 5000 SHU. How much of the new pepper do I need?"

**🤖 AI Agent:**
> You will need 0.6 units of the 5000 SHU pepper to maintain the same heat level.

---

**👤 You:**
> "Create a plan to go from 5000 SHU to 15000 SHU in steps of 2000."

**🤖 AI Agent:**
> Your progression plan is: Stage 1: 7000 SHU, Stage 2: 9000 SHU, Stage 3: 11000 SHU, Stage 4: 13000 SHU, Stage 5: 15000 SHU.


## ❓ FAQ

**Q: How does the scaling work?**
The engine uses a linear scaling factor based on Scoville Heat Units (SHU). By calculating the current cumulative heat and comparing it to your target, it determines the exact multiplier needed for each ingredient via `calculate_adjusted_recipe`.

**Q: Can I swap a jalapeño for a habanero?**
Yes. You can use `find_equivalent_heat_substitutes` to calculate exactly how much of a habanero you need to provide the same heat contribution as the original jalapeño.

**Q: How do I safely increase my heat tolerance?**
You can use `get_tolerance_progression_plan` to generate a multi-stage plan that increases your target Scoville level in controlled increments.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/spice-level-adjuster](https://vinkius.com/en/ai-agent-connect/spice-level-adjuster)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Spice Level Adjuster** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `spice-level-adjuster` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Spice Level Adjuster** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "spice-level-adjuster": {
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

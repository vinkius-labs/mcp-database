# Dinner Leftover Portion Planner MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/dinner-leftover-portion-planner)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Divide cooked meals into dinner, lunches, freezer portions, and reserves.

## Description
This MCP server helps you manage meal yields by calculating how to distribute a single cooked dish across immediate consumption, packed lunches, long-term freezer storage, and emergency reserves. Use `calculate_portion_distribution` to split your total yield, `validate_yield_capacity` to check if you have enough food for your plans, `suggest_optimal_reserve` to find a safe buffer, and `get_storage_category_summary` to organize portions by storage type.


## Available Tools (4)
- **calculate_portion_distribution**: Determines how much food should be assigned to each category based on user preferences and total food available
- **get_storage_category_summary**: Groups the planned portions into storage-type buckets
- **suggest_optimal_reserve**: Calculates a recommended reserve amount based on the number of diners and intended lunches
- **validate_yield_capacity**: Checks if a planned meal volume is sufficient for a specific set of requirements


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Dinner Leftover Portion Planner** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I made 10 portions of lasagna. 4 people are eating tonight, and I want 2 lunches for tomorrow. How should I distribute the rest?"

**🤖 AI Agent:**
> With 10 portions total, you can serve 4 people tonight, pack 2 lunches, and you will have 4 portions remaining for the freezer or reserve.

---

**👤 You:**
> "I have 5 portions of chicken. Can I feed 3 people tonight and have 3 lunches ready?"

**🤖 AI Agent:**
> No, you only have 5 portions available, which is not enough to cover 3 diners and 3 lunches (6 portions total).

---

**👤 You:**
> "I have 8 portions of stew. Suggest a reserve amount for me."

**🤖 AI Agent:**
> A recommended reserve for your 8 portions is 0.8 portions (10% buffer).


## ❓ FAQ

**Q: How do I know if I have enough food for everyone?**
You can use the `validate_yield_capacity` tool to check if your total food volume is sufficient for your planned diners and lunch portions.

**Q: Can I calculate how much to put in the freezer?**
Yes, `calculate_portion_distribution` allows you to specify exactly how many portions you want to set aside for the freezer.

**Q: How much reserve should I keep?**
The `suggest_optimal_reserve` tool can recommend a safe buffer based on your total yield and the number of people eating.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/dinner-leftover-portion-planner](https://vinkius.com/en/ai-agent-connect/dinner-leftover-portion-planner)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Dinner Leftover Portion Planner** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `dinner-leftover-portion-planner` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Dinner Leftover Portion Planner** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "dinner-leftover-portion-planner": {
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

# Wine Menu Placement Optimizer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/wine-menu-placement-optimizer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [business-intelligence](../categories/business-intelligence.md)

Analyze wine menu positioning to optimize sales using menu engineering.

## Description
This MCP server provides strategic analysis tools for restaurant managers to optimize wine menu performance. By applying menu engineering principles, it evaluates how wine placement affects consumer behavior. Use `analyze_wine_position` to calculate visibility scores and sales probability for specific items, or `calculate_menu_health` to categorize your offerings into Stars, Plowhorses, Puzzles, and Dogs. For actionable improvements, `recommend_placement_optimization` suggests specific structural changes to maximize profit or volume based on your current menu layout.


## Available Tools (4)
- **calculate_menu_health**: Provides a high-level overview of a menu's performance based on sales and profitability data
- **get_menu_benchmarks**: Retrieves standardized visibility and performance thresholds for different menu types
- **analyze_wine_position**: Evaluates the strategic effectiveness of a specific wine's placement on a menu
- **recommend_placement_optimization**: Suggests specific structural changes to the menu to improve the performance of "Puzzle" or "Dog" items


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Wine Menu Placement Optimizer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How is the placement of the first wine in my by-glass menu performing?"

**🤖 AI Agent:**
> The wine at position 0 has a high visibility score due to the Primacy effect, resulting in a high sales probability.

---

**👤 You:**
> "Analyze my menu health with this data: [{"volume": 50, "margin": 20}, {"volume": 10, "margin": 45}] and type 'by-glass'."

**🤖 AI Agent:**
> Your menu contains 1 Plowhorse and 1 Puzzle item, with an overall performance score of 0.75.

---

**👤 You:**
> "What are the ideal margin thresholds for a bottle list?"

**🤖 AI Agent:**
> For a bottle list, the ideal margin threshold is 0.45 and the optimal position range is [0, 2].


## ❓ FAQ

**Q: How can I improve my high-margin wines that aren't selling?**
You can use `recommend_placement_optimization` to identify high-margin 'Puzzle' items and receive specific suggestions on moving them to high-visibility positions like Prime zones.

**Q: What is a visibility score?**
The visibility score, provided by `analyze_wine_position`, is a metric representing the visual impact of a wine's position based on psychological effects like Primacy and Recency.

**Q: Can I analyze both by-glass and bottle lists?**
Yes, all tools such as `get_menu_benchmarks` and `calculate_menu_health` are designed to handle both 'by-glass' and 'bottle-list' menu types.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/wine-menu-placement-optimizer](https://vinkius.com/en/ai-agent-connect/wine-menu-placement-optimizer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Wine Menu Placement Optimizer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `wine-menu-placement-optimizer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Wine Menu Placement Optimizer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "wine-menu-placement-optimizer": {
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

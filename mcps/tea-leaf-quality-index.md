# Tea Leaf Quality Index MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/tea-leaf-quality-index)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [agriculture](../categories/agriculture.md)

Calculate optimal plucking intervals and expected cup quality scores for tea harvests.

## Description
This MCP server provides precise analytical tools for tea plantation management. It connects AI agents to chemical and biological data to determine the best time for harvesting. Use `calculate_plucking_metrics` to find the ideal plucking interval and expected quality score based on leaf position, shoot age, and chemical composition. You can also use `predict_grade_distribution` to forecast commercial grade percentages or `evaluate_black_tea_potential` to analyze the theaflavin and thearubigin ratio for black tea production.


## Available Tools (3)
- **calculate_plucking_metrics**: Determines the ideal timing and expected quality of a harvest based on current leaf state
- **evaluate_black_tea_potential**: Specifically analyzes the oxidation potential for black tea production
- **predict_grade_distribution**: Forecasts the percentage of leaves that will fall into specific commercial grades


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tea Leaf Quality Index** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the expected quality score for a 10-day old shoot at the apical position with 50 units of polyphenols, 10 caffeine, and 20 amino acids for black tea?"

**🤖 AI Agent:**
> The expected cup quality score for this shoot is 85/100, with an optimum plucking interval of 3 days.

---

**👤 You:**
> "Predict the grade distribution for a mid-position shoot that is 15 days old for green tea with a seasonal factor of 1.0."

**🤖 AI Agent:**
> The predicted distribution is 60% premium grade, 30% standard grade, and 10% low grade.

---

**👤 You:**
> "Analyze the black tea potential for 80 units of polyphenols with a nitrogen level of 5."

**🤖 AI Agent:**
> The analysis shows a theaflavin potential of 0.65 and a thearubigin potential of 0.35, resulting in a quality ratio of 1.85.


## ❓ FAQ

**Q: How can I determine the best time to harvest my tea?**
You can use the `calculate_plucking_metrics` tool. By providing the leaf position, shoot age, and chemical composition, the tool returns the optimum plucking interval and an expected cup quality score.

**Q: Can I predict the commercial grade of my tea leaves?**
Yes, the `predict_grade_distribution` tool allows you to forecast the percentage of premium, standard, and low grade leaves based on shoot maturity and seasonal factors.

**Q: How does this tool help with black tea production?**
The `evaluate_black_tea_potential` tool specifically analyzes the oxidation potential by calculating the ratio of theaflavin and thearubigin based on polyphenol levels.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/tea-leaf-quality-index](https://vinkius.com/ai-agent-connect/tea-leaf-quality-index)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tea Leaf Quality Index** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tea-leaf-quality-index` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tea Leaf Quality Index** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tea-leaf-quality-index": {
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

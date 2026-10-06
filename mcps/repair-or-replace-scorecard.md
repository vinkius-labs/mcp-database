# Repair or Replace Scorecard MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/repair-or-replace-scorecard)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [sustainability](../categories/sustainability.md)

Rank repair and replacement options using weighted multi-factor scoring.

## Description
This MCP server provides a strategic decision-making framework for facilities management and asset lifecycle planning. It allows AI agents to evaluate whether to maintain an existing asset or purchase a new one by analyzing multiple dimensions. Using the `calculate_scores` tool, agents can rank candidates based on repair cost, expected life, new-item cost, material factor, and energy factor. The server also includes `validate_weights` to ensure mathematical consistency, `summarize_decision` for qualitative recommendations, and `filter_options` to apply budget or longevity constraints.


## Available Tools (4)
- **filter_options**: Narrows down potential options based on budget or life constraints
- **summarize_decision**: Provides a high-level qualitative recommendation based on rankings
- **validate_weights**: Ensures user-provided priority settings are mathematically sound
- **calculate_scores**: Weights must sum to 1.0.

Generates a ranked list of options based on provided candidates and user weights


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Repair or Replace Scorecard** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Rank these options: Option A (Repair: 500, Life: 5, New: 2000, Material: 0.8, Energy: 0.7) and Option B (Repair: 1500, Life: 8, New: 2200, Material: 0.9, Energy: 0.9) with weights: {repairCost: 0.2, expectedLife: 0.3, newItemCost: 0.2, materialFactor: 0.15, energyFactor: 0.15}."

**🤖 AI Agent:**
> Option B is the recommended choice with a total score of 0.78, outperforming Option A which scored 0.62.

---

**👤 You:**
> "I have a budget of $1000. Which of these options are available: Option 1 (Repair: 800, Life: 3), Option 2 (Repair: 1200, Life: 4), Option 3 (New: 1500, Life: 10)?"

**🤖 AI Agent:**
> The available option within your $1000 budget is Option 1.

---

**👤 You:**
> "Are these weights valid: {repairCost: 0.5, expectedLife: 0.5}?"

**🤖 AI Agent:**
> Yes, the weights are valid as they sum to 1.0.


## ❓ FAQ

**Q: How do I ensure my priority weights are correct?**
You can use the `validate_weights` tool to verify that your priority multipliers are non-negative and sum exactly to 1.0.

**Q: Can I filter options by a specific budget?**
Yes, the `filter_options` tool allows you to narrow down candidates based on a maximum budget or a minimum required expected life.

**Q: What does the final recommendation tell me?**
The `summarize_decision` tool provides a qualitative recommendation and a confidence level based on the gap between the top-ranked option and the next best choice.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/repair-or-replace-scorecard](https://vinkius.com/en/ai-agent-connect/repair-or-replace-scorecard)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Repair or Replace Scorecard** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `repair-or-replace-scorecard` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Repair or Replace Scorecard** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "repair-or-replace-scorecard": {
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

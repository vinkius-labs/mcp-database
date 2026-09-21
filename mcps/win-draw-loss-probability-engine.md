# Win-Draw-Loss Probability Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/win-draw-loss-probability-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [mathematics](../categories/mathematics.md)

Aggregates football scoreline matrices into match outcome probabilities and fair decimal odds.

## Description
This MCP server provides mathematical tools to transform granular football scoreline matrices into primary match outcomes. Use `aggregate_outcomes` to convert specific scoreline probabilities into Home Win, Draw, and Away Win totals. You can use `validate_matrix_completeness` to ensure a scoreline distribution is mathematically complete, or `calculate_fair_odds` to derive decimal odds from known probabilities. Finally, `get_outcome_summary` provides a text-based overview of match likelihoods.


## Available Tools (4)
- **aggregate_outcomes**: Each object must have homeGoals, awayGoals, and probability.

Transforms a matrix of specific scorelines into primary match outcome probabilities
- **calculate_fair_odds**: Determines the mathematically fair decimal odds for each primary match outcome
- **get_outcome_summary**: Provides a high-level text-based summary of match likelihoods and potential value
- **validate_matrix_completeness**: Verifies if a provided scoreline matrix represents a complete probability distribution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Win-Draw-Loss Probability Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Aggregate these scorelines: [{"homeGoals": 1, "awayGoals": 0, "probability": 0.4}, {"homeGoals": 0, "awayGoals": 0, "probability": 0.6}]"

**🤖 AI Agent:**
> Home Win: 0.4, Draw: 0.6, Away Win: 0.0. The total probability is conserved.

---

**👤 You:**
> "Calculate fair odds for a home win probability of 0.5, draw of 0.2, and away win of 0.3."

**🤖 AI Agent:**
> The fair decimal odds are: Home Win: 2.0, Draw: 5.0, Away Win: 3.33.

---

**👤 You:**
> "Is this matrix complete: [{"homeGoals": 1, "awayGoals": 0, "probability": 0.5}]?"

**🤖 AI Agent:**
> No, the matrix is incomplete. The missing probability is 0.5.


## ❓ FAQ

**Q: How do I convert scorelines to match outcomes?**
You can use the `aggregate_outcomes` tool by providing a JSON array of scoreline objects containing home goals, away goals, and their respective probabilities.

**Q: Can I calculate betting odds with this server?**
Yes, the `calculate_fair_odds` tool calculates the mathematically fair decimal odds for Home Win, Draw, and Away Win based on provided probabilities.

**Q: What happens if the probability sum is not 1.0?**
The `validate_matrix_completeness` tool will detect if the sum is not 1.0 and will report the missing probability as a 'No-Result' state.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/win-draw-loss-probability-engine](https://vinkius.com/en/ai-agent-connect/win-draw-loss-probability-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Win-Draw-Loss Probability Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `win-draw-loss-probability-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Win-Draw-Loss Probability Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "win-draw-loss-probability-engine": {
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

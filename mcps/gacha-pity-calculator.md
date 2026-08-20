# Gacha Pity Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/gacha-pity-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Calculate exact gacha probabilities, soft pity escalation, and resource costs.

## Description
This MCP server provides deterministic probability modeling for gacha loot box systems. It helps users navigate complex pity mechanics common in mobile games. Use `calculate_single_pull_odds` to find the immediate chance of success, `calculate_cumulative_projections` to estimate total currency costs and success rates over multiple pulls, or `check_pity_status` to determine if a featured character is guaranteed via the 50/50 mechanic.


## Available Tools (3)
- **calculate_single_pull_odds**: Determines the specific probability of success for the very next pull based on the current state of the pity counter
- **check_pity_status**: Evaluates the user's current standing regarding "guaranteed" featured items (the 50/50 mechanic)
- **calculate_cumulative_projections**: Projects the likelihood of success and resource requirements over a user-defined number of future pulls


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gacha Pity Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my chance of getting a 5-star on my next pull if I am at 74 pity, the base rate is 0.6%, soft pity starts at 74, hard pity is 90, and the increment is 6%?"

**🤖 AI Agent:**
> Your probability of success on the next pull is 6.6%.

---

**👤 You:**
> "How much will it cost to do 50 more pulls if each pull costs 160 gems, with a base rate of 0.6%, soft pity at 74, hard pity at 90, and increment of 6%? I am currently at 0 pity."

**🤖 AI Agent:**
> The total cost for 50 pulls is 8,000 gems, and your cumulative probability of success is approximately 32.8%.

---

**👤 You:**
> "Am I guaranteed the featured character next time I hit a 5-star?"

**🤖 AI Agent:**
> Yes, you are currently in a Guaranteed state.


## ❓ FAQ

**Q: How do I calculate my next pull chance?**
You can use the `calculate_single_pull_odds` tool. Provide your current pity counter, the base rate, and the soft/hard pity thresholds to get the exact probability.

**Q: Can I estimate how much currency I need for a banner?**
Yes, use `calculate_cumulative_projections` to see the total cost and the cumulative probability of success for a specific number of pulls.

**Q: What is the 50/50 mechanic?**
The 50/50 mechanic determines if your next high-rarity pull is the featured character. You can use `check_pity_status` to see if you are currently in a 'Guaranteed' state.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/gacha-pity-calculator](https://vinkius.com/ai-agent-connect/gacha-pity-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gacha Pity Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gacha-pity-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gacha Pity Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gacha-pity-calculator": {
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

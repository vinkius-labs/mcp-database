# Bridge Scoring Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/bridge-scoring-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [utilities](../categories/utilities.md)

Deterministic duplicate bridge scoring for contract results, trick points, bonuses, and penalties.

## Description
This MCP server provides a deterministic scoring engine for duplicate bridge. It calculates precise contract results, trick scores based on suit tiers, fixed bonuses for games and slams, and penalties for undertricks. Use `calculate_contract_result` to check if a contract was made, `calculate_trick_points` for suit-based scoring, `calculate_bonuses` for game/slam rewards, and `calculate_penalties` for defender scores when a contract fails.


## Available Tools (4)
- **calculate_bonuses**: Calculates fixed bonuses for making a Game or a Slam
- **calculate_contract_result**: Determines if the contract was successful or failed and by how many tricks
- **calculate_penalties**: Calculates the penalty score awarded to the defenders when a contract is not made
- **calculate_trick_points**: Calculates the score derived solely from the tricks won


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Bridge Scoring Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Was the 4♠ contract made if 10 tricks were taken?"

**🤖 AI Agent:**
> Yes, the contract was made with 1 extra trick.

---

**👤 You:**
> "Calculate the trick points for a 3NT contract where 9 tricks were taken."

**🤖 AI Agent:**
> The trick score is 120 points.

---

**👤 You:**
> "What is the penalty for a 3♥ contract being down 1 trick when not vulnerable?"

**🤖 AI Agent:**
> The penalty is 50 points.


## ❓ FAQ

**Q: How does the engine handle doubled or redoubled contracts?**
The engine applies multipliers to trick scores and bonuses for doubled contracts, and higher multipliers for redoubled contracts, as well as increasing penalties for undertricks.

**Q: Can I calculate penalties for undertricks?**
Yes, you can use the `calculate_penalties` tool to determine the score awarded to defenders based on the number of undertricks and vulnerability.

**Q: What suits are supported?**
The engine supports clubs, diamonds, hearts, spades, and no trump (nt).


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/bridge-scoring-engine](https://vinkius.com/ai-agent-connect/bridge-scoring-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Bridge Scoring Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `bridge-scoring-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Bridge Scoring Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "bridge-scoring-engine": {
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

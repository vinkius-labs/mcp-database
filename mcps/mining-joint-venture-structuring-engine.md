# Mining Joint Venture Structuring Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/mining-joint-venture-structuring-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Design and simulate mining joint venture agreements by modeling capital, equity, and governance.

## Description
This MCP server provides a specialized engine for designing and simulating mining joint venture (JV) agreements. It allows users to model complex financial and legal structures by calculating baseline ownership via `calculate_equity_distribution`, simulating incremental equity gains through `model_earn_in_pathway`, and assessing the impact of capital calls using `simulate_dilution_event`. Additionally, it evaluates the balance of power through `analyze_governance_structure` to ensure control rights align with ownership interests. It is an essential tool for mining operators and investors to reach equitable agreements.


## Available Tools (4)
- **analyze_governance_structure**: Evaluate the balance of power and control rights within the JV
- **model_earn_in_pathway**: Simulate how a party's ownership evolves as they meet milestones
- **calculate_equity_distribution**: Determine baseline ownership interest based on capital and asset contributions
- **simulate_dilution_event**: Calculate the impact on all partners when a capital call occurs


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Mining Joint Venture Structuring Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the initial ownership for Party A contributing 600k and Party B contributing 400k."

**🤖 AI Agent:**
> Party A holds a 60% ownership interest and Party B holds a 40% ownership interest.

---

**👤 You:**
> "What happens to ownership if Party A has 50% and we have a 100k capital call where only Party B contributes 100k?"

**🤖 AI Agent:**
> After the capital call, Party B's ownership increases and Party A's ownership is diluted based on the new total capital base.

---

**👤 You:**
> "Check if a party with 30% interest can pass a decision that requires a 40% threshold."

**🤖 AI Agent:**
> No, the party with 30% interest cannot pass the decision as it falls below the required 40% threshold.


## ❓ FAQ

**Q: How does the engine handle ownership changes?**
The engine uses `simulate_dilution_event` to calculate how ownership percentages shift when new capital is introduced and certain partners do not contribute to a capital call.

**Q: Can I model earn-in agreements?**
Yes, you can use `model_earn_in_pathway` to simulate how a party's ownership evolves as they meet specific performance or capital milestones.

**Q: How is governance analyzed?**
The `analyze_governance_structure` tool evaluates the balance of power by mapping voting rules and specific control rights to the JV structure.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/mining-joint-venture-structuring-engine](https://vinkius.com/en/ai-agent-connect/mining-joint-venture-structuring-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Mining Joint Venture Structuring Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `mining-joint-venture-structuring-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Mining Joint Venture Structuring Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "mining-joint-venture-structuring-engine": {
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

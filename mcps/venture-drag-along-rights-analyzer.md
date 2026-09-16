# Venture Drag-Along Rights Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-drag-along-rights-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates the impact of drag-along provisions on shareholder value and exit scenarios.

## Description
This MCP server provides specialized tools for analyzing drag-along rights in shareholder agreements. It allows AI agents to determine if a majority group can force a sale using `calculate_drag_impact`, assess the economic outcome for non-participating holders with `evaluate_minority_value`, and identify potential blockers via `analyze_veto_risk`. It also enables complex modeling of multiple exit possibilities through `simulate_exit_scenarios` to find the most lucrative outcomes for drag parties.


## Available Tools (4)
- **analyze_veto_risk**: 
- **simulate_exit_scenarios**: 
- **calculate_drag_impact**: 
- **evaluate_minority_value**: 


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Drag-Along Rights Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "If the drag threshold is 60% and the founders own 65%, what is the impact of a $50M sale with a 5% min price protection?"

**🤖 AI Agent:**
> The drag-along is triggered. The negotiation leverage is High, and the sale can proceed.

---

**👤 You:**
> "A minority holder has 5,000 shares out of 100,000 total. If the sale price is $10M and there is no minimum price protection, what is their payout?"

**🤖 AI Agent:**
> The expected payout for the minority shareholder is $500,000.

---

**👤 You:**
> "Analyze the risk if the drag threshold is 75% but the required consent for a sale is 30% and minority holders own 26%."

**🤖 AI Agent:**
> Veto power exists, and the risk level is High because the drag parties cannot act alone.


## ❓ FAQ

**Q: How can I determine if a sale will be forced?**
You can use the `calculate_drag_impact` tool by providing the drag threshold and the ownership percentage of the initiating group.

**Q: Can I calculate the specific payout for a minority holder?**
Yes, the `evaluate_minority_value` tool calculates the expected payout, accounting for any minimum price protections.

**Q: How do I check if minority shareholders can block a sale?**
Use the `analyze_veto_risk` tool to assess if the required consent thresholds allow minority holders to exercise veto power.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-drag-along-rights-analyzer](https://vinkius.com/en/ai-agent-connect/venture-drag-along-rights-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Drag-Along Rights Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-drag-along-rights-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Drag-Along Rights Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-drag-along-rights-analyzer": {
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

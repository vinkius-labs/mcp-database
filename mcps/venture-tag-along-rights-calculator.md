# Venture Tag-Along Rights Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-tag-along-rights-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates financial protection value and liquidity benefits of tag-along rights during co-sale opportunities.

## Description
This MCP server provides specialized tools for venture capital and private equity professionals to quantify the impact of tag-along rights. By connecting AI agents to precise financial models, it enables the calculation of protection value, liquidity benefits, and negotiation leverage during exit events. Use `simulate_exit_scenario` to model a complete transaction, or `calculate_protection_value` to determine the specific dollar amount gained by protected shareholders when a majority holder exits.


## Available Tools (4)
- **calculate_protection_value**: Determines the specific dollar amount of value gained by protected shareholders through the exercise of tag-along rights
- **simulate_exit_scenario**: Provides a comprehensive overview of a potential exit event by combining protection, liquidity, and leverage metrics
- **evaluate_liquidity_impact**: Analyzes how much the tag-along right improves the exit timing and ease of liquidation for the protected shareholder
- **determine_negotiation_leverage**: Assesses the strategic position of the protected shareholder based on the trigger conditions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Tag-Along Rights Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the protection value for 50,000 shares if the majority holder is selling at $15.00 per share with a 10% tag threshold."

**🤖 AI Agent:**
> The protection value for the 50,000 shares at a price of $15.00 per share is $750,000.00.

---

**👤 You:**
> "What is the negotiation priority if the tag threshold is 5% and the majority stake is 60%?"

**🤖 AI Agent:**
> The negotiation priority is High due to the low 5% trigger threshold, providing significant strategic advantage.

---

**👤 You:**
> "Simulate an exit where 100,000 shares are sold at $20.00 per share with a 15% threshold and 50,000 protected shares."

**🤖 AI Agent:**
> The simulated exit results in a total protection value of $1,000,000.00 with a significant liquidity benefit.


## ❓ FAQ

**Q: What is the purpose of the `calculate_protection_value` tool?**
It determines the specific dollar amount of value gained by protected shareholders when they exercise their right to participate in a majority shareholder's exit.

**Q: How can I model a full exit event?**
You can use the `simulate_exit_scenario` tool, which aggregates protection, liquidity, and leverage metrics into a single decision-support object.

**Q: Does this tool account for the trigger threshold?**
Yes, the tools require the `tagThreshold` to ensure the calculation respects the specific percentage of ownership that must be sold to trigger the rights.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-tag-along-rights-calculator](https://vinkius.com/en/ai-agent-connect/venture-tag-along-rights-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Tag-Along Rights Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-tag-along-rights-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Tag-Along Rights Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-tag-along-rights-calculator": {
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

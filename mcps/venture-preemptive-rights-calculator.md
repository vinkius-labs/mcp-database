# Venture Preemptive Rights Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/venture-preemptive-rights-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculates the monetary and strategic value of shareholder preemptive rights to prevent dilution.

## Description
This MCP server provides precise valuation models for shareholder preemptive rights. It allows AI agents to quantify the economic and strategic impact of future financing rounds. Using tools like `calculate_preemptive_rights_total`, agents can determine the capital required for ownership maintenance, the economic benefit of anti-dilution protections, and the strategic optionality provided by notice periods and oversubscription provisions. This is essential for venture capital analysis and shareholder protection modeling.


## Available Tools (4)
- **calculate_preemptive_rights_total**: Aggregates all components into a comprehensive valuation
- **calculate_anti_dilution_benefit**: Estimates the economic protection provided against dilution
- **calculate_ownership_maintenance**: Determines the capital required to prevent ownership dilution
- **calculate_strategic_optionality**: Quantifies the value of the choice to invest or abstain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Venture Preemptive Rights Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total preemptive rights value for a 10% shareholder in a $5M round with a $50M post-money valuation, 70% probability, 30-day notice, and oversubscription available."

**🤖 AI Agent:**
> The total preemptive rights value is $500,000, which includes $350,000 for ownership maintenance, $105,000 for anti-dilution benefit, and $45,000 for strategic optionality.

---

**👤 You:**
> "How much capital is needed to maintain a 5% stake in a $10M financing round with a $40M post-money valuation?"

**🤖 AI Agent:**
> The capital required to maintain a 5% ownership stake is $500,000.

---

**👤 You:**
> "What is the strategic optionality value if the financing probability is 0.5, notice period is 15 days, and no oversubscription is available?"

**🤖 AI Agent:**
> The strategic optionality value is $12,500 with a flexibility score of 0.4.


## ❓ FAQ

**Q: What does the total valuation include?**
The total value is the sum of ownership maintenance capital, anti-dilution economic benefits, and strategic optionality, all weighted by the probability of the future financing event.

**Q: How is strategic optionality calculated?**
It uses `calculate_strategic_optionality` to evaluate the value of the choice to invest based on the probability of a round, the notice period, and whether oversubscription is available.

**Q: Can I calculate the specific capital needed to maintain my stake?**
Yes, you can use the `calculate_ownership_maintenance` tool to determine the exact dollar amount required to prevent ownership dilution in a future round.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/venture-preemptive-rights-calculator](https://vinkius.com/en/ai-agent-connect/venture-preemptive-rights-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Venture Preemptive Rights Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `venture-preemptive-rights-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Venture Preemptive Rights Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "venture-preemptive-rights-calculator": {
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

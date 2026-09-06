# Infra Exit Option Analysis MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/infra-exit-option-analysis)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Calculates strategic and financial exit valuations and optimal timing for infrastructure startups.

## Description
This MCP server provides decision-support tools for infrastructure startups to evaluate their exit potential. It calculates strategic value for competitors and financial value for infrastructure funds. Use `analyze_exit_scenarios` to compare paths, `calculate_strategic_valuation` for synergy-based pricing, `calculate_financial_valuation` for yield-based pricing, or `optimize_exit_timing` to find the most lucrative exit window.


## Available Tools (4)
- **analyze_exit_scenarios**: Compares strategic and financial exit paths to provide a side-by-side comparison
- **calculate_financial_valuation**: Determines the potential exit price when selling to a financial buyer
- **calculate_strategic_valuation**: Determines the potential exit price when selling to a strategic buyer
- **optimize_exit_timing**: Identifies the optimal year to exit to maximize total valuation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Infra Exit Option Analysis** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Compare the strategic and financial exit options for a startup with a $50M asset base, $10M revenue, 15% growth, 0.8 strategic interest, and 0.9 fund appetite."

**🤖 AI Agent:**
> The strategic path yields a valuation of $85M, while the financial path yields $72M. The recommended path is the strategic exit.

---

**👤 You:**
> "What is the optimal year to exit if current revenue is $5M, growth is 10%, market conditions are stable, and the time horizon is 5 years?"

**🤖 AI Agent:**
> The optimal exit year is Year 4, with a projected maximum valuation of $7.32M.

---

**👤 You:**
> "Calculate the strategic valuation for an infrastructure company with $100M in assets, $20M revenue, 5% growth, 0.7 strategic interest, and 0.8 asset quality."

**🤖 AI Agent:**
> The strategic valuation is $126M.


## ❓ FAQ

**Q: How does this tool determine strategic value?**
Strategic value is calculated by assessing the asset base and revenue, then scaling by growth rates, strategic interest, and asset quality via `calculate_strategic_valuation`.

**Q: Can I compare different exit paths?**
Yes, you can use `analyze_exit_scenarios` to receive a side-by-side comparison of strategic and financial exit paths.

**Q: How is the optimal exit year identified?**
The `optimize_exit_timing` tool identifies the best year by balancing revenue growth against market condition trends.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/infra-exit-option-analysis](https://vinkius.com/ai-agent-connect/infra-exit-option-analysis)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Infra Exit Option Analysis** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `infra-exit-option-analysis` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Infra Exit Option Analysis** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "infra-exit-option-analysis": {
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

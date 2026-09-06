# Infra Finance Analyzer MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/infra-finance-analyzer)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [infrastructure](../categories/infrastructure.md)

Compare ROE vs IRR for infrastructure investments.

## Description
This MCP server provides specialized financial tools to evaluate infrastructure project profitability. Use `analyze_unlevered_return` to find the fundamental project return, `analyze_levered_return` to calculate investor ROE after debt and taxes, `optimize_capital_structure` to find the ideal debt level, and `compare_returns_profile` to assess leverage effectiveness.


## Available Tools (4)
- **analyze_levered_return**: Calculate the actual return seen by the investor after accounting for debt servicing and tax benefits
- **analyze_unlevered_return**: Determine the fundamental profitability of the infrastructure project before considering any debt
- **compare_returns_profile**: Provide a high-level comparison between the project's organic performance and the investor's leveraged performance
- **optimize_capital_structure**: Identify the most efficient level of debt to maximize investor returns


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Infra Finance Analyzer** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the fundamental return for a project with $10M equity and $15M in returns?"

**🤖 AI Agent:**
> The unlevered IRR for this project is 50%.

---

**👤 You:**
> "Calculate the levered ROE for $5M equity, $12M returns, a 2.0 leverage ratio, 5% cost of debt, and 20% tax rate."

**🤖 AI Agent:**
> The levered ROE is 144%.

---

**👤 You:**
> "Is it worth using debt for a project with 10% IRR and 15% ROE?"

**🤖 AI Agent:**
> Yes, the use of debt is value-adding as the levered ROE exceeds the unlevered IRR.


## ❓ FAQ

**Q: How do I calculate the fundamental return of a project?**
You can use the `analyze_unlevered_return` tool to determine the project's inherent profitability before any debt is applied.

**Q: Can this tool help find the best debt level?**
Yes, the `optimize_capital_structure` tool identifies the optimal leverage ratio to maximize your levered ROE.

**Q: Does the tool account for tax benefits?**
Yes, `analyze_levered_return` incorporates the tax shield provided by interest payments to calculate the net return.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/infra-finance-analyzer](https://vinkius.com/ai-agent-connect/infra-finance-analyzer)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Infra Finance Analyzer** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `infra-finance-analyzer` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Infra Finance Analyzer** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "infra-finance-analyzer": {
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

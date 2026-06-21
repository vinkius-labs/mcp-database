# PIS/COFINS Tax Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/piscofins-tax-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate PIS and COFINS tax liabilities for cumulative and non-cumulative regimes.

## Description
This MCP server provides specialized tools to calculate Brazilian social contributions (PIS and COFINS). Use `calculate_cumulative_tax` for simplified taxation with fixed rates, `calculate_non_cumulative_tax` to account for input credits in the complex regime, or `evaluate_regime_comparison` to determine the most tax-efficient method based on your revenue and operational costs.


## Available Tools
- **calculate_cumulative_tax**: Calculate PIS and COFINS liability under the cumulative regime
- **calculate_non_cumulative_tax**: Calculate net PIS and COFINS liability under the non-cumulative regime
- **evaluate_regime_comparison**: Compare cumulative and non-cumulative taxation regimes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **PIS/COFINS Tax Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate my PIS/COFINS for 100,000 BRL revenue in the cumulative regime."

**🤖 AI Agent:**
> The `calculate_cumulative_tax` tool would return a PIS amount of 650.00 and COFINS of 3,000.00, totaling 3,650.00.

---

**👤 You:**
> "Compare regimes for 500,000 BRL revenue with 50,000 BRL in raw material costs."

**🤖 AI Agent:**
> Using `evaluate_regime_comparison`, the tool will analyze both regimes and suggest the one with the lowest net liability based on your input credits.

---

**👤 You:**
> "What is my tax liability if I have 200,000 BRL revenue and 20,000 BRL in energy costs?"

**🤖 AI Agent:**
> By calling `calculate_non_cumulative_tax` with the provided input credits, you can see your net PIS and COFINS balance.


## ❓ FAQ

**Q: How do I calculate taxes for the cumulative regime?**
Use the `calculate_cumulative_tax` tool by providing your total gross revenue. The tool applies a 0.65% rate for PIS and 3% for COFINS.

**Q: Can I include input credits in the calculation?**
Yes, when using `calculate_non_cumulative_tax`, you can provide a JSON array of input costs (like raw materials or energy) to calculate available tax credits.

**Q: How does the regime comparison tool work?**
The `evaluate_regime_comparison` tool calculates both taxation methods simultaneously and recommends the one that results in a lower total tax burden.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/piscofins-tax-calculator](https://vinkius.com/mcp/piscofins-tax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **PIS/COFINS Tax Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE", enter `piscofins-tax-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **PIS/COFINS Tax Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "piscofins-tax-calculator": {
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

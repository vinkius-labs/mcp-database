# Seller Net Proceeds Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/seller-net-proceeds-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate the final cash amount a seller retains after all transaction costs.

## Description
This MCP server provides precise financial calculations for real estate transactions. It allows AI agents to determine the exact net proceeds a seller will receive by accounting for mortgage payoffs, agent commissions, seller concessions, transfer taxes, repair costs, and closing fees. Using tools like `calculate_net_proceeds`, `estimate_commission_impact`, `calculate_tax_burden`, and `validate_sale_feasibility`, agents can provide clear financial breakdowns and feasibility checks for property sales.


## Available Tools (4)
- **calculate_net_proceeds**: Calculate the net proceeds a seller will receive after all deductions
- **calculate_tax_burden**: Calculate the amount of transfer taxes owed
- **estimate_commission_impact**: Estimate how much the agent commission will reduce the total proceeds
- **validate_sale_feasibility**: Check if the sale price is sufficient to cover debts and expenses


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Seller Net Proceeds Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will I walk away with if I sell my house for $500,000 with a $300,000 mortgage payoff, 6% commission, and $5,000 in closing fees?"

**🤖 AI Agent:**
> Your estimated net proceeds are $165,000. This accounts for the $30,000 commission, $300,000 mortgage payoff, and $5,000 in closing fees.

---

**👤 You:**
> "What will the agent commission be for a $750,000 sale at a 5% rate?"

**🤖 AI Agent:**
> The agent commission will be $37,500.

---

**👤 You:**
> "Is a sale price of $250,000 feasible if I owe $240,000 on my mortgage and expect $15,000 in total expenses?"

**🤖 AI Agent:**
> No, the sale is not feasible as the total obligations ($255,000) exceed the sale price ($250,000).


## ❓ FAQ

**Q: What is included in the net proceeds calculation?**
The calculation subtracts the mortgage payoff, agent commissions, seller concessions, transfer taxes, repair costs, and closing fees from the gross sale price.

**Q: Can I check if my sale price is high enough to cover my debts?**
Yes, you can use the `validate_sale_feasibility` tool to check if the proposed sale price covers your mortgage payoff and estimated expenses.

**Q: How are transfer taxes calculated?**
Transfer taxes are calculated by multiplying the gross sale price by the local jurisdiction's tax rate using the `calculate_tax_burden` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/seller-net-proceeds-estimator](https://vinkius.com/en/ai-agent-connect/seller-net-proceeds-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Seller Net Proceeds Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `seller-net-proceeds-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Seller Net Proceeds Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "seller-net-proceeds-estimator": {
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

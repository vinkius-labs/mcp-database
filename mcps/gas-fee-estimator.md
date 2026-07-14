# Gas Fee Estimator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/gas-fee-estimator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Estimate blockchain transaction costs for EVM-compatible chains.

## Description
The Gas Fee Estimator provides precise calculations for Ethereum Virtual Machine (EVM) compatible networks. It calculates total gas costs using `calculate_gas_cost` based on gas limits and EIP-1559 fees, converts native token expenditures to fiat values via `convert_gas_to_fiat`, suggests optimal tip amounts with `recommend_priority_fee` by analyzing recent fee history, and enables side-by-side cost comparisons across multiple chains using `compare_chain_costs`.


## Available Tools (4)
- **compare_chain_costs**: Compare transaction costs across different blockchains
- **convert_gas_to_fiat**: g., USD).

Convert a native token cost into its fiat currency value
- **calculate_gas_cost**: Calculate the total cost of a transaction in native tokens
- **recommend_priority_fee**: Suggest a priority fee based on recent network activity


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Gas Fee Estimator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the total cost in ETH for a transaction with 21000 gas limit, 50 gwei base fee, and 2 gwei tip?"

**🤖 AI Agent:**
> The total gas price is 52 gwei, resulting in a total cost of 0.001092 ETH.

---

**👤 You:**
> "Convert 0.5 ETH to USD assuming an exchange rate of 2500."

**🤖 AI Agent:**
> The transaction cost is 1250.0 USD.

---

**👤 You:**
> "Based on this history: '[{"baseFee": 50, "priorityFee": 2}, {"baseFee": 55, "priorityFee": 3}]', what is a good fast priority fee?"

**🤖 AI Agent:**
> For the 'fast' tier, a recommended priority fee is 4 gwei.


## ❓ FAQ

**Q: How can I calculate the total cost of an Ethereum transaction?**
You can use the `calculate_gas_cost` tool by providing the gas limit, base fee, and priority fee.

**Q: How do I know what priority fee to set for a fast transaction?**
The `recommend_priority_fee` tool analyzes recent network activity to suggest the best tip for 'slow', 'standard', or 'fast' tiers.

**Q: Can I compare costs between Polygon and Ethereum?**
Yes, the `compare_chain_costs` tool allows you to input estimates for multiple chains and see a side-by-side comparison.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/gas-fee-estimator](https://vinkius.com/mcp/gas-fee-estimator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Gas Fee Estimator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `gas-fee-estimator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Gas Fee Estimator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "gas-fee-estimator": {
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

# Accelerator Economics Engine MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/accelerator-economics-engine)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate detailed per-company economic impact and value delivery optimization.

## Description
This MCP server provides advanced economic modeling for accelerator programs. It allows AI agents to evaluate the net economic value of participating companies by analyzing direct costs against equity, services, network, and brand value. Use `calculate_company_net_economics` to determine profitability, `analyze_cost_composition` to assess the quality of economic returns, and `optimize_value_delivery` to find the necessary adjustments to reach target economic ratios.


## Available Tools (3)
- **calculate_company_net_economics**: Determines the total economic impact and profitability of a single company
- **optimize_value_delivery**: Suggests adjustments to maximize net economics based on current cost and value inputs
- **analyze_cost_composition**: Breaks down the ratio of tangible cash costs versus intangible value creation


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Accelerator Economics Engine** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the net economics for a company with $50,000 direct costs, $200,000 equity value, $30,000 services value, $20,000 network value, and $10,000 brand value."

**🤖 AI Agent:**
> The total value delivered is $260,000, and the net economics is $210,000 with an economic ratio of 5.2.

---

**👤 You:**
> "Analyze the cost composition for $100,000 direct costs and $150,000 in intangible value."

**🤖 AI Agent:**
> The cost to value ratio is 0.67, the cash to intangible ratio is 0.67, and the return is value-driven.

---

**👤 You:**
> "Suggest how to optimize economics if I have $80,000 in costs, $100,000 in total value, and I want a target economic ratio of 2.0."

**🤖 AI Agent:**
> To reach a target ratio of 2.0, you need a required value increase of $60,000 or a required cost reduction of $30,000.


## ❓ FAQ

**Q: How do I calculate the net economic value of a company?**
You can use the `calculate_company_net_economics` tool. Provide the direct costs, equity value, program services value, network value, and brand value to get the net economics and economic ratio.

**Q: Can I optimize my program's economic performance?**
Yes, the `optimize_value_delivery` tool suggests specific actions, such as required value increases or cost reductions, to help you reach a target economic ratio.

**Q: What is the difference between cash costs and intangible value?**
Direct costs are tangible cash expenditures, while intangible value includes the market value of services, network access, and brand association. You can use `analyze_cost_composition` to see the ratio between them.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/accelerator-economics-engine](https://vinkius.com/ai-agent-connect/accelerator-economics-engine)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Accelerator Economics Engine** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `accelerator-economics-engine` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Accelerator Economics Engine** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "accelerator-economics-engine": {
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

# Depletion Allowance Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/depletion-allowance-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate tax-deductible depletion allowances for oil and gas properties.

## Description
This MCP server provides specialized financial tools to calculate depletion allowances for natural resource properties. It allows users to determine tax deductions using both Cost Depletion and Percentage Depletion methods. Use `calculate_cost_depletion` to find deductions based on property cost and reserves, or `calculate_percentage_depletion` to calculate deductions based on gross income and statutory rates. You can also use `compare_methods` to identify the most tax-efficient approach and `get_property_summary` to track the remaining basis and recovery progress.


## Available Tools (4)
- **calculate_percentage_depletion**: Calculate depletion deduction using the Percentage Depletion method
- **compare_methods**: Compare Cost Depletion and Percentage Depletion methods
- **get_property_summary**: Get a summary of the property investment recovery status
- **calculate_cost_depletion**: Calculate depletion deduction using the Cost Depletion method


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Depletion Allowance Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the cost depletion for a property with an original cost of $500,000, total reserves of 100,000 barrels, and an annual production of 5,000 barrels, with a current basis of $500,000."

**🤖 AI Agent:**
> The annual depletion deduction is $2,500.00, and the remaining basis is $497,500.00.

---

**👤 You:**
> "What is the percentage depletion for a production with $100,000 gross income, a current basis of $200,000, and a depletion rate of 15%?"

**🤖 AI Agent:**
> The annual depletion deduction is $15,000.00, and the remaining basis is $185,000.00.

---

**👤 You:**
> "Compare cost depletion of $5,000 and percentage depletion of $7,000 with a marginal tax rate of 24%."

**🤖 AI Agent:**
> The optimal method is Percentage Depletion, providing an annual deduction of $7,000. This results in a tax savings difference of $480.00 compared to Cost Depletion.


## ❓ FAQ

**Q: What is the difference between Cost and Percentage Depletion?**
Cost Depletion is based on the actual cost of the property relative to its reserves, while Percentage Depletion is a fixed percentage of gross income, limited by the remaining basis.

**Q: How can I find the best tax deduction method?**
You can use the `compare_methods` tool to compare the results of both methods and determine which provides the higher deduction for your current production.

**Q: Can I track my remaining investment basis?**
Yes, the `get_property_summary` tool provides the remaining basis and the percentage of the original cost that has been recovered.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/depletion-allowance-calculator](https://vinkius.com/ai-agent-connect/depletion-allowance-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Depletion Allowance Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `depletion-allowance-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Depletion Allowance Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "depletion-allowance-calculator": {
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

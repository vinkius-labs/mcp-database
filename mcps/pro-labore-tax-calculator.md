# Pro-Labore Tax Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/pro-labore-tax-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate INSS, IRRF, and compare compensation strategies for business partners.

## Description
This MCP server provides a specialized financial engine to calculate the tax burden on partner compensation. It allows users to determine mandatory deductions like INSS (Social Security) and progressive IRRF (Income Tax) based on gross pro-labore amounts. Additionally, it enables comparing two distinct strategies: achieving a target net income through full pro-labore versus a hybrid model using both taxable pro-labore and tax-exempt profit distribution. Use `calculate_tax_breakdown` to see specific deductions, `compare_compensation_strategies` for strategic planning, and `validate_tax_parameters` to check against current regulatory ceilings.


## Available Tools (3)
- **calculate_tax_breakdown**: Calculates all mandatory tax deductions and the final net amount for a specific gross pro-labore value
- **validate_tax_parameters**: Verifies if a provided amount is within the valid operational bounds
- **compare_compensation_strategies**: Compares two methods of achieving a specific target monthly income


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Pro-Labore Tax Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the tax breakdown for a gross pro-labore of $5,000."

**🤖 AI Agent:**
> For a gross amount of $5,000.00:
- INSS Deduction: $550.00
- IRRF Deduction: $425.30
- Net Amount: $4,024.70

---

**👤 You:**
> "Compare strategies for a target net income of $10,000 with a $2,000 pro-labore component."

**🤖 AI Agent:**
> Comparison Results:
- Strategy A (Full Pro-labore) Total Tax: $2,450.00
- Strategy B (Hybrid Model) Total Tax: $185.00
- Potential Tax Savings: $2,265.00

---

**👤 You:**
> "Is an amount of $8,000 subject to the INSS ceiling?"

**🤖 AI Agent:**
> Yes, an amount of $8,000.00 has reached or exceeded the current INSS contribution ceiling.


## ❓ FAQ

**Q: What does the `calculate_tax_breakdown` tool do?**
It calculates the INSS deduction, IRRF income tax, and the final net amount for a given gross pro-labore value.

**Q: How can I compare different payment methods?**
Use the `compare_compensation_strategies` tool. It compares a strategy where the entire target income is taxed as pro-labore against a hybrid model using both taxable pro-labore and exempt profit distribution.

**Q: Does the tool account for the INSS ceiling?**
Yes, the engine automatically applies the current INSS contribution ceiling to ensure deductions do not exceed regulatory limits.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/pro-labore-tax-calculator](https://vinkius.com/mcp/pro-labore-tax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Pro-Labore Tax Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `pro-labore-tax-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Pro-Labore Tax Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "pro-labore-tax-calculator": {
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

# France Income Tax Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/france-income-tax-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate French income tax using the quotient familial system, progressive brackets, and social contributions.

## Description
This MCP server provides a specialized calculation engine for determining personal income tax liabilities in France. It implements the complex 'quotient familial' system, which adjusts taxable income based on the number of dependents (children) in a household. By using tools like `calculate_tax_burden`, users can determine their total tax liability, including social contributions (CSG/CRDS), and see their resulting net income. The server also includes `compute_fiscal_parts` to calculate household parts and `assess_marginal_pressure` to analyze the difference between average and marginal tax rates. It is an essential tool for financial planning and understanding the impact of family changes on French taxation.


## Available Tools (3)
- **compute_fiscal_parts**: 5 for first two, 1.0 for others).

Calculate the number of fiscal parts based on children
- **assess_marginal_pressure**: Analyze tax pressure from marginal vs average rates
- **calculate_tax_burden**: Calculate total tax burden and net income


## 💬 Prompt Examples

Here are some examples of how you can interact with the **France Income Tax Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much tax will I pay if my gross taxable income is 50,000 EUR and I have 2 children?"

**🤖 AI Agent:**
> With a gross income of 50,000 EUR and 2 children, your total tax liability is approximately 4,875.00 EUR, which includes both income tax and social contributions (CSG/CRDS). Your estimated net income would be 45,125.00 EUR.

---

**👤 You:**
> "Calculate the number of fiscal parts for a household with 3 children."

**🤖 AI Agent:**
> A household with 3 children is entitled to 2.5 fiscal parts (1 base + 0.5 for the first child + 0.5 for the second child + 0.5 for the third child).

---

**👤 You:**
> "What is my tax pressure if I earn 100,000 EUR with no children?"

**🤖 AI Agent:**
> With an income of 100,000 EUR and no children, your average tax rate is approximately 20.45%, while your marginal tax rate is 41%. This results in a significant gap between the two rates.


## ❓ FAQ

**Q: How does the quotient familial system work?**
The system divides your taxable income by a number of 'fiscal parts' determined by your household size and children. This reduces the amount of income subject to higher tax brackets.

**Q: What are social contributions (CSG/CRDS)?**
These are mandatory social levies in France, calculated at a fixed rate of 9.7% on your gross taxable income, alongside the progressive income tax.

**Q: Can I use this to see my net income?**
Yes, by using the `calculate_tax_burden` tool, you can input your gross taxable income and number of children to receive a detailed breakdown including net income.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/france-income-tax-calculator](https://vinkius.com/mcp/france-income-tax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **France Income Tax Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `france-income-tax-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **France Income Tax Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "france-income-tax-calculator": {
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

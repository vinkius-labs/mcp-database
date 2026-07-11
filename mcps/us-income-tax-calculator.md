# US Income Tax Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-income-tax-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate US federal, state, and local income tax liabilities including SECA, LTCG, and credits.

## Description
A specialized calculation engine for determining US federal, state, and local income tax liabilities. The MCP server provides tools to calculate the split between ordinary income, capital gains, and NIIT, as well as computing combined state/local taxation for all 50 states. Use `calculate_self_employment_impact` to determine SECA tax liability and deductible portions of self-employment income. Additionally, use `apply_credits_and_deductions` to calculate final adjustments including standard deductions, Child Tax Credit phase-outs, and EITC. The server also supports calculating state/local taxes via `calculate_state_local_taxation` for jurisdictions like NYC or DC.


## Available Tools (4)
- **apply_credits_and_deductions**: Calculate final tax adjustments
- **calculate_federal_tax_layers**: Calculate split between ordinary, capital gains, and NIIT
- **calculate_self_employment_impact**: Calculate SECA tax and deductible portion
- **calculate_state_local_taxation**: g., NYC, DC).

Compute combined state and local tax liability


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Income Tax Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much self-employment tax will I owe on $50,000 of income?"

**🤖 AI Agent:**
> On $50,000 of gross self-employment income, your total SECA tax is approximately $7,065, with a deductible portion of $3,532.50 to reduce your AGI.

---

**👤 You:**
> "Calculate my federal tax layers for an AGI of $100,000 with $10,000 in LTCG and MFJ status."

**🤖 AI Agent:**
> For a Married Filing Jointly status with $100,000 AGI, your ordinary income tax is calculated across the progressive brackets, while your capital gains tax on $10,000 of LTCG remains at 0% based on current thresholds.

---

**👤 You:**
> "What is my state tax for New York?"

**🤖 AI Agent:**
> For taxable income in New York, the calculation includes both the state-level progressive tax and any applicable local taxes like NYC, depending on your specific jurisdiction.


## ❓ FAQ

**Q: Does this tool account for self-employment tax?**
Yes, you can use `calculate_self_employment_impact` to determine your total SECA tax liability and the deductible portion that reduces your AGI.

**Q: Can I calculate state-specific taxes?**
Yes, the `calculate_state_local_taxation` tool allows you to compute liabilities for any of the 50 US states and specific local jurisdictions like NYC or DC.

**Q: How are capital gains handled?**
The `calculate_federal_tax_layers` tool calculates the split between ordinary income tax, preferential rates for long-term capital gains and qualified dividends, and the NIIT surcharge.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-income-tax-calculator](https://vinkius.com/mcp/us-income-tax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Income Tax Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-income-tax-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Income Tax Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-income-tax-calculator": {
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

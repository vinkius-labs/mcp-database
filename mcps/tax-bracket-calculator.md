# Tax Bracket Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/ai-agent-connect/tax-bracket-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate marginal and effective tax rates, standard deductions, and capital gains.

## Description
This MCP server provides precise tax calculations for US federal income tax. It connects AI agents to tools like `calculate_tax_liability` to determine total tax owed, `get_tax_brackets` to view progressive income segments, and `get_standard_deduction` to find applicable income shields. The server accounts for filing status, tax year, and handles capital gains rates separately from ordinary income to provide accurate effective and marginal tax rates.


## Available Tools (3)
- **calculate_tax_liability**: Calculate total tax liability including ordinary and capital gains tax
- **get_standard_deduction**: Retrieve the standard deduction amount for a specific filing status and year
- **get_tax_brackets**: Retrieve progressive tax brackets for a specific filing status and year


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tax Bracket Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is my total tax liability if I have $75,000 in ordinary income and $5,000 in capital gains as a single filer in 2024?"

**🤖 AI Agent:**
> For a single filer in 2024 with $75,000 ordinary income and $5,000 capital gains, your total tax owed is $8,645.00, with an effective tax rate of 11.53%.

---

**👤 You:**
> "Show me the tax brackets for a married filing jointly status for the 2023 tax year."

**🤖 AI Agent:**
> The 2023 tax brackets for Married Filing Jointly are: 10% on income up to $22,000, 12% on income between $22,001 and $89,450, 22% on income between $89,451 and $190,750, and so on.

---

**👤 You:**
> "How much is the standard deduction for Head of Household in 2024?"

**🤖 AI Agent:**
> The standard deduction for Head of Household in 2024 is $21,900.


## ❓ FAQ

**Q: How does this tool handle different filing statuses?**
The `calculate_tax_liability` tool uses the provided filing status (Single, Married Filing Jointly, Married Filing Separately, or Head of Household) to select the correct standard deduction and progressive tax brackets for the specified tax year.

**Q: Does it account for capital gains?**
Yes, you can provide capital gains as an optional input to `calculate_tax_liability`. The tool calculates capital gains tax using the appropriate 0%, 15%, or 20% rates based on your total income.

**Q: Can I check the standard deduction for a specific year?**
Yes, use the `get_standard_deduction` tool by providing your filing status and the desired tax year to see how much income is shielded from taxation.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/ai-agent-connect/tax-bracket-calculator](https://vinkius.com/ai-agent-connect/tax-bracket-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tax Bracket Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tax-bracket-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tax Bracket Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tax-bracket-calculator": {
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

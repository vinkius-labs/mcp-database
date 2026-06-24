# US Self-Employment Tax Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-self-employment-tax-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate US Self-Employment tax (Social Security and Medicare) and associated income tax deductions for the 202rag year.

## Description
This MCP server provides specialized tools to calculate US Self-Employment (SE) tax liabilities. It breaks down the total obligation into its Social Security (12.4%) and Medicare (2.9%) components, applying the 2024 Social Security wage base limit of $168,600. Use `calculate_se_tax` to see the breakdown of your taxes, `calculate_deductible_amount` to find your tax deduction, and `get_tax_impact_summary` for a complete overview of your financial impact.


## Available Tools (3)
- **calculate_deductible_amount**: Calculates the SE tax deduction amount
- **calculate_se_tax**: 4%) and Medicare (2/9%) components based on 2024 limits ($168,600).

Calculates the breakdown of total Self-Employment tax
- **get_tax_impact_summary**: Provides a summary of the financial impact of SE taxes


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Self-Employment Tax Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much is my self-employment tax if my net profit is $50,000?"

**🤖 AI Agent:**
> For a net profit of $50,000, your total Self-Employment tax is $7,650. This consists of $6,200 for Social Security and $1,450 for Medicare.

---

**👤 You:**
> "Calculate the tax impact for a net profit of $200,000."

**🤖 AI Agent:**
> With a net profit of $200,000, your total SE tax liability is $29,144. This includes the capped Social Security component and the full Medicare component on all earnings.

---

**👤 You:**
> "What is my deductible amount if my SE tax is $10,000?"

**🤖 AI Agent:**
> Your deductible amount is $5,000.


## ❓ FAQ

**Q: What is included in the Self-Employment tax calculation?**
The calculation includes both Social Security (12.4%) and Medicare (2.9%) taxes. The Social Security portion is subject to the annual wage base limit.

**Q: How can I find my deductible amount?**
You can use the `calculate_deductible_amount` tool. It calculates exactly 50% of your total Self-Employment tax, which is the amount you can deduct from your gross income.

**Q: Does this tool account for the 2024 Social Security limit?**
Yes, the `calculate_se_tax` tool applies the $168,600 wage base limit for the 2024 tax year.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-self-employment-tax-calculator](https://vinkius.com/mcp/us-self-employment-tax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Self-Employment Tax Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-self-employment-tax-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Self-Employment Tax Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-self-employment-tax-calculator": {
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

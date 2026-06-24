# US Capital Gains Tax Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-capital-gains-tax-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate US capital gains tax liability based on holding periods and taxable income.

## Description
This MCP server provides tools to determine if a transaction results in a short-term or long-term capital gain and estimates the resulting tax liability. Use `calculate_gain_classification` to find your profit and classification based on how many days you held the asset. Then, use `estimate_tax_liability` with your annual taxable income and filing status to calculate exactly how much tax is owed. You can also use `get_tax_bracket_context` to see the specific income thresholds for long-term capital gains rates.


## Available Tools (3)
- **calculate_gain_classification**: Determines if a transaction results in short-term or long or long-term capital gain
- **get_tax_bracket_context**: Provides income thresholds for long-term tax rates
- **estimate_tax_liability**: Calculates the dollar amount of tax owed on a realized gain


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US Capital Gains Tax Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "I bought a stock for $1,000 and sold it for $2,500 after 400 days. What is my gain classification?"

**🤖 AI Agent:**
> Your transaction resulted in a long-term capital gain of $1,500.

---

**👤 You:**
> "I have a $5,000 long-term gain and my annual taxable income is $40,000 with a Single filing status. How much tax do I owe on this gain?"

**🤖 AI Agent:**
> The estimated tax due on your $5,000 gain is $0.00, as it falls within the 0% tax bracket for your income level.

---

**👤 You:**
> "What are the long-term capital gains thresholds for someone filing as Married Filing Jointly?"

**🤖 AI Agent:**
> For Married Filing Jointly, the thresholds are: Up to $94,050 = 0%, Up to $583,750 = 15%, and above $583,750 = 20%.


## ❓ FAQ

**Q: What is the difference between short-term and long-term capital gains?**
Short-term gains apply to assets held for one year or less and are taxed at your ordinary income tax rate. Long-term gains apply to assets held for more than one year and benefit from lower preferential rates of 0%, 15%, or 20%.

**Q: How do I calculate my tax liability?**
First, use `calculate_gain_classification` to determine your gain amount and whether it is short-term or long-term. Once you have the gain amount, use `estimate_tax_liability` along with your annual taxable income and filing status to find the total tax due.

**Q: Can I see the current tax thresholds?**
Yes, you can use the `get_tax_bracket_context` tool to retrieve a list of income thresholds and their associated long-term tax rates for your specific filing status.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-capital-gains-tax-calculator](https://vinkius.com/mcp/us-capital-gains-tax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US Capital Gains Tax Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-capital-gains-tax-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US Capital Gains Tax Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-capital-gains-tax-calculator": {
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

# Writing Contest Fee Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/writing-contest-fee-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculates granular cost breakdowns for writing contest entries, including taxes, discounts, and currency conversions.

## Description
This MCP server provides a precise financial engine for managing writing contest entry costs. It allows AI agents to compute detailed breakdowns for multiple contests simultaneously, accounting for base entry fees, optional professional feedback fees, discounts, and regional taxes. By using `get_contest_fee_breakdown`, agents can generate a complete financial overview including transaction fees and converted totals in target currencies. Additionally, tools like `calculate_tax_impact` and `get_currency_conversion_rate` provide granular control over specific financial components, ensuring accurate budgeting for participants across different geographic regions.


## Available Tools (4)
- **get_contest_fee_breakdown**: Provides a detailed cost analysis for a list of contests, including all adjustments and converted totals
- **get_currency_conversion_rate**: Retrieves the specific multiplier needed to convert from a base currency to a target currency
- **validate_contest_eligibility**: Verifies if a participant's selected discount or tax tier is valid for a specific contest type
- **calculate_tax_impact**: Determines the specific tax amount for a single contest entry


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Writing Contest Fee Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "Calculate the total cost for two contests: one with a $50 fee and 10% tax, and another with a $30 fee, a $15 feedback fee, and a 5% discount."

**🤖 AI Agent:**
> Contest 1: Total is $55.00. Contest 2: Total is $42.00.

---

**👤 You:**
> "What is the tax amount for a net entry fee of $100 with a tax rate of 0.08?"

**🤖 AI Agent:**
> The tax amount is $8.00.

---

**👤 You:**
> "Convert a $100 fee to EUR using an exchange rate of 0.92."

**🤖 AI Agent:**
> The total in EUR is €92.00.


## ❓ FAQ

**Q: How does the tool handle currency conversion?**
You can use `get_contest_fee_breakdown` by providing an array of exchange rates. The tool will automatically calculate the total target currency for each contest entry based on the provided rates.

**Q: Can I calculate taxes separately?**
Yes, the `calculate_tax_impact` tool allows you to determine the specific tax amount for a single entry given a net amount and a tax rate.

**Q: How do I check if a discount is valid for my contest type?**
Use the `validate_contest_eligibility` tool. It checks if a specific discount type is applicable to a contest category within a specific geographic region.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/writing-contest-fee-calculator](https://vinkius.com/en/ai-agent-connect/writing-contest-fee-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Writing Contest Fee Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `writing-contest-fee-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Writing Contest Fee Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "writing-contest-fee-calculator": {
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

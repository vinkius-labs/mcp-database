# Tax Percentage Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/en/ai-agent-connect/tax-percentage-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Derive tax rates and validate monetary tax figures.

## Description
This MCP server provides tools to calculate tax rates, validate tax figures, and compare different tax scenarios. Use `calculate_tax_rate` to find the percentage applied to a base amount, `validate_tax_figures` to ensure amounts are logically consistent, `get_tax_breakdown` for total costs, and `compare_tax_rates` to identify higher tax burdens.


## Available Tools (4)
- **calculate_tax_rate**: Calculates the tax percentage rate applied to a base amount
- **compare_tax_rates**: Compares two different tax scenarios
- **get_tax_breakdown**: Calculates the total cost including tax and the tax rate
- **validate_tax_figures**: Validates if the provided tax figures are logically consistent


## 💬 Prompt Examples

Here are some examples of how you can interact with the **Tax Percentage Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the tax rate for a $100 item with a $15 tax?"

**🤖 AI Agent:**
> The tax rate is 15%.

---

**👤 You:**
> "Calculate the total cost for a $50 base amount and $10 tax."

**🤖 AI Agent:**
> The total cost is $60, with a tax rate of 20%.

---

**👤 You:**
> "Which is higher: 10% tax on $200 or 12% tax on $150?"

**🤖 AI Agent:**
> The second scenario (12%) has a higher tax rate.


## ❓ FAQ

**Q: How do I calculate a tax rate?**
You can use the `calculate_tax_rate` tool by providing the taxable amount and the tax amount.

**Q: Can I compare two different tax scenarios?**
Yes, the `compare_tax_rates` tool allows you to determine which of two scenarios has a higher percentage rate.

**Q: What happens if the taxable amount is zero?**
The tool will return an error because a tax rate cannot be calculated when the base amount is zero.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/en/ai-agent-connect/tax-percentage-calculator](https://vinkius.com/en/ai-agent-connect/tax-percentage-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **Tax Percentage Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `tax-percentage-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **Tax Percentage Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "tax-percentage-calculator": {
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

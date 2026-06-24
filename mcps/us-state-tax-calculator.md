# US State Tax Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/us-state-tax-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate US state income tax rates and liabilities based on residency and taxable income.

## Description
This MCP server provides a specialized utility for determining US state income tax liabilities. By connecting your AI agent to this tool, you can instantly retrieve the specific tax rate for any of the 5 and identify states with no income tax. Use `get_state_rate` to find the decimal rate for a state, `calculate_state_liability` to compute total tax owed based on taxable income, and `list_no_tax_states` to see which jurisdictions like Texas or Florida have zero percent taxation. It acts as a bridge between your AI client--such as Cursor, VS Code, Claude Desktop, or Windsurf--and accurate US state tax data.


## Available Tools (3)
- **calculate_state_liability**: Calculate the total state income tax liability
- **get_state_rate**: Retrieve the tax rate for a specific US state
- **list_no_tax_states**: List all US states with no state income tax


## 💬 Prompt Examples

Here are some examples of how you can interact with the **US State Tax Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "What is the income tax rate in California?"

**🤖 AI Agent:**
> The income tax rate for California is 0.08.

---

**👤 You:**
> "If I earned $50,000 in Texas, how much state income tax do I owe?"

**🤖 AI Agent:**
> Since Texas is a zero-tax state, your state income tax liability is $0.00.

---

**👤 You:**
> "How much tax will I owe in New York on $100,000 of taxable income?"

**🤖 AI Agent:**
> Based on the current rate for New York, your estimated state tax liability is $6,500.00.


## ❓ FAQ

**Q: How do I find the tax rate for a specific state?**
Use the `get_state_rate` tool by providing the full name of the US state, such as 'California'.

**Q: Can I calculate my total tax liability?**
Yes, use the `calculate_state_liability` tool. You will need to provide the state name and your taxable income amount.

**Q: Which states have no state income tax?**
You can retrieve a complete list of all zero-tax jurisdictions by using the `list_no_tax_states` tool.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/us-state-tax-calculator](https://vinkius.com/mcp/us-state-tax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **US State Tax Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `us-state-tax-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **US State Tax Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "us-state-tax-calculator": {
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

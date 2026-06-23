# UK Income Tax Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uk-income-tax-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [finance](../categories/finance.md)

Calculate UK income tax liabilities, including personal allowance tapering and National Insurance contributions.

## Description
This MCP server provides precise calculations for United Kingdom income tax. It accounts for the Personal Allowance tapering that occurs when annual earnings exceed £100,000. Users can calculate specific liabilities using `calculate_income_tax` for income tax brackets, `calculate_national_insurance` for Class 1 and Class 4 contributions, or `get_tax_summary_report` for a complete breakdown of tax, NI, and net take-home pay.


## Available Tools (3)
- **get_tax_summary_report**: Get a comprehensive UK tax summary report
- **calculate_income_tax**: Calculate UK Income Tax liability
- **calculate_national_insurance**: Calculate UK National Insurance contribution


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UK Income Tax Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much income tax will I pay on £50,000 annual earnings?"

**🤖 AI Agent:**
> On an annual income of £50,000, your estimated income tax is £7,430 (based on standard thresholds).

---

**👤 You:**
> "Calculate my NI contribution for Class 1 with £30,000 earnings."

**🤖 AI Agent:**
> Your National Insurance Class 1 contribution on £30,000 is approximately £245.60.

---

**👤 You:**
> "What is my net take-home pay if I earn £120,000 as an employee?"

**🤖 AI Agent:**
> With £120,000 annual earnings as an employee, your estimated net take-home pay after Income Tax and Class 1 NI is approximately £84,500.


## ❓ FAQ

**Q: How does the Personal Allowance tapering work?**
If your annual earnings exceed £100,000, your Personal Allowance is reduced by £1 for every £2 earned above this threshold. This effectively increases the tax rate on income in this range.

**Q: What National Insurance classes are supported?**
The tool supports Class 1 NI (for employees) and Class 4 NI (for self-employed individuals).

**Q: Can I get a full breakdown of my take-home pay?**
Yes, by using the `get_tax_summary_report` tool, you can receive a comprehensive report including total income tax, total NI contributions, and your final net take-home pay.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uk-income-tax-calculator](https://vinkius.com/mcp/uk-income-tax-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UK Income Tax Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `uk-income-tax-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UK Income Tax Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "uk-income-tax-calculator": {
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

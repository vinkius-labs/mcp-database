# UK PAYE Calculator MCP Server

[![Deploy on Vinkius Edge](https://img.shields.io/badge/Deploy%20on-Vinkius%20Edge-blue?style=for-the-badge)](https://vinkius.com/mcp/uk-paye-calculator)
[![Built with MCP Fusion](https://img.shields.io/badge/Framework-MCP%20Fusion-success?style=for-the-badge)](https://www.npmjs.com/package/@mcpfusion/core)

## Overview

**Category:** [productivity](../categories/productivity.md)

Calculate UK Income Tax and National Insurance deductions for weekly or monthly pay periods.

## Description
The UK PAYE Calculator MCP server provides precise tools to estimate your take-home pay after tax. By using the `calculate_weekly_paye` and `calculate_monthly_paye` tools, you can determine exactly how much Income Tax and National Insurance (NI) will be deducted from your gross salary based on your specific UK tax code. Additionally, use `get_tax_code_allowance` to quickly translate any alphanumeric HMRC tax code into its corresponding annual personal allowance amount.


## Available Tools (3)
- **get_tax_code_allowance**: Get personal allowance from a UK tax code
- **calculate_monthly_paye**: Calculate monthly PAYE deductions
- **calculate_weekly_paye**: Calculate weekly PAYE deductions


## 💬 Prompt Examples

Here are some examples of how you can interact with the **UK PAYE Calculator** MCP server using an AI Agent (Claude, ChatGPT, etc.).

**👤 You:**
> "How much will my weekly take-home pay be if my annual salary is £35,000 and my tax code is 1257L?"

**🤖 AI Agent:**
> With an annual salary of £35,000 and a 1257L tax code, your weekly net pay is approximately £614.50, with £48.20 deducted for Income Tax and £22.30 for National Insurance.

---

**👤 You:**
> "What is the annual personal allowance for tax code 1257L?"

**🤖 AI Agent:**
> The annual personal allowance for tax code 12             57L is £12,570.

---

**👤 You:**
> "Calculate my monthly net pay for a £50,000 salary with tax code 1257L."

**🤖 AI Agent:**
> For a monthly gross salary of £4,166.67, your net monthly pay is approximately £3,245.50 after deducting £625.40 in Income Tax and £305.77 in National Insurance.


## ❓ FAQ

**Q: How do I calculate my monthly take-home pay?**
You can use the `calculate_monthly_paye` tool. Simply provide your annual gross salary and your UK tax code (e.g., 1257L) to get a breakdown of monthly net pay, income tax, and NI deductions.

**Q: What is a tax code?**
A UK tax code is an alphanumeric identifier used by HMRC to specify your personal allowance. You can use the `get_tax_code_allowance` tool to find out how much income you can earn before paying tax based on your code.

**Q: Does this tool include National Insurance deductions?**
Yes, both the weekly and monthly calculation tools automatically calculate your National Insurance contributions based on current UK thresholds.


## Installation & Usage

This MCP server is fully hosted and managed by **[Vinkius Cloud](https://vinkius.com)**, providing a zero-setup, high-performance, and secure execution environment. You do not need to manage local servers or dependencies. Simply connect your AI agent to the Vinkius Edge network using the instructions below.

1. View installation instructions and explore the server: [https://vinkius.com/mcp/uk-paye-calculator](https://vinkius.com/mcp/uk-paye-calculator)
2. Connect to the Vinkius Cloud to start using it: [cloud.vinkius.com/connect](https://cloud.vinkius.com/connect)

### Claude.ai
Follow the steps below to connect in seconds.

1. Open [claude.ai](https://claude.ai) and sign in to your account.
2. Go to **Customize → Connectors**.
3. Click the **+** button and select "Add custom connector".
4. Paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`) and save.
5. Click the **+** button in any chat and enable **UK PAYE Calculator** under Connectors.

### Cursor
Follow the steps below to connect in seconds.

1. In Cursor, open Settings (`⌘ ,`) → scroll to **Features** → **MCP Servers**.
2. Click **+ Add new MCP Server**.
3. Set Type to "SSE" (or "streamable HTTP"), enter `uk-paye-calculator` as the name, and paste the MCP server link (`https://edge.vinkius.com/[TOKEN]/mcp`).
4. Click **Save** — Cursor will connect and list all **UK PAYE Calculator** tools.

**Configuration:**
```json
{
  "mcpServers": {
    "uk-paye-calculator": {
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
